# 自然语言处理工具

## 文档中使用的自然语言处理工具包
- **hanlp**: 适用于基本自然语言处理任务，包括分词、词性分析、句法分析、语义分析、静态词向量提取等等，对于中文比较友好。[[官方文档]](https://hanlp.hankcs.com/docs/)

- **Huggingface系列**: AI模型社区，可以调用开源的深度学习模型完成更多任务，例如情感分析、句子语义嵌入、文本生成等等。[[官网]](https://huggingface.co/)

    ```{note}
    调用Huggingface中的模型时，我们可以使用Huggingface开发的transformers库以及相应的datasets库等等。Huggingface为模型的使用提供了完整的文档。[[NLP Course]](https://huggingface.co/learn/nlp-course/chapter1/1)
    ```

- **srilm**: SRILM是一个用于构建和应用统计语言模型的工具包。在本文档中，我们会使用[srilm-python](https://srilm-python.readthedocs.io/en/latest/#)调用SRILM来计算频次、转移概率。[[官方文档]](http://www.speech.sri.com/projects/srilm/)
    
    ```{note}
    srilm的安装较为复杂，具体可以参考[srilm-python](https://srilm-python.readthedocs.io/en/latest/#)和[pysrilm](https://github.com/zhaoyanpeng/pysrilm)。    
    ```

## 其他常用工具包
- **nltk**：可以调用众多语料库（如wordnet等），也可以进行一系列的自然语言处理任务。[[官方文档]](https://www.nltk.org/)
- **spacy**：速度快、功能全面的自然语言处理工具包。[[官方文档]](https://spacy.io/)
- **stanza**：Stanford CoreNLP的python版本。[[官方文档]](https://stanfordnlp.github.io/stanza/)
- **fastNLP**：复旦大学制作的NLP工具包。[[官方文档]](https://fastnlp.readthedocs.io/zh/latest/)