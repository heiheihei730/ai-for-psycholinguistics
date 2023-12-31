# FAQ

1. **Q**：汉语中如何根据字粒度模型计算词的转移概率？

    **A**：可以考虑用基于字级别的概率相乘来计算词汇级别的概率，例如：$p(蝴蝶|一只飞舞的)=p(蝴|一只飞舞的) \times p(蝶|一只飞舞的蝴)$

1. **Q**：模型输出的`output.logits`是下个词汇的预测分数，还需要用**softmax**转换为概率值吗？那么如果词汇概率通过字概率连乘，因为概率值在[0,1]中，词汇序列越长最终得出的词汇概率就会相对地越小，是否不合理呢?

    **A**：（1）需要用softmax将预测分数转换为概率值。（2）从概率上来说，字的概率包含了以这个字开头的所有词汇的概率，所以是合理。不过词汇的概率也不会特别小，以Q1中例子为例，如果模型足够好，那么$p(蝶|一只飞舞的蝴)$将约等于1，所以$p(蝴蝶|一只飞舞的)=p(蝴|一只飞舞的) \times p(蝶|一只飞舞的蝴)$的概率并不会太小。但模型实际情况如何，可能需要多进行一些测试才能知道。

1. **Q**：GPT模型的输出中，转移概率的维度是指? 如何提取语境下某个字的转移概率?

    **A**: 转移概率维度是词表的大小。如何提取请参考代码或者[语义特征](/semantic)。

1. **Q**：GPT模型中，如何根据根据input id得到对应字？

    **A**：可以使用[tokenizer](https://huggingface.co/learn/nlp-course/chapter2/4?fw=pt)的[convert_ids_to_token](https://huggingface.co/docs/transformers/v4.34.1/en/main_classes/tokenizer#transformers.PreTrainedTokenizer.convert_ids_to_tokens)函数获得的对应id的字。

1. **Q**：GPT模型的词表从哪里找？

    **A**：词表可以从模型文件夹下的vocab.txt里找到。

1. **Q**：GPT模型中，如何分别输入目标词和语境? 

    **A**：GPT模型不需要分别输入目标词和语境。只需要输入一句完整的句子，就可以得到一串输出，分别对应给定前文时每个位置的转移概率及其他目标。

1. **Q**：srilm安装不上？

    **A**：srilm的安装较为复杂，具体可以参考[srilm-python](https://srilm-python.readthedocs.io/en/latest/#)和[pysrilm](https://github.com/zhaoyanpeng/pysrilm)。 

1. **Q**：huggingface中的模型很多，该如何选择？有哪些参考指标？

    **A**：在显卡算力足够的情况下，模型越大越好。其次可以参考的指标包括下载量、模型对应文献的引用量等。最好是使用各种文献中常用的模型。

1. **Q**：用GPT2计算句子语境中关键词的surprisal时，在输入语境的时候，是否需要包括目标词呢？

    **A**：需要包括目标词。不知道目标词是什么的情况下，无法计算surprisal。

1. **Q**：大语言模型似乎还是不够准确，看起来还是基于语料库，而不是输入的语境。例如在句子“夏日里喝可乐的时候加一些”中，目标词是“冰”，与目标词语义相关但不合理的词是“雪”（评定出来的雪的合理性是比较低的），但是GPT计算出来“雪”的surprisal也是比较小的（surprisal=1.54）

    **A**：示例里的这个模型不是目前最先进的模型，所以和人的结果不一定会完全一致。可以考虑改成更厉害一些的模型。