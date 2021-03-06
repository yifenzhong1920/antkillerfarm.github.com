---
layout: post
title:  深度学习（二十九）——Graph NN（1）
category: DL 
---

* toc
{:toc}

# Graph NN

## GraphSAGE

GraphSAGE取自Graph SAmple and aggreGatE，SAmple指如何对邻居个数进行采样。aggreGatE指拿到邻居的embedding之后如何汇聚这些embedding以更新自己的embedding信息。

https://mp.weixin.qq.com/s/DNePTCpyjrlZEixw5L7w5A

GraphSAGE：我寻思GCN也没我牛逼

https://mp.weixin.qq.com/s/1DHvLLysMU24dBeLzbSpUA

GraphSAGE

https://mp.weixin.qq.com/s/IcLk-fMjKO19BaHbuUCeXg

GraphSAGE算法原理，实现和应用

https://zhuanlan.zhihu.com/p/142205899

GraphSAGE源码解析

https://mp.weixin.qq.com/s/45PlgqZag8dXqZr4xvj9Hw

GraphSAGE算法细节详解

## GAT

https://mp.weixin.qq.com/s/_aydey5ZVwrObmoFXXIYcw

Bengio等人提出图注意网络架构GAT，可处理复杂结构图

https://zhuanlan.zhihu.com/p/34232818

《Graph Attention Networks》阅读笔记

https://zhuanlan.zhihu.com/p/81350196

GAT（图注意力模型）

https://mp.weixin.qq.com/s/JlUqwie3BtOSIwgSKvRz4w

深入探讨图注意力模型：Graph Attention

https://zhuanlan.zhihu.com/p/132497231

深入理解图注意力机制

https://zhuanlan.zhihu.com/p/57168713

深入理解图注意力机制

https://mp.weixin.qq.com/s/7LfJ8wDr4K6cVunb8Q_83g

图注意力网络（GAT）详解

## DeepWalk

https://mp.weixin.qq.com/s/SXnRyUj_mMs8UEtNyP6qNw

DeepWalk论文解读

https://mp.weixin.qq.com/s/h1vDImYTLEheatZnScZwbg

使用DeepWalk从图中提取特征

https://mp.weixin.qq.com/s/F2jF1vuzK4u8ZPrDK_CyLw

KDD2018网络表示学习最新教程：DeepWalk作者Perozzi等人带你探索最前沿

https://mp.weixin.qq.com/s/QvPB3wNT3IeFuqLB8_nxsw

从Word2vec到DeepWalk

https://mp.weixin.qq.com/s/gsxE1V_fNTDjIMhs3ZW72Q

DeepWalk：图网络与NLP的巧妙融合

## 参考

https://github.com/thunlp/GNNPapers

清华NLP图神经网络GNN论文分门别类，16大应用200+篇论文

https://github.com/nnzhan/Awesome-Graph-Neural-Networks

图神经网络论文列表

https://github.com/DeepGraphLearning/LiteratureDL4Graph

图深度学习资源汇总

https://github.com/IndexFziQ/GNN4NLP-Papers

自然语言领域中图神经网络模型（GNN）应用现状（论文列表）

https://github.com/jdlc105/Must-read-papers-and-continuous-tracking-on-Graph-Neural-Network-GNN-progress

Papers on Graph neural network(GNN)

https://github.com/benedekrozemberczki/awesome-graph-classification

图网络大列表

https://mp.weixin.qq.com/s/SW6V-AxGq1z9Uq7qIJLj5A

Github上热门图深度学习（GraphDL）源码与工业级框架

http://www.p-chao.com/2019-01-20/%e5%9b%be%e7%a5%9e%e7%bb%8f%e7%bd%91%e7%bb%9cgnn/

图神经网络GNN的简单理解

https://mp.weixin.qq.com/s/_TAhfkjj1wsWEZDT8q5K8Q

图表示学习极简教程

