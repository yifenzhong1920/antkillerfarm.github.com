---
layout: post
title:  TensorFlow（三）
category: AI 
---

* toc
{:toc}

# TensorFlow

## TensorFlow Serving（续）

参考：

https://zhuanlan.zhihu.com/p/23361413

TensorFlow Serving尝尝鲜

http://www.cnblogs.com/xuchenCN/p/5888638.html

tensorflow serving

https://mp.weixin.qq.com/s/iqvpX6QuBEmF_UK9RMu9eQ

TensorFlow Serving入门

https://mp.weixin.qq.com/s/TL87BY3DdP1bolc0Sxkahg

gRPC客户端创建和调用原理解析

https://zhuanlan.zhihu.com/p/30628048

远程通信协议：从CORBA到gRPC

https://mp.weixin.qq.com/s/b569est_LpcxsoTNWXcfog

TensorFlow Extended帮你快速落地项目

https://mp.weixin.qq.com/s/qOy9fR8Zd3SufvsMmLpoGg

使用TensorFlow Serving优化TensorFlow模型

https://mp.weixin.qq.com/s/IPwOZKvDsONegyIuwkG6bQ

将深度学习模型部署为web应用有多难？答案自己找

https://mp.weixin.qq.com/s/7nugWFKtD-C6cpwm2TyvdQ

手把手教你如何部署深度学习模型

https://zhuanlan.zhihu.com/p/77664408

如何解决推荐系统工程难题——深度学习推荐模型线上serving？

https://mp.weixin.qq.com/s/vqFRbsM9DGu8ikJ3VNp_-g

TensorFlow Extended(TFX)：面向生产环境的机器学习

http://mp.weixin.qq.com/s/hpv6bzr-5VZet-UCHOCQLQ

谷歌TFX：基于TensorFlow可大规模扩展的机器学习平台

https://mp.weixin.qq.com/s/ANoY3MZEvz7SvKXDE-24NQ

迈向ML工程：TensorFlow Extended(TFX)简史

https://mp.weixin.qq.com/s/DkCGusznH8F8p39oRLuNBQ

TensorFlow Serving模型更新毛刺的完全优化实践

## op的C++实现

有的时候为了将Tensorflow的op移植到其他平台，需要找到相应op的cpu实现。比如space_to_batch这个op，它的实现在：

core/kernels/spacetobatch_op.cc

简单的op一般找到这里就可以了，但space_to_batch还要更深一层：

core/kernels/spacetobatch_functor.cc

一般XXX_impl.cc或者XXX_functor.cc才是op实现真正所在的位置。

此外，TFlite的实现往往更加简单：

tensorflow/contrib/lite/kernels/internal/reference/reference_ops.h

## TensorFlow.js

https://mp.weixin.qq.com/s/dqMS4NjmNYs7IFHm8uFM8w

TensorFlow发布面向JavaScript开发者的机器学习框架TensorFlow.js

https://zhuanlan.zhihu.com/p/35181413

TensorFlow.js人脸识别—玩转吃豆豆小游戏

https://mp.weixin.qq.com/s/ebLHZAG8H78TsZUKSzAtIw

TF官方博客：基于TensorFlow.js框架的浏览器实时姿态估计

https://mp.weixin.qq.com/s/z6p4A4DfCuK8IBGVGwrtLQ

如何利用TensorFlow.js部署简单的AI版“你画我猜”图像识别应用

https://mp.weixin.qq.com/s/NO_XY-JmTpIkoC-fpkZ-qg

在浏览器上也能训练神经网络？TensorFlow.js带你玩游戏~

https://mp.weixin.qq.com/s/vjpMr3TsF3Lui8Q0IstQxw

浏览器上跑：TensorFlow发布实时人物分割模型，秒速25帧，24个部位

https://mp.weixin.qq.com/s/-BblgnvPLuqpYM8PZ7PQCQ

三行代码实时追踪你的手，只要有浏览器就够了

https://mp.weixin.qq.com/s/C7QdVathJ8YTXF-zXPC-Ow

有人分析了7个基于JS语言的DL框架，发现还有很长的路要走

## Eager Execution

TensorFlow的Eager Execution可立即评估操作，无需构建图：操作会返回具体的值，而不是构建以后再运行的计算图。这也就是所谓的动态图计算的概念。

参考：

