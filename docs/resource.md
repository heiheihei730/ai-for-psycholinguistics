# 其他资源


## 语义和词汇特征

### 采用共现矩阵作为语义特征
1. Tom M. Mitchell et al. ,Predicting Human Brain Activity Associated with the Meanings of Nouns.Science320,1191-1195(2008).DOI:10.1126/science.1152876

1. Huth, A., de Heer, W., Griffiths, T. et al. Natural speech reveals the semantic maps that tile human cerebral cortex. Nature 532, 453–458 (2016). https://doi.org/10.1038/nature17637

1. Gong, X.L., Huth, A.G., Deniz, F. et al. Phonemic segmentation of narrative speech in human cerebral cortex. Nat Commun 14, 4309 (2023). https://doi.org/10.1038/s41467-023-39872-w


### 采用静态词向量（Word2Vec，GloVe等）作为语义特征
1. Michael P. Broderick, Andrew J. Anderson, Giovanni M. Di Liberto, Michael J. Crosse, Edmund C. Lalor, Electrophysiological Correlates of Semantic Dissimilarity Reflect the Comprehension of Natural, Narrative Speech, Current Biology, Volume 28, Issue 5, 2018, Pages 803-809.e3, ISSN 0960-9822, https://doi.org/10.1016/j.cub.2018.01.080.

1. Grand, G., Blank, I.A., Pereira, F. et al. Semantic projection recovers rich human knowledge of multiple object features from word embeddings. Nat Hum Behav 6, 975–987 (2022). https://doi.org/10.1038/s41562-022-01316-8

1. Lu, Y., Jin, P., Pan, X., & Ding, N. (2022). Delta-band neural activity primarily tracks sentences instead of semantic properties of words. NeuroImage, 251.

1. Lu, Y., Jin, P., Ding, N., & Tian, X. (2022). Delta-band neural tracking primarily reflects rule-based chunking instead of semantic relatedness between words. Cerebral Cortex (New York, NY), 33, 4448 - 4458.

1. Ze Fu, Xiaosha Wang, Xiaoying Wang, Huichao Yang, Jiahuan Wang, Tao Wei, Xuhong Liao, Zhiyuan Liu, Huimin Chen, Yanchao Bi, Different computational relations in language are captured by distinct brain systems, Cerebral Cortex, Volume 33, Issue 4, 15 February 2023, Pages 997–1013, https://doi.org/10.1093/cercor/bhac117


### 采用上下文词向量（gpt2等）作为语义特征
1. Caucheteux, C., King, JR. Brains and algorithms partially converge in natural language processing. Commun Biol 5, 134 (2022). https://doi.org/10.1038/s42003-022-03036-1

1. Schrimpf, M., Blank, I.A., Tuckute, G., Kauf, C., Hosseini, E.A., Kanwisher, N.G., Tenenbaum, J.B., & Fedorenko, E. (2020). The neural architecture of language: Integrative modeling converges on predictive processing. Proceedings of the National Academy of Sciences, 118.

1. Goldstein, A., Zada, Z., Buchnik, E. et al. Shared computational principles for language processing in humans and deep language models. Nat Neurosci 25, 369–380 (2022). https://doi.org/10.1038/s41593-022-01026-4

1. Aw, K.L., & Toneva, M. (2022). Training language models to summarize narratives improves brain alignment. International Conference on Learning Representations.

1. Caucheteux, C., Gramfort, A. & King, JR. Evidence of a predictive coding hierarchy in the human brain listening to speech. Nat Hum Behav 7, 430–441 (2023). https://doi.org/10.1038/s41562-022-01516-2

1. Tang, J., LeBel, A., Jain, S. et al. Semantic reconstruction of continuous language from non-invasive brain recordings. Nat Neurosci 26, 858–866 (2023). https://doi.org/10.1038/s41593-023-01304-9

1. Setti, F., Handjaras, G., Bottari, D. et al. A modality-independent proto-organization of human multisensory areas. Nat Hum Behav 7, 397–410 (2023). https://doi.org/10.1038/s41562-022-01507-3

1. Antonello, R., Vaidya, A.R., & Huth, A.G. (2023). Scaling laws for language encoding models in fMRI. ArXiv, abs/2305.11863.

1. Tuckute G, Sathe A, Srikant S, Taliaferro M, Wang M, Schrimpf M, Kay K, Fedorenko E. Driving and suppressing the human language network using large language models. bioRxiv [Preprint]. 2023 Oct 30:2023.04.16.537080. doi: 10.1101/2023.04.16.537080.


### 采用转移概率的研究
1. Brodbeck, C., Bhattasali, S., Heredia, A.C., Resnik, P., Simon, J.Z., & Lau, E.F. (2021). Parallel processing in speech perception with local and global representations of linguistic context. eLife, 11.

1. Goldstein, A., Zada, Z., Buchnik, E. et al. Shared computational principles for language processing in humans and deep language models. Nat Neurosci 25, 369–380 (2022). https://doi.org/10.1038/s41593-022-01026-4

1. Gwilliams, L., King, JR., Marantz, A. et al. Neural dynamics of phoneme sequences reveal position-invariant code for content and order. Nat Commun 13, 6606 (2022). https://doi.org/10.1038/s41467-022-34326-1

1. Byung-Doh Oh, William Schuler; Why Does Surprisal From Larger Transformer-Based Language Models Provide a Poorer Fit to Human Reading Times?. Transactions of the Association for Computational Linguistics 2023; 11 336–350. doi: https://doi.org/10.1162/tacl_a_00548

## 句法特征
1. Brennan JR, Stabler EP, Van Wagenen SE, Luh WM, Hale JT. Abstract linguistic structure correlates with temporal activity during naturalistic comprehension. Brain Lang. 2016 Jun-Jul;157-158:81-94. doi: 10.1016/j.bandl.2016.04.008.
1. Brennan JR, Dyer C, Kuncoro A, Hale JT. Localizing syntactic predictions using recurrent neural network grammars. Neuropsychologia. 2020 Sep;146:107479. doi: 10.1016/j.neuropsychologia.2020.107479. 
1. Stanojević, M., Brennan, J. R., Dunagan, D., Steedman, M., & Hale, J. T. (2023). Modeling Structure‐Building in the Brain With CCG Parsing and Large Language Models. Cognitive science, 47(7), e13312.

## 基于语音模型的语音特征
本次工作坊主要关注语言模型，但是最近语音模型也展现出强大的语言能力，例如语音识别、语音增强、语音分流等等。一些研究语音认知加工的工作也开始采用语音模型来提取语音以及语义特征。
1. Millet, J., Caucheteux, C., Orhan, P., Boubenec, Y., Gramfort, A., Dunbar, E., Pallier, C., & King, J. (2022). Toward a realistic model of speech processing in the brain with self-supervised learning. ArXiv, abs/2206.01685.
1. Vaidya, A.R., Jain, S., & Huth, A.G. (2022). Self-supervised models of audio effectively explain human cortical responses to speech. International Conference on Machine Learning.
1. Défossez, A., Caucheteux, C., Rapin, J. et al. Decoding speech perception from non-invasive brain recordings. Nat Mach Intell 5, 1097–1107 (2023). https://doi.org/10.1038/s42256-023-00714-5
1. Li, Y., Anumanchipalli, G.K., Mohamed, A. et al. Dissecting neural computations in the human auditory pathway using deep neural networks for speech. Nat Neurosci (2023). https://doi.org/10.1038/s41593-023-01468-4