https://github.com/icoxfog417/graph-convolution-nlp

图卷积神经网络自然语言处理应用代码和教程

https://mp.weixin.qq.com/s/VEAnkznZUyZ1RCJulSnwGg

基于图结构网络的表征学习

https://mp.weixin.qq.com/s/rxZQrhvRk6Dw3AWpGJS4dg

《基于图的句子意思表征》教程, 300多页PPT带你进入这一新兴领域

https://mp.weixin.qq.com/s/w5ldyp00CqkX8Kp-8Aw0nQ

图深度学习(GraphDL)，下一个人工智能算法热点？一文了解最新GDL相关文章

https://mp.weixin.qq.com/s/Jt6CjMqNFEXWoL5pkLeVyw

洛桑理工：Graph上的深度学习报告

https://mp.weixin.qq.com/s/eelcT5x_kWC0dDt0_Ph4qg

清华朱文武组一文综述GraphDL五类模型

https://mp.weixin.qq.com/s/0rs8Wur7Iv6jSpFz5C-KNg

来自IEEE Fellow的GNN综述

https://mp.weixin.qq.com/s/cdbHoR_E_mpIdcvmNGWfDA

掌握图神经网络GNN基本，看这篇文章就够了

https://www.cnblogs.com/SivilTaram/p/graph_neural_network_1.html

从图(Graph)到图卷积(Graph Convolution)：漫谈图神经网络模型 (一)

https://www.cnblogs.com/SivilTaram/p/graph_neural_network_2.html

从图(Graph)到图卷积(Graph Convolution)：漫谈图神经网络模型 (二)

https://www.cnblogs.com/SivilTaram/p/graph_neural_network_3.html

从图(Graph)到图卷积(Graph Convolution)：漫谈图神经网络模型 (三)

https://mp.weixin.qq.com/s/Irs_fLrf4oybc3sAfpmEeA

图嵌入（Graph embedding）综述

https://mp.weixin.qq.com/s/hyW3b7o4kRZN0oflMLYlTw

图嵌入概述

https://mp.weixin.qq.com/s/4YlDC24vC-H7PHRZhhiZJg

图节点嵌入(Node Embeddings)概述，9页pdf

https://mp.weixin.qq.com/s/s6E2vV1KrQDI4SeAnkYTKw

图神经网络将成AI下一拐点！MIT斯坦福一文综述GNN到底有多强

https://mp.weixin.qq.com/s/5oOobY_3blbXYYxuuQmShQ

一文读懂图神经网络

https://mp.weixin.qq.com/s/U51C2t92nlE7Tv7oKXgx2A

一份完全解读：是什么使神经网络变成图神经网络？

https://mp.weixin.qq.com/s/vK0bzljCNdR1OumUmsi2sA

斯坦福大牛Jure Leskovec：图神经网络研究最新进展

https://mp.weixin.qq.com/s/WMpcamrHjUDnYwqyISdooA

斯坦福Jure Leskovec图表示学习：无监督和有监督方法

https://mp.weixin.qq.com/s/8zhO5phIVc2gz70omn9xKA

Jure Leskovec：图神经网络GNN研究进展：表达性、预训练、OGB，71页ppt

https://mp.weixin.qq.com/s/lt9lZbulkW0C8A_xi6hodQ

浅析图卷积神经网络

https://mp.weixin.qq.com/s/aeQyZ8cpz81cK8Dg-84mjA

网络表征学习综述

https://mp.weixin.qq.com/s/bsNDI9YxFdaB2Q5aRz9ECw

图卷积神经网络的变种与挑战

https://mp.weixin.qq.com/s/oKwxWbCkH-xqYSJIBdb92A

2018超网络节点表示学习

https://mp.weixin.qq.com/s/WQlSghxG89JCroNZSmop8w

朱军：关于图的表达学习

https://mp.weixin.qq.com/s/mTCrTPzyeogwRHfgitfK6Q

