<div align="center">
  <img src="assets/embodied-rsi-banner.svg" width="100%" alt="Awesome Embodied RSI 横幅">
  <br><br>
  <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <img src="https://img.shields.io/badge/%E7%AD%9B%E9%80%89-%E4%BA%BA%E5%B7%A5%E5%AE%A1%E6%A0%B8-2ea44f?style=flat-square" alt="人工审核">
  <img src="https://img.shields.io/badge/%E6%9B%B4%E6%96%B0-%E6%AF%8F%E5%91%A8-6366f1?style=flat-square" alt="每周更新">
  <img src="https://img.shields.io/badge/RSI-L0%20%E2%86%92%20L4-f97316?style=flat-square" alt="RSI L0 到 L4">
  <a href="LICENSE"><img src="https://img.shields.io/badge/%E8%AE%B8%E5%8F%AF%E8%AF%81-MIT-0ea5e9?style=flat-square" alt="MIT 许可证"></a>
  <br><br>
  <strong>系统梳理具身智能体如何从经验中持续改进，<br>并进一步改进其“自我改进能力”。</strong>
  <br><br>
  <a href="README.md">English</a> · <a href="docs/TAXONOMY.zh-CN.md">分类体系</a> · <a href="CONTRIBUTING.zh-CN.md">贡献指南</a>
</div>

<br>

<table>
  <tr>
    <td align="center" width="20%"><a href="#overview"><b>🧭 项目概览</b></a><br><sub>定义与范围</sub></td>
    <td align="center" width="20%"><a href="#highlights"><b>🔥 每周精选</b></a><br><sub>近期重点条目</sub></td>
    <td align="center" width="20%"><a href="#research"><b>🧠 学术研究</b></a><br><sub>研究版图</sub></td>
    <td align="center" width="20%"><a href="#resources"><b>🧪 资源索引</b></a><br><sub>基准与综述</sub></td>
    <td align="center" width="20%"><a href="#contributing"><b>🤝 参与贡献</b></a><br><sub>推荐新资源</sub></td>
  </tr>
</table>

<p align="center"><b>33</b> 项研究 &nbsp;·&nbsp; <b>2</b> 条产业动态 &nbsp;·&nbsp; <b>1</b> 个基准 &nbsp;·&nbsp; <b>2</b> 篇综述</p>

<a id="overview"></a>

## 🧭 什么是 Embodied RSI？

具身递归式自我改进研究能够通过物理或模拟环境中的交互经验，对模型、策略、记忆、技能、Harness 或具身形态产生持久改进的智能体；在更高阶段，改进还会增强系统下一轮自我改进的能力。

<p align="center"><code>获取经验 → 自我评估 → 持久更新 → 重新部署 ↺</code></p>

## 🧩 范围、分类与 RSI 等级

| 等级 | 阶段 | 发生了什么变化？ | 在本列表中的定位 |
|:---:|---|---|---|
| `L0` | **Embodied** | 能感知和行动，但没有持久改进 | 背景 |
| `L1` | **Adaptive** | 任务内适应、反思或重新规划 | 相关工作 |
| `L2` | **Self-Improving** | 利用自身经验产生持久变化 | **核心** |
| `L3` | **Recursive** | 改进能够强化后续改进循环的组件 | **核心 RSI** |
| `L4` | **Open-Ended** | 自主生成目标并持续积累、扩展能力 | 前沿 |

核心列表优先收录 L2–L4；L0–L1 只在构成重要基础或基准时收录。

<a id="highlights"></a>

## 🔥 每周精选

<!-- WEEKLY_HIGHLIGHTS -->
- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.11350)<br>
  <sub><b>作者:</b> Peidong Wang, Zhiming Ma, Ying Chang, Xufang Luo, Xiaocui Yang, Shi Feng, Yuqing Yang, Dongsheng Li</sub><br>
  SHAPER 保持模型参数冻结，利用目标环境中的执行轨迹进化可复用技能以及具身智能体外围的上下文代码 Harness。Simulation, no real machine.
