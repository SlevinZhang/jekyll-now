---
layout: post
title: K-Nearest-Neighbor
---
### 向量模型  
用一个高维的特征向量来表示一个数据  
而这样的表示其实是对原始数据进行降维的结果  
也可以使用PCA来对特征向量进行降维  


### 向量距离  
1. 欧式距离
2. Cosine Similarity  

### 高维空间求最邻近  
1. Annoy 算法  
  * 构建一个二叉树，而结点划分的方式就是在平面随机挑选两个点，然后以垂直于这两个点的等距平面将集合划分成两部分  
  * 在相应的子树上迭代上述方法  
  * 直到每一个根结点只剩下K个点为止  
  * 求最邻近的k个点时候
    * 遍历二叉树，直到根结点，在每个节点处，到其子结点平面的距离会决定我们遍历的方向  
    * 使用优先队列， 如果子结点之间足够近（threshold），我们将同时搜寻两个子节点，要设置阈值来判断什么时候会搜寻两个子节点  
  * Link
    * [Annoy Github](https://github.com/spotify/annoy)
    * [Powerpoin](https://www.slideshare.net/erikbern/approximate-nearest-neighbor-methods-and-vector-models-nyc-ml-meetup)
    
2. 穷举搜索法  
  * 一对一对的比较，在比较对象太多的时候效率很低  
3. K-nn 方法  
  * 将搜索的特征空间聚类，每一类中包含K 个元素，然后计算所有类别的中心点  
  * 计算新得到的向量和中心点直接的距离，找到最近的点，然后返回该中心点所在类别中的所有元素  
  
  