https://mp.weixin.qq.com/s/Yp2zE85VCx8q67YXvuw5qw

TensorFlow引入了动态图机制Eager Execution

https://github.com/ZhuanZhiCode/TensorFlow-Eager-Execution-Examples

Eager Execution的代码示例

https://github.com/madalinabuzau/tensorflow-eager-tutorials

TensorFlow的动态图工具Eager怎么用？这是一篇极简教程

https://mp.weixin.qq.com/s/Lvd4NfLg0Lzivb4BingV7w

Tensorflow Eager Execution入门指南

https://github.com/snowkylin/TensorFlow-cn

简单粗暴TensorFlow Eager教程

https://github.com/snowkylin/tensorflow-handbook

简单粗暴TensorFlow 2.0

https://mp.weixin.qq.com/s/zz8XCykJ6jxbE5J4YwAkEA

一招教你使用tf.keras和eager execution解决复杂问题

## Estimator

![](/images/img2/tensorflow_programming_environment.png)

Estimator是一个非常高级的API，其抽象等级甚至在Keras之上。

Estimator主要包括以下部分：

1.初始化。定义网络结构。

2.train。

3.evaluate。

4.predict。

TensorFlow已经包含了一些预置的Estimator。例如：BoostedTreesClassifier、DNNClassifier、LinearClassifier等。具体可参见：

https://tensorflow.google.cn/api_docs/python/tf/estimator

参考：

https://mp.weixin.qq.com/s/a68brFJthczgwiFoUBh30A

TensorFlow数据集和估算器介绍

https://mp.weixin.qq.com/s/zpEVU1E5DfElAnFqHCqHOw

训练效率低？GPU利用率上不去？快来看看别人家的tricks吧～

## tf.data

tf.data提供了一套构建灵活高效的输入流水线的API。

![](/images/img2/datasets_without_pipelining.png)

![](/images/img2/datasets_with_pipelining.png)

上面两幅图中，第一幅图是没有使用流水线的情况，而第二幅图则是使用流水线的情况。

参考：

https://mp.weixin.qq.com/s/dfXTV4PFgC1Wbti42Zf4wQ

tf.data API，让你轻松处理数据

https://mp.weixin.qq.com/s/mjUnrPBPBuY6XKXkUymX-w

实例介绍TensorFlow的输入流水线

https://mp.weixin.qq.com/s/1ZlyVDJK6RWZ_1Ox7399IA

用一行tf.data实现数据Shuffle、Batch划分、异步预加载等

## TensorFlow Probability

TensorFlow Probability是一个概率编程工具包。

官网：

https://tensorflow.google.cn/probability/

参考：

https://mp.weixin.qq.com/s/NPuYanaUnaX4mYbaNbNNSQ

概率编程工具：TensorFlow Probability官方简介

https://mp.weixin.qq.com/s/cV-5W4YWC9f9wsoNX5fIXA

使用TensorFlow Probability对金融模型中的误差进行介绍性分析

https://mp.weixin.qq.com/s/cxC3SarlBBPTwIxQZ4AG_g

快速上手TensorFlow Probability内置概率编程教材

https://mp.weixin.qq.com/s/T0TsS8YwyCbCjt4J-xonOw

使用TensorFlow Probability Layers的变分自编码器

https://mp.weixin.qq.com/s/6l-NS0NbYK44JS0jnRl82w

使用TensorFlow Probability的概率层执行回归

https://mp.weixin.qq.com/s/2cbd7LBPBRqGt-QO1A7SfQ

在TensorFlow Probability中对结构时间序列建模

## TensorFlow Federated

TFF是一个开源框架，用于试验针对分散式数据的机器学习和其他计算。它采用的是一种名为联合学习(FL)的方法，许多参与的客户端能够训练共享的ML模型，同时将数据保存在本地。

这个项目感觉上和Leela Zero有些相似。

从原理上说，TFF主要使用了Federated Machine Learning技术。

参考：

https://mp.weixin.qq.com/s/K2-i3U-BCOctetMkvuvVxg

TensorFlow Federated发布

https://mp.weixin.qq.com/s/6QKyE3jIOwBK_2rcG-Vtiw

联邦机器学习-概念与应用

## TensorNetwork

TensorFlow的计算图模型不仅可以用于DL领域，亦可应用于其他科学计算领域。TensorNetwork就是一个基于TensorFlow的张量运算库。现成的矩阵运算库已经很多了，这次升级为张量运算库了。

