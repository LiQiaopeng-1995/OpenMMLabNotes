# OpenMMLab-AI训练营-2

图像分类与 MMClassification

## 1. 图像分类

### 任务目标: 给定一张图片, 识别图像中的物体是什么.  

### 数学表示: 

图像是像素构成的HWC数组, 输出类别为y∈{1, ..., K}的向量.  
构建出一个可计算实现的函数F: R^HxWxC^->{1, ..., K}, 且预测结果符合人类认知.

### 难点:

基于规则的机器学习:
1. 收集数据;
2. 定义模型:
通常为含参变量的函数: y = F~θ~(X)
1. 训练:
寻找最佳参数θ*, 使得模型y = F~θ*~(X)在训练集上达到最佳正确率;
1. 预测:
对于新图像X', 使用训练好的模型来预测其类别, y' = F~θ*~(X').

机器学习的局限:  
机器学习善于处理低维, 分布相对简单的数据; 而图像数据在极高维的空间以复杂的方式"纠缠"在一起, 机器学习难以处理复杂数据分布.  

传统方法: 手动设计图像特征;  
特征学习: 学习如何产生适合分类的特征, 多个简单特征变换复合构成一个复杂的端到端分类器;  

### 基于模型的图像分类

1. 模型设计: 设计适合图像的F~θ~(X).
   1. 卷积神经网络;
   2. 轻量化卷积神经网络;
   3. 神经结构搜索;
   4. Transformer;
2. 模型学习: 求解一组好的参数~θ~.
   1. 监督学习: 基于标注数据学习
      1. 损失函数;
      2. 随机梯度下降算法;
      3. 视觉模型常用训练技巧
   2. 自监督学习: 基于无标注的数据学习.