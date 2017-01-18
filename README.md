
# 东野圭吾小说分析
数据挖掘大作业, 文本数据挖掘
----------

## 实现的功能
- 提取小说中的关键属性(人名、地名、时间词、职业)
- 包含小说中出现的专业名词的精确分词
- 小说中关键属性的统计
- word2vec提取词向量进行相似分析



----------
## 运行环境与依赖库
- python3 (统一unicode编码中文)
- hanlp (专业汉语词汇分词含日本人名\中国人名等)
- jieba (专业中文分词)
- gensim (快速word2vec库)

----------
## 代码结构
- sp_words.py
利用hanlp进行分词，提取人名、地名、时间词、职业
- count_attrs.py
统计属性并写入专业词库
- resp_words.py
利用jieba导入专业词库后再次分词
- advance_analysis.py
利用gensim训练word2vec模型，进行相似分析
