---
title: "基于强化学习的机器人组装策略研究（本科毕业设计）"
excerpt: "基于强化学习结合六轴力/力矩传感器信号提高机器人孔轴装配任务性能"
collection: projects
---
## 项目简介
孔轴装配是现代工业生产中重要的一环，由于精度要求较高，装配部件刚度大，纯视觉的装配策略往往无法满足要求。通过在机械臂末端增加六维力/力矩传感器，可以获得孔轴之间的接触信息，并使用强化学习训练装配策略，有效提升了机器人孔轴装配任务性能。
* 对基于等距螺旋线的传统搜孔策略进行改进，在CoppeliaSim和Mujoco环境中进行了实验验证。
* 在Mujoco环境中搭建实验平台，设计奖励函数，使用PPO算法进行策略训练，与基于轨迹搜索的策略进行性能对比。 
 <video width="600" controls>
  <source src="/video/PPO1.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
在未经训练的情况下在其他形状的孔轴装配任务中进行泛化能力测试。
 <video width="500" controls>
  <source src="/video/PPO2.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
 <video width="500" controls>
  <source src="/video/PPO3.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