为什么说图网络是AI的未来？

https://mp.weixin.qq.com/s/DUv5c6ce-dgLOBAE4ChiQg

图神经网络为何如此强大？看完这份斯坦福31页PPT就懂了！

https://mp.weixin.qq.com/s/OV-rXGU8DTNqv3QZcKo00Q

Graph Learning

https://mp.weixin.qq.com/s/PkUJsnZdihPM7q9BpvO8Ag

深度学习中不得不学的Graph Embedding方法

https://mp.weixin.qq.com/s/PxNGJ0hcmCo-2zvWD-rfug

GCN作者Thomas Kipf最新Talk：利用图神经网络进行无监督学习

https://mp.weixin.qq.com/s/t2kjxrcn6O9tbJ-IQELboQ

高君宇：图神经网络在视频分类中的应用

https://mp.weixin.qq.com/s/SWcJut6QqOvbziirxTd2Kg

斯坦福教授ICLR演讲：图网络最新进展GraphRNN和GCPN

https://mp.weixin.qq.com/s/Lakq83_ngUJf1ES3N7J9_g

图卷积在基于骨架的动作识别中的应用

https://mp.weixin.qq.com/s/5wSgC4pXBfRLoCX-73DLnw

什么是图卷积网络？行为识别领域新星

https://mp.weixin.qq.com/s/1-Dmckby2NcXsaoK08zk8w

视频理解中的图表示学习

https://mp.weixin.qq.com/s/sJB4N_ObUqKM8H65yU_1sg

Graph基础知识介绍

https://mp.weixin.qq.com/s/edrh-HXqW01Yx7c8tQ8UxA

从数据结构到算法：图网络方法初探

https://mp.weixin.qq.com/s/JvtrGa0YiUmR6UA5wBQ-pQ

图神经网络GNN最新理论进展和应用探索

https://mp.weixin.qq.com/s/zQU47tjpTCPiLdEmUmZx3Q

图卷积神经网络及其应用

https://mp.weixin.qq.com/s/8Sz_jo7pokL_nzupEBGGdg

当深度强化学习遇见图神经网络

https://zhuanlan.zhihu.com/p/28170197

《Gated Graph Sequence Neural Networks》阅读笔记

https://blog.csdn.net/yorkhunter/article/details/104056795

综述论文“A Comprehensive Survey on Graph Neural Networks”

https://mp.weixin.qq.com/s/rTnv7XOnIvRDGDdhbuoE9g

深度图相似学习综述

https://mp.weixin.qq.com/s/FDWoAXGOlRxOEkvli3gd5Q

55页图深度学习导论《A Gentle Introduction to Deep Learning for Graphs》

https://mp.weixin.qq.com/s/Pm1HiEQOBnbo_GQ_v6Y_zw

腾讯提出自适应图卷积神经网络，接受不同图结构和规模的数据

https://zhuanlan.zhihu.com/p/31067515

《Semi-Supervised Classification with Graph Convolutional Networks》阅读笔记

https://mp.weixin.qq.com/s/6viSk0Ts_7eTfYrWYi_HDQ

基于图结构的实体和关系联合抽取模型简介

https://zhuanlan.zhihu.com/p/36117802

《Learn to Represent Programs with Graphs》阅读笔记。这篇论文讲述了DL在程序代码纠错方面的应用。

https://zhuanlan.zhihu.com/p/37278426

Graph2Seq: Graph to Sequence Learning with Attention-based Neural Networks

https://mp.weixin.qq.com/s/iQYVyo2PHuGbEsYgdIf_oQ

DeepMind等机构提出“图网络”：面向关系推理

https://mp.weixin.qq.com/s/TAccHagxXQ82lfE91Y6xWg

CNN已老，GNN来了：重磅论文讲述深度学习的因果推理

https://mp.weixin.qq.com/s/UONtTJJgDawRPWtatAVKkg

