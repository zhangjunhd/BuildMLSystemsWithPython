# Python自然语言处理

![cover](https://img3.doubanio.com/lpic/s27313176.jpg)

    作者: (美)Steven Bird Ewan Klein Edward Loper 
    出版社: 人民邮电出版社
    原作名: Natural Language Processing With Python
    译者: 张旭 / 崔阳 / 刘海平 
    出版年: 2014-6-25
    页数: 508
    定价: 89.00
    装帧: 平装
    ISBN: 9787115333681

[豆瓣链接](https://book.douban.com/subject/25916599/)

1. [NLTK入门][201]
    - 搜索文本
    - 计数词汇
    - 将文本当作词链表
    - 简单的统计
        - 频率分布
        - 词语搭配和双连词
        - 词长分布
1. [获取文本语料库][202]
    - 古腾堡语料库
    - 网络和聊天文本
    - 布朗语料库
    - 路透社语料库
    - 就职演说语料库
    - 其他语言的语料库
    - 文本语料库的结构
    - 载入你自己的语料库
        - txt文件载入
        - 载入宾州树库的副本
1. [条件频率分布][203]
    - 条件与事件
    - 按文体计数词汇
    - 绘制分布图和分布表
    - 使用Bigrams生成随机文本
1. [词典资源][204]
    - 词典资源
        - 词典(`Lexical`)或词典资源是一个词和/或短语及其相关信息的集合，例如：词性(`part-of-speech`)和词意(`sense`)定义等相关信息。
        - 词项(`lexical entry`)包括词目(`headword`)（也叫词条(`lemma`)）及其他附加信息，例如：词性和词意定义。
        - 词汇列表语料库
            - 停用词(`stopwords`)语料库
            - 名字语料库
        - 发音的词典
            - 美国英语的CMU发音词典
                - 音素(`phones`)
        - 比较词表
            - Swadesh wordlists
        - 词汇工具：Toolbox
    - WordNet
        - 意义与同义词(`synonyms`)
        - WordNet的层次结构
            - `unique beginners`
            - `hyponyms`
            - `hypernyms`
        - 更多的词汇关系
            - `Hypernyms` 和 `hyponyms` 被称为词汇关系(`lexical relations`)。
            - 蕴含(`entails`)
            - 反义词(`antonymy`)
        - 语义相似度
            - 如果两个同义词集共用一个特定的`hypernym`——在hypernym层次结构中处于较低层——它们一定有密切的联系。
            - 可以通过查找每个同义词集的深度来量化这个普遍性概念。
            - path_similarity基于hypernym层次结构概念中相互关联的最短路径下，在0~1范围内的相似度（两者之间没有路径返回-1）。同义词集与自身比较将返回1。
1. [处理原始文本][205]
    - 从网络和硬盘访问文本
        - 电子书
        - 处理HTML
        - 处理RSS订阅
        - 读取本地文件
        - NLP流程
    - 使用正则表达式
        - 提取字符块
        - 查找词干(`stems`)
        - 搜索已分词文本
    - 规范化(`Normalizing`)文本
        - 词干提取器(`Stemmers`)
        - 词形归并(`Lemmatization`)
        - 分割(`Segmentation`)
            - `Tokenization` is an instance of a more general problem of `segmentation`.
            - 将分词转换成搜索问题
                - 评估函数
                - 模拟退火
1. [分类和标注词汇][206]
    - 使用词性标注器(`part-of-speech tagger` 或 `POS tagger`)
    - 标注语料库
        - 读取已标注的语料库
        - 简化的词性标记集
        - 名词
        - 动词
        - 未简化的标记
        - 探索已标注的语料库
    - 自动标注
        - 默认标注器
        - 正则表达式标注器
        - 查询标注器
    - N-gram标注
        - 一元标注器(Unigram Tagging)
        - 分离训练和测试数据
        - 一般的N-gram的标注
        - 组合标注器
        - 标注生词
        - 存储标注器
        - 性能限制
        - 跨句子边界标注
    - 基于转换的标注(Transformation-Based Tagging)
    - 如何确定一个词的分类
        - 形态学(Morphological)线索
        - 句法(Syntactic)线索
        - 语义(Semantic)线索
        - 新词
        - 词性标注集中的形态学(Morphology in Part-of-Speech Tagsets)
1. [分类文本性别鉴定][207]
    - naive Bayes classifier
    - 似然比(`likelihood ratios`)
1. [分类文本电影评论正负面评价][208]
    - NaiveBayesClassifier
1. [分类文本词性标注][209]
    - 词性标注(`Part-of-Speech Tagging`)
    - 基于后缀
    - 探索上下文语境
    - 序列分类
        - 为了获取相关分类任务之间的依赖关系，我们可以使用`joint classifier`模型，为一些相关的输入选择适当的标签。
        - 在词性标注的例子中，可以使用各种不同的`sequence classifier`模型为给定的句子中的所有词选择词性标签。
        - 一种称为`consecutive classification`或`greedy sequence classification`的序列分类器策略，为第一个输入找到最有可能的类标签，然后在此基础上找到下一个输入的最佳的标签。这个过程可以不断重复直到所有的输入都被贴上标签。
    - 其他序列分类方法
        - 这种方法的缺点是一旦做出决定便无法更改。例如：如果决定将一个词标注为名词，但后来发现应该是动词，那也没有办法修复我们的错误了。解决这个问题的方法是采取转型策略(`transformational strategy`)。转型联合分类(`Transformational joint classifiers`)的工作原理是为输入的标签创建一个初始值，然后反复提炼该值，尝试修复相关输入之间的不一致。`Brill标注器`，是使用这种策略的。
        - 隐马尔可夫模型(`Hidden Markov Models`)采取了这种方法。
            - 最大熵隐马尔可夫模型(`Maximum Entropy Markov Models`)和线性链条件随机场模型(`Linear-Chain Conditional Random Field Models`)
1. [分类文本句子分割][210]
1. [识别对话行为类型][211]
1. [识别文字蕴含][212]
1. [决策树][213]
    - 熵(Entropy)和信息增益(Information Gain)
1. [朴素贝叶斯][214]
1. [最大熵][215]
1. [从文本提取信息][216]
    - 信息提取
        - 信息提取结构
    - 分块(Chunking)
        - 名词短语分块
        - 用正则表达式分块
        - 探索文本语料库
        - 缝隙(Chinking)
        - 分块的表示：标记与树状图
    - 开发和评估分块器
        - 读取IOB格式与CoNLL2000分块语料库
        - 简单评估和基准
        - 训练基于分类器的分块器
    - 语言结构中的递归
        - 用级联分块器构建嵌套结构
        - 树状图
    - 命名实体识别(Named Entity Recognition)
    - 关系抽取(Relation Extraction)
1. [分析句子结构][217]
    - 文法(Syntax)的用途
    - 上下文无关文法
    - 上下文无关文法分析(Parsing with Context-Free Grammar)
        - 递归下降解析器(Recursive Descent Parsing)
        - 移进-规约分析(Shift-Reduce Parsing)
    - 依存关系(Dependencies)和依存文法(Dependency Grammar)

[201]: nltk-introduction.ipynb
[202]: corpus.ipynb
[203]: conditional-frequency-distribution.ipynb
[204]: lexical.ipynb
[205]: handle-with-raw-text.ipynb
[206]: classify-and-pos-tagging.ipynb
[207]: classify_gender.ipynb
[208]: classify_movie_reviews.ipynb
[209]: classify_pos_tagging.ipynb
[210]: classify_sentence_segment.ipynb
[211]: recognizing-dialog-behaviour.ipynb
[212]: recognizing-textual-entailment.ipynb
[213]: decision-tree.ipynb
[214]: naive-bayes.ipynb
[215]: maximum-entropy.ipynb
[216]: extract-from-text.ipynb
[217]: sentence-structure.ipynb