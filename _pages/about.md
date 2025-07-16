---
permalink: /
title: "个人简介"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
---

**翁悦阳**，哈尔滨工业大学（深圳）控制科学与工程24级在读研究生（导师：[李衍杰教授](https://faculty.hitsz.edu.cn/liyanjie)）。

教育经历
--------
- **工学硕士 - 在读**  
  哈尔滨工业大学（深圳）  
  控制科学与工程（2024年9月 – 至今）  
  RLG实验室
  <!-- [RLG实验室](https://www.rlg-hitsz.net) -->

- **工学学士**  
  哈尔滨工业大学（深圳）  
  自动化（2020年9月 – 2024年6月）

研究方向
--------
基于强化学习和模仿学习的机器人操作算法。

项目经历
--------

<div style="display: flex; align-items: flex-start; text-decoration: none; margin-bottom: 10px;">
    <div style="display: flex; flex-direction: column;">
        <a href="/projects/1-TAS" style="font-size: 22px; font-weight: bold; text-decoration: none; color: #0073e6;">
            基于模仿学习动作分块策略的时序动作选择器
        </a>
        <p style="font-style: italic; color: #777; font-size: 16px; margin: 0 0 12px;">
            负责人 （2025年01月 - 至今）
        </p>
        <img src='/images/my/TAS.jpg' alt="Simulation Project" 
            style="max-width: 100%; height: auto; border-radius: 8px; margin-bottom: 10px;">
        <p style="margin: 5px 0 0; color: #555; font-size: 18px;">
            在本项研究中，我们提出了时序动作选择（TAS）算法，通过堆叠每一个时刻预测得到的动作块，获得k个待选动作，使用基于神经网络的选择器对待选动作进行自主选择，并使用强化学习算法在稀疏奖励环境中对选择器进行训练，使其自主习得期望奖励最大化的选择策略。此方法适用于任何使用动作分块机制的策略，且不会破坏基础策略的多模态输出，在不同任务、同一任务的不同阶段自主地取得响应实时性，长程规划能力的均衡，从而获得显著高于基础策略的性能。
        </p>
    </div>
</div>
---
<div style="display: flex; gap: 20px; margin-bottom: 20px;">
    <div style="flex: 1 0 200px;">
        <a href="/projects/2-GP" style="font-size: 22px; font-weight: bold; text-decoration: none; color: #0073e6; display: block; margin-bottom: 10px;">
            基于强化学习的机器人组装策略研究（本科毕业设计）
        </a>
        <p style="font-style: italic; color: #777; font-size: 16px; margin: 0 0 12px;">
            负责人 （2023年10月 - 2024年06月）
        </p>
        <img src='/images/my/GP.jpeg' alt="Smart Car Competition" 
             width="350" style="float: left; margin-right: 15px; border-radius: 8px;">
        <div style="overflow: hidden;">
            <p style="color: #555; font-size: 18px; line-height: 1.6; margin-bottom: 10px;">
                基于强化学习结合六轴力/力矩传感器信号提高机器人孔轴装配任务性能。
            </p>
            <p style="color: #555; font-size: 18px; line-height: 1.6; margin-bottom: 10px;">
                在Mujoco环境中搭建实验平台，设计奖励函数，使用PPO算法进行策略训练，与基于轨迹搜索的策略进行性能对比。 
            </p>
        </div>
    </div>
</div>
---
<div style="display: flex; gap: 20px; margin-bottom: 20px;">
    <div style="flex: 1 0 200px;">
        <a href="/projects/3-IMCC" style="font-size: 22px; font-weight: bold; text-decoration: none; color: #0073e6; display: block; margin-bottom: 10px;">
            第十六届全国大学生智能汽车竞赛-国家级一等奖
        </a>
        <p style="font-style: italic; color: #777; font-size: 16px; margin: 0 0 12px;">
            队长 （2020年12月 - 2021年08月）
        </p>
        <img src='/images/my/img01.jpg' alt="Smart Car Competition" 
             width="150" style="float: left; margin-right: 15px; border-radius: 8px;">
        <div style="overflow: hidden;">
            <p style="color: #555; font-size: 18px; line-height: 1.6; margin-bottom: 10px;">
                设计车模双核控制、通讯架构。完成车模循迹，特殊赛道元素识别，状态切换代码实现。运用微分跟踪器（TD）等进行车模速度信号，电磁信号滤波。使用PID、模糊PID等算法实现车模控制。
            </p>
            <p style="color: #555; font-size: 18px; line-height: 1.6;">
                结合神经网络对特征分类、端到端行为克隆控制方案进行探索与验证。
            </p>
        </div>
    </div>
</div>