如何利用高效的搜索算法来搜索网络的拓扑结构

https://mp.weixin.qq.com/s/SGCtwYWfnxjcpMJeeH1b4w

图神经网络+池化模块，斯坦福等提出层级图表征学习

https://mp.weixin.qq.com/s/DOau_vTbwCauQ8mrHkGu9Q

首个面向Facebook、arXiv网络图类的对抗攻击研究

https://mp.weixin.qq.com/s/_0quf0IRe8mn4dnsBwf6Aw

基于路径的实体图关系抽取模型

https://mp.weixin.qq.com/s/jCgbBldpw4TGHUvN9WkJZg

在对抗中学习网络结构——87页PPT带你学习Graph中的GAN

https://mp.weixin.qq.com/s/xTZbfiLYHB64AJJRcw04qQ

知识图和神经网络：如何有效读取图节点属性

https://mp.weixin.qq.com/s/9fFjVSiMg-LwddXfNJuKuw

DeepMind开源图网络库，一种结合图和神经网络的新方法

https://mp.weixin.qq.com/s/5DmpgPN4t3p3H53Xu7_-3A

北大、微软亚洲研究院：高效的大规模图神经网络计算

https://mp.weixin.qq.com/s/BFJD8i_yg1Y6fxZS5or-rw

Bengio最新论文提出GibbsNet：深度图模型中的迭代性对抗推断

https://mp.weixin.qq.com/s/zg3yW7e4UKIs9-m6WmcbvA

GraphWave：一种全新的无监督网络嵌入方法

https://mp.weixin.qq.com/s/mamet6l_lA7fhoYkysZ7PQ

华为联合LSE提出KONG：有序近邻图的核函数

https://mp.weixin.qq.com/s/OnRB44tliuTFcjlmuRG3Xw

图神经网络“理论在哪里“？

https://mp.weixin.qq.com/s/Uy2ekBiwkI2sIo637b-16g

北大、微软提出NGra：高效大规模图神经网络计算

https://mp.weixin.qq.com/s/diIzbc0tpCW4xhbIQu8mCw

阿里凑单算法首次公开！基于Graph Embedding的打包购商品挖掘系统解析

https://mp.weixin.qq.com/s/chiHw5gKnJyTJTQeF6gViw

在向量空间中启用网络分析和推理，清华大学崔鹏博士最新分享

https://mp.weixin.qq.com/s/kQlxLDHLI6xxFzwJVjFj7w

GraRep: 基于全局结构信息的图结点表示学习

https://mp.weixin.qq.com/s/aGP8pcsCmEdjdCWVjA82Jg

近期必读的5篇CVPR 2019图卷积网络相关论文和代码

https://mp.weixin.qq.com/s/XApSbi-Pg-AeYGkPN3fldg

旷视研究院提出ML-GCN：基于图卷积网络的多标签图像识别模型

https://mp.weixin.qq.com/s/49vnVOO0G_JvKrWcsN2_Ww

关系图注意力网络-Relational Graph Attention Networks

https://mp.weixin.qq.com/s/rvcj9-6KlBsVmF_CAsip2A

超越标准GNN！DeepMind、谷歌提出图匹配网络

https://mp.weixin.qq.com/s/UotqgRjCTpjPrsIEWBRPxA

基于随机游走的图匹配算法

https://mp.weixin.qq.com/s/dDaFhssFEYxS7ElMy4ekJw

基于图嵌入的深度图匹配

https://mp.weixin.qq.com/s/LZvxvDpxQEtlKuXoxT_gTQ

可变形曲面跟踪，亮风台新出基于图匹配的方法

https://mp.weixin.qq.com/s/7DyPJ9LnqZ9XyAop33SxSw

ST-GCN动作识别算法详解

https://mp.weixin.qq.com/s/fxVsN2dDmayxJfxBRIXHhQ

解读PingSage：图卷积神经网络在数十亿数据网络级别推荐系统的应用
