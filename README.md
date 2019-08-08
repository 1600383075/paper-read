#论文信息    
论文题目‘DILOF：EFFective and Memory Efficient Local Outlier Detection in Data Streams’    
论文作者：Gyoung S.Na,Donghyun Kim,Hwanjo Yu    
来源：KDD2018   
     
     
#相关介绍    
在流数据异常检测领域，有三大类异常检测方法：   
1、 distribution-based：这类方法目的是研究基于流数据的概率模型，但是这种模型需要太多的先验知识，如分布性等，而现实情况中是无法转却知道一种数据的分布特征的，最常见的假设都是基于数据分布为正态分布，而这种假设会严重造成异常数据精测精度的降低。   
2、 Clustering-based:构建集群来为底层数据分布建模。然后，根据算法，形成小簇的数据点或远离簇形中心的数据点被认为是离群点。然而，设计这种算法的主要目的是建立一个聚类模型，而不是检测离群值，这种算法通常对异常单点效果较好，在异常情况复杂的数据点效果一般。   
3、Distance-based:通过计算一个点相对于数据集中其他点的距离来检测异常值,在不知道数据分布或者数据特征情况都了解不足的情况下可以选择这种方法，因此，基于距离的方法在近些年使用最为广泛。
还有一些利用RNN、一维CNN、DNN等方法检测异常数据的方法，属于极少数，暂不做解释。   
    
      
#论文核心剖析   
一、论文核心架构    
    论文中算法名称为Density summarizing incremental LOF(DILOF)
