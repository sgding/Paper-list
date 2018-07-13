# End-to-end Multi-Modal Multi-Task Vehicle Control for Self-Driving Cars with Visual Perceptions
## 摘要
* 背景：之前的端到端的方法，以单幅图像或者图像序列为输入，利用CNN预测方向盘转角。虽然只预测方向盘转角的方法可以获得较好的效果，但是只有方向盘转角是不能满足车辆控制需求的。
* 方法：该论文提出一种多任务的学习框架，利用端到端的方案同时预测方向盘转角和速度控制。由于直接预测速度值非常困难，该论文首先提出使用网络，根据图像序列，预测离散的速度命令和方向盘转角。此外，改论文还提出一种多模态多任务的网络，以之前的速度反馈和视觉信息为输入。
> 注：其中多模态指的是不同类型的输入，这里是指速度反馈和视觉图像两种不同模态的输入。
* 实验：在Udacity数据集和新采集的SAIC数据集上进行了实验。

## 网络结构
### 方向盘转角模型

![](https://github.com/sgding/Paper-list/planning/end-to-end/pictures/steering-image.png) 
![baidu](http://www.baidu.com/img/bdlogo.gif)  
