---
title: CReST: A Class-Rebalancing Self-Training Framework for Imbalanced Semi-Supervised Learning
tags:
  - 论文总结
---

CReST: A Class-Rebalancing Self-Training Framework
for Imbalanced Semi-Supervised Learning
=======================================

## 类型

解决类不平衡

## 主要创新

提出了一个类再平衡自我训练框架（CReST），该框架利用而不是受制于模型的偏差来缓解少数类上的性能退化。
此外，扩展了分布式对齐，并将其整合为CReST+，以进一步提高在线伪标签的质量。

对自我训练进行了两个修改。首先，使用SSL算法在有标签和无标签的数据上训练，不仅仅是有标签的数据，以便获得更好的教师模型；通过选定一个子集来扩展标签集，一个类别的频率越低，被预测为类别的未标记样本就越多地被纳入伪标记集。

<img src="\assets\image\2022-11-10-0.png" style="zoom:100%;" />

## 不足

只讲了多数类少数类的类别不平衡，并没有正样本和负样本的不平衡