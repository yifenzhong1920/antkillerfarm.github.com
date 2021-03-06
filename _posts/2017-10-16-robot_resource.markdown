---
layout: post
title:  机器人/无人驾驶参考资源（一）
category: resource 
---

* toc
{:toc}

# 机器人/无人驾驶参考资源

由于已经有了强化学习系列blog和资源，因此本资源中不再包含强化学习的内容。但毫无疑问，强化学习才是这方面的主角。

此外，SLAM、Apollo、传感器（主要是传感器的物理原理，不包括传感器数据的融合处理。）系列也有单独的资源，这里不再列出。

## 前言

2004年，DARPA举办了第一届 “DARPA”挑战赛（无人车挑战赛）。根本没有一支参赛队伍完成这次比赛任务，这件事对来自斯坦福大学的Sebastian Thrun刺激很大。

于是，他在2005年组建了自己的无人车队，并且成为这项挑战赛上的第一支完赛队伍，获得奖金200万美元。这笔奖金虽然巨额，但事实上Sebastian Thrun在这个项目的投入远远大于200万美金。

Sebastian团队另外一大贡献就是在完成挑战赛后，发表了一篇著名的paper：

《Stanley: The Robot that Won the DARPA Grand Challenge》

## 行业

![](/images/img2/ADAS.jpg)

https://mp.weixin.qq.com/s/Okolok3ZLZhgw0TQ_TROKA

一文看尽国内智能驾驶格局：三条技术路线和玩家鏖战2020年

https://mp.weixin.qq.com/s/Jz-VqWCyNc6nUi-2PuB8rg

中美“军用无人机”发展情况及其制造商

https://mp.weixin.qq.com/s/oi5ME4QRTt3U526lzAHTcA

滴滴重磅发布：KDD2018大会187页人工智能+交通教程

https://mp.weixin.qq.com/s/BUwu6R83klL3E5tI7TEX9A

一文带你看懂自动驾驶

https://mp.weixin.qq.com/s/4PPiwJJWPi4qn5mBwX6wDw

ADAS处理器、芯片主流企业及相应技术梳理

https://mp.weixin.qq.com/s/y0HnpWRUBLyEyqzWfOhkCw

博世集团百年启示录

Never forget your humanity, and respect human dignity in your dealings with others.---Robert Bosch

https://mp.weixin.qq.com/s/GtAZa5veVKFpQdJgdlMDBg

你不一定知道的博世！

https://mp.weixin.qq.com/s/xgxsmcMAqstzmhTJZFZIyw

特斯拉重磅深度：T E S L A，T-S.E.X.Y

https://mp.weixin.qq.com/s/uei9W13lOp_bbcobv4VvlQ

一张版图带你摸清全球10大自动驾驶联盟布局

https://mp.weixin.qq.com/s/fG_Oee0biudXyX-B-93THw

史上最全的自动驾驶研究报告（上）

https://mp.weixin.qq.com/s/Qe6ex06SFbI1ggq9ONZYFA

史上最全的自动驾驶研究报告（下）

https://mp.weixin.qq.com/s/iQ9vnGX7TjtMP_UOmvVjlA

特斯拉深度研究报告

https://mp.weixin.qq.com/s?__biz=MzI1ODYwOTkzNg==&mid=2247497740&idx=3&sn=eedfb5f889b80fde545d89f5fb29238d

中国汽车工业沉浮70年

https://mp.weixin.qq.com/s/myAUMq4hknEcZ7X2Xx455g

万字长文回顾智能驾驶进化史

## 课程

http://selfdrivingcars.mit.edu/

MIT 6.S094: Deep Learning for Self-Driving Cars

>主讲：Lex Fridman，MIT博士后。   
>个人主页：   
>http://lexfridman.com/

这个课程不仅提供了课件，还提供了DeepTraffic和DeepTesla两个小工具供学生验证自己的算法。

参考：

https://mp.weixin.qq.com/s/cPyWAD-t-qLHfZJT1To2wQ

自动驾驶“老司机”拼车技，MIT的这个比赛已经飙到了时速123公里

这两个工具是用ConvNetJS编写的。

ConvNetJS是Andrej Karpathy编写的基于JavaScript的DL框架。

官网：

http://cs.stanford.edu/people/karpathy/convnetjs/

代码：

https://github.com/karpathy/convnetjs

参考：

https://mp.weixin.qq.com/s/9jS7T51kMDhmzaOp9SI0oA

从Brain.js到Mind，一文收录11个移动端Javascript机器学习库

----

http://www.eecs.wsu.edu/~taylorm/16_483F/index.html

CptS 483: Introduction to Robotics

http://www.eecs.wsu.edu/~taylorm/2011_cs420/index.html

CS 420：Artificial Intelligence

http://ctms.engin.umich.edu/CTMS/index.php

