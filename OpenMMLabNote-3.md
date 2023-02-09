# OpenMMLab-AI训练营-3

图像分类代码实战

## 1. MMClassification介绍

MMClassification是OpenMMLab里专门针对图像分类做的一个代码库。  
Github仓库: <https://github.com/open-mmlab/mmclassification>  
文档教程: <https://mmclassification.readthedocs.io/zh_CN/latest/index.html>  

首先演示了Pytorch原生进行模型训练的代码， 然后介绍了MMClassification进行模型训练的流程。  
MMClassification以配置文件为核心：

1. 集成了各种各样的模型，如第2讲介绍的VGG，ResNet等等，支持很多数据集；
2. 可以调整优化器策略，学习率策略，数据增强策略；
3. 提供大量应用的工具以及预训练的模型；
4. 进行一体化训练，也可以剥离相关的模块整合进自己的代码；

## 2. 超算平台介绍

这块已经有文档进行相关的介绍了，不做赘述。
<https://aicarrier.feishu.cn/docx/QMRzd0NoxokuKvxNfS3car1EnHh>