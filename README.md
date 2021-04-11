## 机器
GeForce RTX 280  


## 环境
python 3.6.12  
pytorch 1.6.0  
tqdm  
sklearn  
tensorboardX


## 中文数据集
ChineseNlpCorpus中属于情感/观点/评论倾向性分析的微博评论数据集weibo_senti_100k
该数据集包含119988条带情感标注的新浪微博评论数据，其中正向评论占59993条，负向评论占59995条

类别：negitive，positive

数据集划分：

数据集|数据量
--|--
训练集|95990
验证集|11999
测试集|11999


## 效果

模型|acc|备注
--|--|--
BiLSTM_Att|97.93%|BiLSTM+Attention
TextRCNN|97.59%|BiLSTM+池化
FastText|97.65%|bow+bigram+trigram

 
# 训练并测试：
# BiLSTM_Att,TextRCNN,FastText
python run.py --model BiLSTM_Att


### 参数
模型都在models目录下，超参定义和模型定义在同一文件中。  
  