这个网页提供了很多机械的控制算法——从系统、控制到仿真的全过程的教程。

https://github.com/Microsoft/AutonomousDrivingCookbook/tree/master/AirSimE2EDeepLearning

这是微软提供的自动驾驶课程

https://www.doc.ic.ac.uk/~ajd/Robotics/index.html

CS 333: Robotics

https://mp.weixin.qq.com/s/T7wI4cjKbciYC3ZNxKfReA

143页 MIT自动驾驶算法地图推理教程

http://abcinstitute.baidu.com/pages/index.html#/specialInfo?specialId=4008

百度的自动驾驶课程

https://mp.weixin.qq.com/s/O-xV6fXtSnF0Y8Z2lxKa1g

自主机器人导论:运动学，感知，定位和规划，241页pdf

## 自动驾驶入门课程

https://mp.weixin.qq.com/s/yO_Lc5Fo-8fBC9PwVCQBqA

自动驾驶入门课程第①讲 — 无人驾驶概览

https://mp.weixin.qq.com/s/IVD0aq8V-qZoB0tcLMigYw

自动驾驶入门课程第②讲 — 高精地图

https://mp.weixin.qq.com/s/KJbm4wfsTLxT5LGR7GV_SA

自动驾驶入门课程第③讲 — 定位

https://mp.weixin.qq.com/s/BCNrsuoThJt031jCnbAjAA

自动驾驶入门课程第④讲 — 感知（上）

https://mp.weixin.qq.com/s/FqW2X9LJZvNe9efllAYhTQ

自动驾驶入门课程第⑤讲 — 感知（下）

https://mp.weixin.qq.com/s/6ro9y69h-6yHZ7MfodxUHQ

自动驾驶入门课程第⑥讲 — 预测

https://mp.weixin.qq.com/s/ZBHKDtnaEI9sVCfEfeeUlQ

自动驾驶入门课程第⑦讲 — 规划（上）

https://mp.weixin.qq.com/s/1yA-kgS_rL4o9I4OWeI4-A

自动驾驶入门课程第⑧讲 — 规划（下）

https://mp.weixin.qq.com/s/8hLVHuv635fyHRNftXJQ4w

自动驾驶入门课程第⑨讲 — 控制（上）

https://mp.weixin.qq.com/s/AnWWnD3ScSW6GhrwRGpRDw

自动驾驶入门课程第⑩讲 — 控制（下）

![](/images/img3/autonomous_driving.png)

## 术语

LIDAR：LIght Detection And Ranging

LDW：Lane Departure Warning System，车道偏离警告系统

LKS：lane keeping system，车道保持系统

LKA：Lane Keeping Assist，车道保持辅助

LCA：lane centering assist

FCW：Forward Collision Warning，前向碰撞预警

AEB：Automatic emergency braking，自动紧急刹车

V2X：vehicle to everything

TMC：Traffic Message Channel，实时交通系统

ISA：Intelligent Speed Adaptation，电子警察系统

VCS：Vehicular Communication Systems，车联网系统

VD：Vihicle Detection，车辆检测

ACC：Adaptive Cruise Control，自适应巡航控制

HMW：Headway Monitoring & Warning，车距检测及警告

CAS：Collision Avoidance System，碰撞避免或预碰撞系统

PED：Pedestrian Detection，行人检测

TSR：Traffic Sign Recognition，道路交通标志识别系统

TLR：Traffic Light Recognition，交通信号灯识别系统

Night Vision，夜视系统

Adaptivelight Control，自适应灯光控制

Pedestrian Protection System，行人保护系统

Automatic Parking，自动泊车

Blind Spot Detection，盲点探测

Driver Drowsiness Detection，驾驶员疲劳探测

Hill Descentcontrol，下坡控制系统

Electric Vehicle Warningsounds，电动汽车报警

Surround View Monitor，全景影像系统

Intelligent Headlight Control，远光自动控制

Augmented Reality Navigation，增强现实导航

High Beam Assist，远近光灯辅助系统

参考：

https://mp.weixin.qq.com/s/ZEtLAj_K_BYU1jtU8LivJA

汽车ABS、EBD、ESP、TCS、HDC、HHC、这些英文都有什么用处？

## blog

http://www.cnblogs.com/yhlx125/

一个Robot+GIS的blog

https://www.cnblogs.com/21207-iHome/

一个Robot方面比较全面的blog

http://vision.ia.ac.cn/

中国科学院自动化研究所模式识别国家重点实验室机器视觉课题组，主要研究领域包括场景三维重建、视觉定位与姿态估计、机器人视觉导航、视觉伺服、目标检测与跟踪等。

http://blog.exbot.net/

一个机器人技术方面的网站。

https://blog.csdn.net/yuxuan20062007/

一个无人驾驶的blog

https://blog.csdn.net/AdamShan