https://github.com/google/TensorNetwork

参考：

https://mp.weixin.qq.com/s/jdjX0jirTHOUqsGagJmGLQ

谷歌AI开源张量计算库TensorNetwork，计算速度暴涨100倍

## Tensorflow 2.x

![](/images/img3/TF.png)

![](/images/img3/TF_2.png)

```python
import tensorflow
main_version = tensorflow.__version__.split('.')[0]
if int(main_version) == 2:
    import tensorflow.compat.v1 as tf
    tf.compat.v1.disable_v2_behavior()
    import tensorflow.compat.v1.lite as tflite
else:
    import tensorflow as tf
    import tensorflow.contrib.lite as tflite
```

https://mp.weixin.qq.com/s/BD-nJSZJLjBBq1n7HEHpKw

将您的代码升级至TensorFlow 2.0

https://mp.weixin.qq.com/s/xgsUF97aI1YfGSdh0FJ6Cw

都在关心TensorFlow 2.0，那我手里基于1.x构建的程序怎么办？

https://mp.weixin.qq.com/s/s8hAYadCw9-_BpWSCh38gg

TensorFlow 2.0：数据读取与使用方式

https://mp.weixin.qq.com/s/rVSC1AXj9YECjUrl5PkSGw

详解深度强化学习展现TensorFlow 2.0新特性

https://mp.weixin.qq.com/s/8D8kxFSfruwWhU2jmYL3sg

Google大佬Josh Gordon发布Tensorflow 2.0入门教程

https://cloud.tencent.com/developer/article/1498043

有了TensorFlow2.0，我手里的1.x程序怎么办？

https://mp.weixin.qq.com/s/ddHKc5AffznRaEY_qhHN_g

升级到tensorflow2.0，我整个人都不好了

https://mp.weixin.qq.com/s/RcolwQnCqrAsGaKEK0oo_A

TensorFlow 2.0中的tf.keras和Keras有何区别？为什么以后一定要用tf.keras？

## 细节

执行`session.run(out)`，会在终端打印out的值，但执行`res = session.run(out)`则不会。

此外，`session.run`可以接受list作为参数。返回值也是一个list，分别对应输入list的每个元素的计算结果。

----

tensorflow的程序中,在main函数下,都是使用tf.app.run()来启动。查看源码可知,该函数是用来处理flag解析，然后执行main函数。

https://blog.csdn.net/lujiandong1/article/details/53262612

tensorflow中的tf.app.run()

----

TF提供了一套专门的IO函数：tf.gfile。主要优点在于：对于写文件来说，open操作直到真的需要写的时候才执行。

----

迁移学习的时候，有的时候需要保持某几层的权值，在后续训练中不被改变。这时，可以在创建Variable时，令trainable=false。

----

sparse_softmax_cross_entropy_with_logits和softmax_cross_entropy_with_logits的区别在于：后者的label是一个one hot的tensor，而前者label直接用对应分类的index表示就行了。

----

CNN中的padding：

"SAME" = with zero padding。

"VALID" = without padding。

----

op的自定义实现可使用`tf.py_func`。

----

tf.dtypes.cast: 类型转换

----

由源代码可以知道`optimizer.minimize`实际上包含了两个步骤，即`compute_gradients`和`apply_gradients`，前者用于计算梯度，后者用于使用计算得到的梯度来更新对应的variable。

如果想要部分更新某个Variable的话，可用如下步骤：

1.生成需要更新的元素的mask tensor。1代表要更新，0代表不更新。

2.`compute_gradients`得到grad tensor。

3.`grad = grad * mask`

4.`apply_gradients`。

通常来说，如果一个计算图中没有optimizer，则一般只包含forward运算，而没有backward运算。

## blog

http://www.jianshu.com/u/eaec1fc422e9

一个TF的blog

http://blog.csdn.net/u012436149

一个TensorFlow+PyTorch的blog

## Hama

TensorFlow实际上是Google开发的第二代DL框架。在它之前，Google内部还有一个叫做DistBelief的框架。这个框架没有开源，但是有论文发表。因此，就有了一个叫做Apache Hama的项目，作为它的开源实现。

官网：

https://hama.apache.org/

这个项目采用了一种叫做Bulk Synchronous Parallel的并行计算模型。