- **ETA: A New Agentic Paradigm for Embodied Tasks** (2026-08-04) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.03924) · [Project](https://openmoss.ai/OpenETA/) · [Code](https://github.com/OpenMOSS/OpenETA)<br>
  <sub><b>作者:</b> Yitong Chen, Zezheng Huai, Sixian Li, Yubang Wang, Haozhe Zhang, Yifei Zhang, Hechang Chen, Jingjing Gong, Yu-Gang Jiang, Xipeng Qiu</sub><br>
  ETA 以 Planner—Interface—World 循环组织具身任务，验证执行结果并将交互转化为可复用经验；OpenETA 以可替换规划器、工具、技能、记忆和可回放轨迹实现该范式。
- **You Don't Need To Stay in The Loop: An Agentic Robotics Loop for Robot-Policy Improvement** (2026-08-02) · *arXiv preprint* · `L3 Recursive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.07555)<br>
  <sub><b>作者:</b> Hang Yu</sub><br>
  AgenticRobotics 将训练—评估—改进组织为持久、证据门控的事务，并加入基于提交的恢复、工具质量测量与可审计晋级，使机器人策略改进循环无需操作者持续值守。
- **Exploratory, Communicative, and Deployable: Vision-Driven Embodied Agents for Open-World Mobile Manipulation** (2026-07-15) · *ECCV 2026* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.13653) · [Project](https://internrobotics.github.io/REAL/) · [Code](https://github.com/InternRobotics/REAL)<br>
  <sub><b>作者:</b> Boyu Mi, Mengchen Ma, Yifei Yao, Xing Gao, Junting Chen, Yangzi Li, Zihou Zhu, Guohao Li, Zhenfei Yin, Tai Wang, Yao Mu, Jiangmiao Pang, Hanqing Wang</sub><br>
  REAL 通过仿真—真机一致的接口结合主动探索、交互式意图消歧、监督微调与在线强化学习，并将所得智能体迁移到真实双臂移动机器人。
- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) · `L1 Adaptive` `news`. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)<br>
  NVIDIA 的 GR00T 开发平台将模拟、遥操作、策略训练、评估和部署连接为完整的人形机器人工作流，并同步发布 GR00T 1.7 模型。

<a id="research"></a>

## 🧠 学术研究