一个无人驾驶的blog

## ROS

http://www.ros.org/

ROS(Robot Operating System）是一个机器人软件平台，前身是斯坦福人工智能实验室为了支持斯坦福智能机器人STAIR而建立的项目。

https://mp.weixin.qq.com/s/Rmvksy54iKgcyd7bqy_oxQ

机器人开源操作系统ROS入门

https://zhuanlan.zhihu.com/p/51353579

Matlab/Simulink与ROS的通讯

https://mp.weixin.qq.com/s/lUhLd8HXz_HG_mCnDwURNg

ROS概述

https://mp.weixin.qq.com/s/zGIHo97bFii1_z8u9_QiUA

ROS原理—1

https://mp.weixin.qq.com/s/EQGI0l_Zw08QsbU22w4IDg

ROS原理—2

https://mp.weixin.qq.com/s/VHtv4yEx77TbZRh2sMhLRw

ROS原理—3

https://mp.weixin.qq.com/s/bZqsV0tbnyf9to5jD0OlLg

ROS原理—4

https://mp.weixin.qq.com/s/Yzt8L-p_aN-Ukm_DdcBn1w

ROS深入介绍

https://mp.weixin.qq.com/s/7tffKpKWqFYNcOmHJ7T3Zw

汽车操作系统的前世今生

https://mp.weixin.qq.com/s/ALTjs2vvHtZs5RJe-k0ECQ

自动驾驶中的机器人操作系统ROS

https://mp.weixin.qq.com/s/IBY2RMSEXde5uZpuRi3cuA

ROS概述与环境搭建

https://mp.weixin.qq.com/s/eyqyaOFenPGA721cMGAC0Q

ROS通信机制

https://mp.weixin.qq.com/s/Sd6rfFAcoP86m98W3wSJkg

ROS通信机制进阶

https://mp.weixin.qq.com/s/3CYZidjGtJtjB5pgjSWfAA

ROS运行管理

https://mp.weixin.qq.com/s/46GnLJw6hciXrkgNLvF12w

ROS常用组件

## PythonRobotics

PythonRobotics是一个机器人算法方面的代码示例库。

官网：

https://atsushisakai.github.io/PythonRobotics/

## OpenDRIVE

OpenDRIVE是一种用于导航和自动驾驶的数据格式。

官网：

http://opendrive.org/

参考：

http://blog.csdn.net/lewif/article/details/78575840

OpenDrive格式地图数据解析

## ArUco

ArUco是一个开源的微型的现实增强库，可用于视觉定位。

官网：

http://www.uco.es/investiga/grupos/ava/node/26

参考：

https://blog.csdn.net/lixujie666/article/details/80246909

基于ArUco的视觉定位

https://blog.csdn.net/Shawn_Zhangguang/article/details/78737686

ArUco--一个微型现实增强库的介绍及视觉应用

## AUTOSAR

AUTOSAR是AUTOmotive Open System Architecture（汽车开放系统架构）的首字母缩写，由汽车制造商，供应商以及工具开发商联合开发的一个开放的、标准化的软件架构。

参考：

https://zhuanlan.zhihu.com/p/41602815

AUTOSAR概述 & 基于AUTOSAR的时间同步

https://zhuanlan.zhihu.com/p/57459276

软件架构--基于AUTOSAR的多模块任务分配策略

## openpilot

openpilot是一个开源的自动驾驶（驾驶代理）。

官网：

https://github.com/commaai/openpilot

## CAN

https://mp.weixin.qq.com/s/8jZKgSeRw7k0F9JOigFJcw

自动驾驶之——CAN总线简介

https://mp.weixin.qq.com/s/U-Nzj3NM3acjkprVuyComg

汽车CAN总线技术详解

https://mp.weixin.qq.com/s/yDQ4zQpo4BVrnnnV_J6dlg

一文看懂四大汽车总线：LIN、CAN、FlexRay、MOST

https://mp.weixin.qq.com/s/u6gibvshU4KI3fEE6h9KeQ

上海大众内训资料：CAN总线讲解

https://mp.weixin.qq.com/s/tjn6Fob1L9aWnl2b35rjgA

一文读懂总线技术

https://mp.weixin.qq.com/s/d35w8Gs0Zzf1yHPkXFv9iQ

CAN总线必看经典

https://mp.weixin.qq.com/s/K-EqcqX8X7oeNA2czT2qIA

高手写的CAN总线入门总结

https://mp.weixin.qq.com/s/5ZfFcbnhkpyO-CdXyw6SKw

一文详解LIN总线

https://mp.weixin.qq.com/s/hxH-e6qz13Cr4kBqjTmVRw

CAN总线的特点和帧结构

https://mp.weixin.qq.com/s/FmdRkyQm0P-N_bCjMEPLbA

CAN协议标准及相关内容
