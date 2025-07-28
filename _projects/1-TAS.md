---
title: "基于模仿学习动作分块策略的时序动作选择器"
excerpt: "使用强化学习策略对目前模仿学习中常用的动作分块（action chunking）进行改进，实现响应实时性与长程规划能力的兼顾"
collection: projects
---
## 项目简介
动作分块策略有效地提高了神经网络对人类行为策略的建模能力，但决策频率的降低也带来了实时响应性能的下降。在高精度或是存在噪声与扰动的操作任务中，由于缺少对最新的环境观测的及时响应，往往带来明显的性能下降甚至直接导致任务失败。另一方面，在执行完整的动作块后，引入新的环境观测得到的动作很可能会导致机器人动作的不流畅，产生明显的周期性抖动。  
  
在本项研究中，我们提出了时序动作选择（TAS）算法，通过堆叠每一个时刻预测得到的动作块，获得k个待选动作，使用基于神经网络的选择器对待选动作进行自主选择，并使用强化学习算法在稀疏奖励环境中对选择器进行训练，使其自主习得期望奖励最大化的选择策略。此方法适用于任何使用动作分块机制的策略，且不会破坏基础策略的多模态输出，在不同任务、同一任务的不同阶段自主地取得响应实时性，长程规划能力的均衡，从而获得显著高于基础策略的性能。

<img src='/images/my/TAS.jpg' alt="Simulation Project" 
    style="max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 10px;">

* 在PushT（低维简单任务）、FurnitureBench（家具装配环境、高维长时序复杂任务）中复现经典和前沿模仿学习策略，如：BC（基于MLP）、CVAE（基于ACT修改）、Diffusion Policy、VQ-BeT、IBC。
* 在仿真环境中使用PPO算法基于稀疏奖励训练动作选择器策略，残差策略，动作选择残差策略，并进行性能对比。
* 实物实验：搭建Franka机械臂实物平台，基于FoundationPose实现FurnitureBench任务中待组装部件的位姿估计，对模仿学习策略、残差强化学习策略和时序动作选择器策略进行性能评估。

## 实验结果
**TAS性能提升**


**PushT任务对比**
<div style="display: flex; justify-content: space-between; gap: 20px; margin-bottom: 30px;">
  <div style="flex: 1;">
    <img src="/video/1step-animation.gif" alt="AH=1" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; margin-top: 8px;">AH=1(动作停滞)</p>
  </div>
  <div style="flex: 1;">
    <img src="/video/8step-animation.gif" alt="AH=8" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; margin-top: 8px;">AH=8(缺少实时反馈)</p>
  </div>
  <div style="flex: 1;">
    <img src="/video/selector-animation.gif" alt="TAS" style="width: 100%; border-radius: 8px;">
    <p style="text-align: center; margin-top: 8px;">TAS</p>
  </div>
</div>

**残差策略性能提升**
<img src="/images/W&B Chart.png" alt="残差策略性能对比" 
    style="max-width: 100%; height: auto; border-radius: 8px; margin: 20px 0;">


**FurnitureBench实物实验**  
残差策略
 <video width="720" controls>
  <source src="/video/franka2.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
  
残差策略+动作选择器
 <video width="720" controls>
  <source src="/video/franka1.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
 <video width="720" controls>
  <source src="/video/franka3.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
---
（待完善中...）