| 研究方向 | 收录范围与主要分类标准 |
|---|---|
| [基础与定义](#foundations-definitions) | 收录概念、定义、边界与理论；当工作主要贡献是构建 Embodied RSI 的问题框架时归入此类。 |
| [目标与课程生成](#goal-curriculum-generation) | 收录目标、任务、奖励、实验或课程的自主生成；依据什么机制驱动智能体选择下一学习目标进行分类。 |
| [自主经验获取](#autonomous-experience-acquisition) | 收录交互经验的自主采集、生成与筛选；依据智能体如何获得自身改进所需数据进行分类。 |
| [自我评估与反馈](#self-evaluation-feedback) | 收录评价器、奖励、验证器、反思与结果诊断；依据系统如何衡量表现并产生反馈进行分类。 |
| **[自我改进机制](#self-improvement-mechanisms)** | 按持久变化的主要改进对象分类：模型或策略、记忆、技能、Harness 或具身形态。 |
| [模型与策略](#model-policy) | 收录模型、策略或世界模型的持久更新；当主要改进对象是学习参数或决策规则时归入此类。 |
| [记忆与知识](#memory-knowledge) | 收录所学知识的持久存储、修订、巩固与检索；依据智能体记住并复用的内容如何变化进行分类。 |
| [技能与行为](#skills-behaviors) | 收录技能或行为的获取、精炼、组合与复用；依据智能体可执行能力库的变化进行分类。 |
| [Harness 与系统](#harness-system) | 收录可变的中间件、工具、上下文、编排与运行时基础设施；当改进对象是智能体外部系统时归入此类。 |
| [具身适应](#embodiment) | 收录形态、传感器、执行器或控制接口的适应；依据智能体物理形态或具身耦合的持久变化进行分类。 |
| [终身与集体进化](#lifelong-collective-evolution) | 收录跨时间、任务、机器人或智能体的能力积累；依据长期保持、迁移、群体学习或集体进化进行分类。 |
| [安全与对齐](#safety-alignment) | 收录面向可变具身系统的约束、监督、审计、回滚与恢复；依据如何使自我改进保持可控和对齐进行分类。 |

<a id="foundations-definitions"></a>

### 🧱 基础与定义

_收录概念、定义、边界与理论；当工作主要贡献是构建 Embodied RSI 的问题框架时归入此类。_

- **Intelligent Robot Manipulation Requires Self-Directed Learning** (2026-03-04) · *OpenReview preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://openreview.net/forum?id=5IpSR7v4gj)<br>
  <sub><b>作者:</b> Li Chen, Chonghao Sima, Kashyap Chitta, Antonio Loquercio, Ping Luo, Yi Ma, Hongyang Li</sub><br>
  这篇观点论文认为，智能操作应超越模仿学习，转向通过真实环境交互和自身经验进行自导向学习。该范式面临两个区别于传统强化学习的核心挑战：真实世界通常不可逆且无法重置，反馈信号也往往含噪、模糊而缺少明确奖励；未来应重点研究自主目标识别、技能习得和效果评估。
- **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents** (2025-05-29) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2505.22954) · [Project](https://sakana.ai/dgm/) · [Code](https://github.com/jennyzzt/dgm)<br>
  <sub><b>作者:</b> Jenny Zhang, Shengran Hu, Cong Lu, Robert Lange, Jeff Clune</sub><br>
  Darwin Gödel Machine 迭代修改并实证评估自身编码智能体代码库，同时维护已发现变体的档案以支持开放式探索。

<a id="goal-curriculum-generation"></a>

### 🎯 目标与课程生成

_收录目标、任务、奖励、实验或课程的自主生成；依据什么机制驱动智能体选择下一学习目标进行分类。_

- **Playful Agentic Robot Learning** (2026-06-17) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.19419) · [Project](https://playful-rats.github.io/) · [Code](https://github.com/Playful-RATs/RATs)<br>
  <sub><b>作者:</b> Junyi Zhang, Jiaxin Ge, Hanjun Yoo, Letian Fu, Zihan Yang, Yaowei Liu, Raj Saravanan, Shaofeng Yin, Justin Yu, Dantong Niu, Zirui Wang, Roei Herzig, Ken Goldberg, Yutong Bai, David M. Chan, Ion Stoica, Angjoo Kanazawa, Jiahui Lei, Haiwen Feng, Trevor Darrell</sub><br>
  RATs 通过自主玩耍提出可学习的操作任务，执行并诊断代码策略，再将成功尝试提炼为持久技能库，并迁移到后续仿真与真实机器人任务。
- **OMNI-EPIC: Open-endedness via Models of human Notions of Interestingness with Environments Programmed in Code** (2024-05-24) · *NeurIPS 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2405.15568) · [Project](https://omni-epic.vercel.app/)<br>
  <sub><b>作者:</b> Maxence Faldor, Jenny Zhang, Antoine Cully, Jeff Clune</sub><br>
  OMNI-EPIC 利用基础模型，根据智能体当前学习进展持续生成可学习且有趣的模拟任务、环境和奖励。

<a id="autonomous-experience-acquisition"></a>

### 🔄 自主经验获取

_收录交互经验的自主采集、生成与筛选；依据智能体如何获得自身改进所需数据进行分类。_

- **Exploratory, Communicative, and Deployable: Vision-Driven Embodied Agents for Open-World Mobile Manipulation** (2026-07-15) · *ECCV 2026* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.13653) · [Project](https://internrobotics.github.io/REAL/) · [Code](https://github.com/InternRobotics/REAL)<br>
  <sub><b>作者:</b> Boyu Mi, Mengchen Ma, Yifei Yao, Xing Gao, Junting Chen, Yangzi Li, Zihou Zhu, Guohao Li, Zhenfei Yin, Tai Wang, Yao Mu, Jiangmiao Pang, Hanqing Wang</sub><br>
  REAL 通过仿真—真机一致的接口结合主动探索、交互式意图消歧、监督微调与在线强化学习，并将所得智能体迁移到真实双臂移动机器人。
- **Autonomous Improvement of Instruction Following Skills via Foundation Models** (2024-07-30) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2407.20635)<br>
  <sub><b>作者:</b> Zhiyuan Zhou, Pranav Atreya, Abraham Lee, Homer Walke, Oier Mees, Sergey Levine</sub><br>
  该方法利用视觉语言模型自主采集并评估有意义的真实机器人经验，随后在无需人工标注的情况下改进指令跟随策略。整个系统提出一个端到端的自我改进循环：VLM 观察当前环境图像并提出任务，随后由机器人执行、进行成功检测与自我标注、后见重标并更新参数；其中后见重标可以复用失败数据。

<a id="self-evaluation-feedback"></a>

### 🪞 自我评估与反馈

_收录评价器、奖励、验证器、反思与结果诊断；依据系统如何衡量表现并产生反馈进行分类。_

- **A Closed-Loop Multi-Agent Framework for Robust Multi-Robot Manipulation** (2026-07-08) · *RSS 2026* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2607.06990)<br>
  <sub><b>作者:</b> Yi-Xiang He, Lan Wei, Haoming Cen, Jian-Jian Jiang, Zhuohao Li, Guanxing Lu, Yihan Yang, Dandan Zhang, Wei-Shi Zheng</sub><br>
  该框架由规划智能体分配子任务、各机器人操作智能体调用自适应工具，并由验证智能体监控物理结果、返回语义纠正，从而闭合多机器人操作循环。
- **From Reaction to Anticipation: Proactive Failure Recovery through Agentic Task Graph for Robotic Manipulation** (2026-05-12) · *RSS 2026* · `L1 Adaptive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.11951) · [Project](https://shengxu.net/AgentChord/) · [Code](https://github.com/EDEM-AI/AgentChord)<br>
  <sub><b>作者:</b> Sheng Xu, Ruixing Jin, Huayi Zhou, Bo Yue, Guanren Qiao, Yunxin Tai, Yueci Deng, Kui Jia, Guiliang Liu</sub><br>
  AgentChord 在执行前构建任务图并加入预判的情境化恢复分支，使低延迟监视器能够直接触发纠正行为，而无需等待完整的重新规划。
- **MindPower: Enabling Theory-of-Mind Reasoning in VLM-based Embodied Agents** (2025-11-28) · *CVPR 2026* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2511.23055)<br>
  <sub><b>作者:</b> Ruoxuan Zhang, Qiyun Zheng, Zhiyu Zhou, Ziqi Liao, Siyu Wu, Jian-Yu Jiang-Lin, Bin Wen, Hongxia Xie, Jianlong Fu, Wen-Huang Cheng</sub><br>
  MindPower 加入面向机器人自身及人类信念、欲望与意图的心智理论推理，并以 Mind-Reward 优化推理链和生成动作之间的一致性。
- **RFTF: Reinforcement Fine-tuning for Vision-language-action Models with Temporal Feedback** (2025-09-19) · *OpenReview preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://openreview.net/forum?id=v8fZ1PbV4D)<br>
  <sub><b>作者:</b> Junyang Shu, Zhiwei Lin, Yongtao Wang</sub><br>
  RFTF 利用时序信息训练价值模型，为 VLA 策略的强化微调提供稠密反馈，并报告了在 CALVIN 上的快速任务适应能力。

<a id="self-improvement-mechanisms"></a>

### ♻️ 自我改进机制

_本组按照发生持久变化、并能在后续任务中继续使用的系统组件进行分类。_

<a id="model-policy"></a>

#### 🧠 模型与策略

_收录模型、策略或世界模型的持久更新；当主要改进对象是学习参数或决策规则时归入此类。_

- **Self-Improving Loops for Visual Robotic Planning** (2026-05-27) · *OpenReview preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://openreview.net/forum?id=HK9OWSMgoq)<br>
  <sub><b>作者:</b> Calvin Luo, Zilai Zeng, Mingxi Jia, Yilun Du, Chen Sun</sub><br>
  SILVR 使用自主产生的轨迹反复更新视觉规划模型(即视频生成模型)，并在未见过的模拟任务和真实机械臂操作上持续提升。
- **RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks** (2026-03-12) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2603.11558) · [Project](https://roboclaw-agibot.github.io/) · [Code](https://github.com/RoboClaw-Robotics/RoboClaw)<br>
  <sub><b>作者:</b> Ruiying Li, Yunlang Zhou, YuYao Zhu, Kylin Chen, Jingyuan Wang, Sukai Wang, Kongtao Hu, Minhui Yu, Bowen Jiang, Zhan Su, Jiayao Ma, Xin He, Yongjian Shen, Yang Yang, Guanghui Ren, Maoqing Yao, Wenhao Wang, Yao Mu</sub><br>
  RoboClaw 在同一 VLM 控制器下统一数据采集、策略学习与部署，并通过成对的正向和逆向行为实现自复位的在策略采集及真实机器人上的迭代策略改进。
- **VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model** (2026-02-12) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2602.12063) · [Project](https://sites.google.com/view/vla-w)<br>
  <sub><b>作者:</b> Yanjiang Guo, Tony Lee, Lucy Xiaoyang Shi, Jianyu Chen, Percy Liang, Chelsea Finn</sub><br>
  VLAW 交替使用真实机器人 Rollout 改进动作条件视频世界模型，再用该世界模型生成的合成 Rollout 改进 VLA 策略。
- **π*0.6: a VLA That Learns From Experience** (2025-11-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2511.14759) · [Official](https://www.pi.website/blog/pistar06)<br>
  <sub><b>作者:</b> Physical Intelligence, Ali Amin, Raichelle Aniceto, Ashwin Balakrishna, Kevin Black, Ken Conley, Grace Connors, James Darpinian, Karan Dhabalia, Jared DiCarlo, Danny Driess, Michael Equi, Adnan Esmail, Yunhao Fang, Chelsea Finn, Catherine Glossop, Thomas Godden, Ivan Goryachev, Lachy Groom, Hunter Hancock, Karol Hausman, Gashon Hussein, Brian Ichter, Szymon Jakubczak, Rowan Jen, Tim Jones, Ben Katz, Liyiming Ke, Chandra Kuchi, Marinda Lamb, Devin LeBlanc, Sergey Levine, Adrian Li-Bell, Yao Lu, Vishnu Mano, Mohith Mothukuri, Suraj Nair, Karl Pertsch, Allen Z. Ren, Charvi Sharma, Lucy Xiaoyang Shi, Laura Smith, Jost Tobias Springenberg, Kyle Stachowicz, Will Stoeckle, Alex Swerdlow, James Tanner, Marcel Torne, Quan Vuong, Anna Walling, Haohuan Wang, Blake Williams, Sukwon Yoo, Lili Yu, Ury Zhilinsky, Zhiyuan Zhou</sub><br>
  RECAP 通过多轮真实机器人执行、奖励反馈与纠正性干预，持续改进模型在长时程操作任务上的表现。它将“示范→纠错→练习”的三阶段学习过程工程化，结合离线 RL 预训练与在线 RL 微调、稀疏奖励与人类远程纠偏，并从失败数据中学习。
- **Self-Improving Embodied Foundation Models** (2025-09-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2509.15155) · [Project](https://self-improving-efms.github.io/)<br>
  <sub><b>作者:</b> Seyed Kamyar Seyed Ghasemipour, Ayzaan Wahid, Jonathan Tompson, Pannag Sanketi, Igor Mordatch</sub><br>
  该两阶段后训练方案从预训练具身基础模型中提取奖励(预测还需多少步到目标作为reward，基础模型自己派生奖励，不需要手工奖励工程)与成功检测能力，使机器人集群能够自主练习并获得新技能。
- **RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation** (2023-06-20) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2306.11706) · [Official](https://deepmind.google/blog/robocat-a-self-improving-robotic-agent)<br>
  <sub><b>作者:</b> Konstantinos Bousmalis, Giulia Vezzani, Dushyant Rao, Coline Devin, Alex X. Lee, Maria Bauza, Todor Davchev, Yuxiang Zhou, Agrim Gupta, Akhil Raju, Antoine Laurens, Claudio Fantacci, Valentin Dalibard, Martina Zambelli, Murilo Martins, Rugile Pevceviciute, Michiel Blokzijl, Misha Denil, Nathan Batchelor, Thomas Lampe, Emilio Parisotto, Konrad Żołna, Scott Reed, Sergio Gómez Colmenarejo, Jon Scholz, Abbas Abdolmaleki, Oliver Groth, Jean-Baptiste Regli, Oleg Sushkov, Tom Rothörl, José Enrique Chen, Yusuf Aytar, Dave Barker, Joy Ortiz, Martin Riedmiller, Jost Tobias Springenberg, Raia Hadsell, Francesco Nori, Nicolas Heess</sub><br>
  RoboCat 能适应新的机械臂与任务，自主生成额外练习轨迹，并将这些数据纳入后续通用模型训练。
- **Self-Improving Robots: End-to-End Autonomous Visuomotor Reinforcement Learning** (2023-03-02) · *CoRL 2023* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2303.01488) · [Project](https://architsharma97.github.io/self-improving-robots/)<br>
  <sub><b>作者:</b> Archit Sharma, Ahmed M. Ahmed, Rehaan Ahmad, Chelsea Finn</sub><br>
  MEDAL++ 通过同时学习任务执行与环境复位，让真实机器人自主练习操作任务，并在极少持续监督下显著超过行为克隆。

<a id="memory-knowledge"></a>

#### 🗃️ 记忆与知识

_收录所学知识的持久存储、修订、巩固与检索；依据智能体记住并复用的内容如何变化进行分类。_

- **When Robots Do the Chores: A Benchmark and Agent for Long-Horizon Household Task Execution** (2026-05-14) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.14504)<br>
  <sub><b>作者:</b> Zilin Zhu, Longteng Guo, Yanghong Mei, Bowen Pang, Zongxun Zhang, Xingjian He, Ruyi Ji, Jing Liu</sub><br>
  LongAct 以自由形式的家务任务评估规划层自主性；HoloMind 则结合 DAG 规划器、多模态空间记忆、情景经验复用和全局 Critic 进行反思式监督。
- **ABot-Claw: A Foundation for Persistent, Cooperative, and Self-Evolving Robotic Agents** (2026-04-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2604.10096) · [Code](https://github.com/amap-cvlab/ABot-Claw)<br>
  <sub><b>作者:</b> Dongjie Huo, Haoyun Liu, Guoqing Liu, Dekang Qi, Zhiming Sun, Maoguo Gao, Jianxin He, Yandan Yang, Xinyuan Chang, Feng Xiong, Xing Wei, Zhiheng Ma, Mu Xu</sub><br>
  ABot-Claw 为智能体运行时加入能力驱动的多机器人调度、跨具身多模态记忆和基于 Critic 的反馈，以在真实环境中进行在线进度评估、纠错与重新规划。

<a id="skills-behaviors"></a>

#### 🧰 技能与行为

_收录技能或行为的获取、精炼、组合与复用；依据智能体可执行能力库的变化进行分类。_

- **EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents** (2026-05-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.10332)<br>
  <sub><b>作者:</b> Ruofei Ju, Xinrui Wang, Xin Ding, Yifan Yang, Hao Wu, Shiqi Jiang, Qianxi Zhang, Hao Wen, Xiangyu Li, Weijun Wang, Kun Li, Yunxin Liu, Haipeng Dai, Wei Wang, Ting Cao</sub><br>
  EmbodiSkill 通过轨迹反思区分技能指导缺陷与执行失误，并围绕冻结模型持续修订可复用的程序性技能。Simulation, no real machine
- **Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models** (2024-06-26) · *ICRA 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2406.18746) · [Project](https://gtziafas.github.io/LRLL_project)<br>
  <sub><b>作者:</b> Georgios Tziafas, Hamidreza Kasaei</sub><br>
  LRLL 通过自主提出任务、在记忆中保存经验并将成功经验提炼为可复用skill策略，持续扩展可组合的机器人技能库。LRLL 不做梯度更新，目标就是把'固定技能库 + 手工提示'的范式，升级成一个会自己长大、自己总结技能的终身学习循环，整个学习过程靠LLM写代码 + 记忆检索 + 经验蒸馏来完成。
- **Voyager: An Open-Ended Embodied Agent with Large Language Models** (2023-05-25) · *TMLR 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2305.16291) · [Project](https://voyager.minedojo.org/)<br>
  <sub><b>作者:</b> Guanzhi Wang, Yuqi Xie, Yunfan Jiang, Ajay Mandlekar, Chaowei Xiao, Yuke Zhu, Linxi Fan, Anima Anandkumar</sub><br>
  Voyager 在 Minecraft 中自主提出任务、根据环境反馈改进可执行技能，并在持续探索中积累可复用的代码技能库。

<a id="harness-system"></a>

#### 🛠️ Harness 与系统

_收录可变的中间件、工具、上下文、编排与运行时基础设施；当改进对象是智能体外部系统时归入此类。_

- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.11350)<br>
  <sub><b>作者:</b> Peidong Wang, Zhiming Ma, Ying Chang, Xufang Luo, Xiaocui Yang, Shi Feng, Yuqing Yang, Dongsheng Li</sub><br>
  SHAPER 保持模型参数冻结，利用目标环境中的执行轨迹进化可复用技能以及具身智能体外围的上下文代码 Harness。Simulation, no real machine.
- **ETA: A New Agentic Paradigm for Embodied Tasks** (2026-08-04) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.03924) · [Project](https://openmoss.ai/OpenETA/) · [Code](https://github.com/OpenMOSS/OpenETA)<br>
  <sub><b>作者:</b> Yitong Chen, Zezheng Huai, Sixian Li, Yubang Wang, Haozhe Zhang, Yifei Zhang, Hechang Chen, Jingjing Gong, Yu-Gang Jiang, Xipeng Qiu</sub><br>
  ETA 以 Planner—Interface—World 循环组织具身任务，验证执行结果并将交互转化为可复用经验；OpenETA 以可替换规划器、工具、技能、记忆和可回放轨迹实现该范式。
- **You Don't Need To Stay in The Loop: An Agentic Robotics Loop for Robot-Policy Improvement** (2026-08-02) · *arXiv preprint* · `L3 Recursive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.07555)<br>
  <sub><b>作者:</b> Hang Yu</sub><br>
  AgenticRobotics 将训练—评估—改进组织为持久、证据门控的事务，并加入基于提交的恢复、工具质量测量与可审计晋级，使机器人策略改进循环无需操作者持续值守。
- **Cortex: A Bidirectionally Aligned Embodied Agent Framework for Long-horizon Manipulation** (2026-07-06) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.05377) · [Project](https://steinate.github.io/Cortex/) · [Code](https://github.com/InternRobotics/Cortex)<br>
  <sub><b>作者:</b> Jiaqi Peng, Xiqian Yu, Delin Feng, Yuqiang Yang, Wenzhe Cai, Jing Xiong, Ganlin Yang, Jinliang Zheng, Jiafei Cao, Xueyuan Wei, Jiangmiao Pang, Yuan Shen, Tai Wang</sub><br>
  Cortex 通过 32 个规范技能原语、事件均衡训练数据、语义记忆与闭环验证，对齐高层 VLM 规划器和低层 VLA，以完成长时程操作任务。
- **ENPIRE: Agentic Robot Policy Self-Improvement in the Real World** (2026-06-18) · *arXiv preprint* · `L3 Recursive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.19980) · [Project](https://research.nvidia.com/labs/gear/enpire/)<br>
  <sub><b>作者:</b> Wenli Xiao, Jia Xie, Tonghe Zhang, Haotian Lin, Letian "Max" Fu, Haoru Xue, Jalen Lu, Yi Yang, Cunxi Dai, Zi Wang, Jimmy Wu, Guanzhi Wang, S. Shankar Sastry, Ken Goldberg, Linxi "Jim" Fan, Yuke Zhu, Guanya Shi</sub><br>
  ENPIRE 为编码智能体提供可重复的物理反馈循环，覆盖自动复位、验证、运行、策略改进，以及跨单机与机器人集群的训练基础设施和算法代码演化。
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.09416) · [PDF](https://arxiv.org/pdf/2606.09416) · [Zhihu Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)<br>
  <sub><b>作者:</b> Sanghoon Lee, Jiyeong Chae, Kyung-Joon Park</sub><br>
  这篇立场论文主张将机器人中间件升级为 Physical AI 的 Harness 层，在控制、计算和通信层面实施投影、隔离与迁移。 (position paper)
- **ROSClaw: An OpenClaw ROS 2 Framework for Agentic Robot Control and Interaction** (2026-03-27) · *arXiv preprint* · `L1 Adaptive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2603.26997) · [Code](https://github.com/ros-claw/rosclaw)<br>
  <sub><b>作者:</b> Irvin Steve Cardenas, Marcus Anthony Arnett, Natalie Catherine Yeo, Lucky Sah, Jong-Hoon Kim</sub><br>
  ROSClaw 通过动态能力发现、观测归一化、执行前安全验证与审计日志，将模型无关的智能体运行时接入 ROS 2，并在三类真实机器人平台上评估执行层。
- **CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation** (2026-03-23) · *ICML 2026* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2603.22435) · [Project](https://capgym.github.io/) · [Code](https://github.com/capgym/cap-x)<br>
  <sub><b>作者:</b> Letian Fu, Justin Yu, Karim El-Refai, Ethan Kou, Haoru Xue, Huang Huang, Wenli Xiao, Guanzhi Wang, Dantong Niu, Fei-Fei Li, Guanya Shi, Jiajun Wu, Shankar Sastry, Yuke Zhu, Ken Goldberg, Linxi "Jim" Fan</sub><br>
  CaP-X 以 CaP-Gym 和 CaP-Bench 系统评测 Code-as-Policy 智能体，通过 CaP-Agent0 利用执行反馈与自动合成技能进行免训练改进，并以 CaP-RL 实现可从仿真迁移到真机的持久强化学习更新。
- **PhyAgentOS: A Session-Centered Runtime for Embodied Intelligence** (2026-03-12) · *Open-source project* · `L1 Adaptive` `system` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Code](https://github.com/PhyAgentOS-dev/PhyAgentOS) · [Project](https://phy-agent-os.net/)<br>
  <sub><b>作者:</b> Sun Yat-sen University HCP Lab, Peng Cheng Laboratory, X-Era Lab</sub><br>
  PhyAgentOS 是一个开源具身智能体 Harness，通过认知—物理解耦和 Session-Centered Runtime，提供目标与策略适配器、验证与恢复、可审计工作区协议、安全检查及仿真到真机部署。

<a id="embodiment"></a>

#### 🦾 具身适应

_收录形态、传感器、执行器或控制接口的适应；依据智能体物理形态或具身耦合的持久变化进行分类。_

_暂无条目。_

<a id="lifelong-collective-evolution"></a>

### 🌱 终身与集体进化

_收录跨时间、任务、机器人或智能体的能力积累；依据长期保持、迁移、群体学习或集体进化进行分类。_

- **Lifelong Autonomous Improvement of Navigation Foundation Models in the Wild** (2024-09-05) · *OpenReview preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://openreview.net/forum?id=vBj5oC60Lk) · [Project](https://kylestach.github.io/lifelong-nav-rl/) · [Code](https://github.com/kylestach/lifelong-nav-rl)<br>
  <sub><b>作者:</b> Kyle Stachowicz, Lydia Ignatova, Sergey Levine</sub><br>
  LiReN 将离线强化学习预训练与持续自主运行结合，使导航基础模型能够利用新部署环境中的在线经验继续微调。

<a id="safety-alignment"></a>

### 🛡️ 安全与对齐

_收录面向可变具身系统的约束、监督、审计、回滚与恢复；依据如何使自我改进保持可控和对齐进行分类。_

- **AGENTSAFE: Benchmarking the Safety of Embodied Agents on Hazardous Instructions** (2025-06-17) · *CVPR 2026* · `L0 Embodied` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2506.14697)<br>
  <sub><b>作者:</b> Zonghao Ying, Le Wang, Yisong Xiao, Jiakai Wang, Yuqing Ma, Jinyang Guo, Zhenfei Yin, Mingchuan Zhang, Aishan Liu, Xianglong Liu</sub><br>
  AGENTSAFE 提出 SAFE-THOR、SAFE-VERSE 与 SAFE-DIAGNOSE，在 1,350 个对抗性仿真任务上评估具身 VLM 智能体面对危险指令时的感知、规划与执行安全。

<a id="resources"></a>

## 🧪 基准与数据集

- **EmbodiedGovBench: A Benchmark for Governance, Recovery, and Upgrade Safety in Embodied Agent Systems** (2026-04-13) · `L1 Adaptive` `benchmark`. [Paper](https://arxiv.org/abs/2604.11174)<br>
  <sub><b>作者:</b> Xue Qin, Simin Luan, John See, Cong Yang, Zhijun Li</sub><br>
  EmbodiedGovBench 面向能力边界、运行漂移、恢复、策略可移植性、升级安全、人工接管和审计完整性提出具身治理评测。

## 🏭 产业与实验室动态

- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) · `L1 Adaptive` `news`. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)<br>
  NVIDIA 的 GR00T 开发平台将模拟、遥操作、策略训练、评估和部署连接为完整的人形机器人工作流，并同步发布 GR00T 1.7 模型。
- **SIMA 2: A Gemini-Powered AI Agent for 3D Virtual Worlds** (2025-12-05) · `L2 Self-Improving` `news`. [Official](https://deepmind.google/blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/) · [Report](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/SIMA_Tech_Report_2025.pdf)<br>
  Google DeepMind 报告称，SIMA 2 能利用 Gemini 生成的任务与反馈，在未见过的 3D 世界中使用自主经验训练后续代智能体。

## 📚 综述

- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) · `L0 Embodied` `survey`. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)<br>
  <sub><b>作者:</b> Che Jiang, Jincheng Zhong, Yu Fu, Kai Tian, Junlin Yang, Kaikai Zhao, Yuchong Wang, Tianwei Luo, Weizhi Wang, Yuxin Zuo, Guoli Jia, Xingtai Lv, Dianqiao Lei, Sihang Zeng, Yuru Wang, Zhenzhao Yuan, Xinwei Long, Ermo Hua, Can Ren, Xin Jiang, Shulei Xie, Yuanchun Zheng, Youbang Sun, Biqing Qi, Ning Ding, Kaiyan Zhang, Bowen Zhou</sub><br>
  该综述梳理经验驱动的自改进智能体，从技能、记忆、上下文、工具和环境的运行时适应，延伸到智能体强化学习、元智能体与进化编排。(无具身)
- **Self-evolving Embodied AI** (2026-02-04) · `L2 Self-Improving` `survey`. [Paper](https://arxiv.org/abs/2602.04411)<br>
  <sub><b>作者:</b> Tongtong Feng, Xin Wang, Wenwu Zhu</sub><br>
  该综述从记忆更新、任务切换、环境预测、具身适应和模型进化等维度构建自进化具身 AI 框架。

<a id="contributing"></a>

## 🤝 参与贡献

请阅读 [CONTRIBUTING.zh-CN.md](CONTRIBUTING.zh-CN.md)。每项候选资源都会依据一手来源核验，并经人工审核后进入主列表。

## 📄 许可证

MIT
