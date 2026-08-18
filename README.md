<div align="center">
  <img src="assets/embodied-rsi-banner.svg" width="100%" alt="Awesome Embodied RSI banner">
  <br><br>
  <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <img src="https://img.shields.io/badge/curation-human--reviewed-2ea44f?style=flat-square" alt="Human reviewed">
  <img src="https://img.shields.io/badge/update-weekly-6366f1?style=flat-square" alt="Updated weekly">
  <img src="https://img.shields.io/badge/RSI-L0%20%E2%86%92%20L4-f97316?style=flat-square" alt="RSI levels L0 through L4">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-0ea5e9?style=flat-square" alt="MIT license"></a>
  <br><br>
  <strong>A curated map of research, systems, benchmarks, and industry progress<br>toward experience-driven embodied agents that improve—and improve how they improve.</strong>
  <br><br>
  <a href="README.zh-CN.md">中文</a> · <a href="docs/TAXONOMY.md">Taxonomy</a> · <a href="CONTRIBUTING.md">Contributing</a>
</div>

<br>

<table>
  <tr>
    <td align="center" width="20%"><a href="#overview"><b>🧭 Overview</b></a><br><sub>Definition & scope</sub></td>
    <td align="center" width="20%"><a href="#highlights"><b>🔥 Highlights</b></a><br><sub>Latest selections</sub></td>
    <td align="center" width="20%"><a href="#research"><b>🧠 Research</b></a><br><sub>Academic landscape</sub></td>
    <td align="center" width="20%"><a href="#resources"><b>🧪 Resources</b></a><br><sub>Benchmarks & surveys</sub></td>
    <td align="center" width="20%"><a href="#contributing"><b>🤝 Contribute</b></a><br><sub>Suggest a resource</sub></td>
  </tr>
</table>

<p align="center"><b>19</b> research works &nbsp;·&nbsp; <b>3</b> industry updates &nbsp;·&nbsp; <b>1</b> benchmark &nbsp;·&nbsp; <b>2</b> surveys</p>

<a id="overview"></a>

## 🧭 What is Embodied RSI?

Embodied Recursive Self-Improvement (Embodied RSI) studies agents that use experience from interaction with physical or simulated environments to make persistent improvements to their models, policies, memories, skills, harnesses, or embodiments—and, at higher levels, improve their ability to improve again.

<p align="center"><code>Experience → Evaluate → Update → Re-deploy ↺</code></p>

## 🧩 Scope, Taxonomy & RSI Levels

| Level | Stage | What changes? | Role in this collection |
|:---:|---|---|---|
| `L0` | **Embodied** | Perception and action, without persistent improvement | Background |
| `L1` | **Adaptive** | In-task adaptation, reflection, or replanning | Related work |
| `L2` | **Self-Improving** | Persistent changes from the agent's own experience | **Core** |
| `L3` | **Recursive** | Components that strengthen later improvement cycles | **Core RSI** |
| `L4` | **Open-Ended** | Autonomous goals and expanding capability accumulation | Frontier |

The core collection prioritizes L2–L4. L0–L1 items are included only when they establish an important foundation or benchmark.

<a id="highlights"></a>

## 🔥 Latest Weekly Highlights

<!-- WEEKLY_HIGHLIGHTS -->
- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2608.11350)<br>
  <sub><b>Authors:</b> Peidong Wang, Zhiming Ma, Ying Chang, Xufang Luo, Xiaocui Yang, Shi Feng, Yuqing Yang, Dongsheng Li</sub><br>
  SHAPER keeps model weights frozen while using target-environment rollouts to evolve reusable skills and the context-code harness that surrounds an embodied agent.
- **LeRobot v0.6.0: Imagine, Evaluate, Improve** (2026-07-07) `L1 Adaptive` `news`. [Official](https://huggingface.co/blog/lerobot-release-v060)<br>
  LeRobot v0.6.0 adds world-model policies, a unified reward-model API, simulation benchmarks, rollout tooling, and human-in-the-loop corrections for robot-learning workflows.
- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) `L1 Adaptive` `news`. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)<br>
  NVIDIA's GR00T development platform connects simulation, teleoperation, policy training, evaluation, and deployment in an integrated humanoid-robot workflow, alongside the GR00T 1.7 model release.
- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) `L1 Adaptive` `survey`. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)<br>
  <sub><b>Authors:</b> Che Jiang, Jincheng Zhong, Yu Fu, Kai Tian, Junlin Yang, Kaikai Zhao, Yuchong Wang, Tianwei Luo, Weizhi Wang, Yuxin Zuo, Guoli Jia, Xingtai Lv, Dianqiao Lei, Sihang Zeng, Yuru Wang, Zhenzhao Yuan, Xinwei Long, Ermo Hua, Can Ren, Xin Jiang, Shulei Xie, Yuanchun Zheng, Youbang Sun, Biqing Qi, Ning Ding, Kaiyan Zhang, Bowen Zhou</sub><br>
  This survey organizes experience-driven self-improving agents from runtime adaptation of skills, memory, context, tools, and environments through agent reinforcement learning to meta-agents and evolution orchestration.
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) `L1 Adaptive` `paper`. [Paper](https://arxiv.org/abs/2606.09416) · [PDF](https://arxiv.org/pdf/2606.09416) · [Zhihu Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)<br>
  <sub><b>Authors:</b> Sanghoon Lee, Jiyeong Chae, Kyung-Joon Park</sub><br>
  This position paper argues that robot middleware should become the harness layer for Physical AI, enforcing projection, isolation, and transfer across control, compute, and communication.

<a id="research"></a>

## 🧠 Academic Research

| Research area | Coverage and primary classification criterion |
|---|---|
| [Foundations & Definitions](#foundations-definitions) | Concepts, definitions, boundaries, and theory; classified here when framing Embodied RSI is the work's primary contribution. |
| [Goal & Curriculum Generation](#goal-curriculum-generation) | Autonomous generation of goals, tasks, rewards, experiments, or curricula; classified by what drives the agent's next learning objective. |
| [Autonomous Experience Acquisition](#autonomous-experience-acquisition) | Autonomous collection, generation, and selection of interaction experience; classified by how the agent obtains its own improvement data. |
| [Self-Evaluation & Feedback](#self-evaluation-feedback) | Critics, rewards, verifiers, reflection, and outcome diagnosis; classified by how the system measures performance and produces feedback. |
| **[Self-Improvement Mechanisms](#self-improvement-mechanisms)** | Persistent changes are grouped by their primary improvement target: model or policy, memory, skills, harness, or embodiment. |
| [Model & Policy](#model-policy) | Persistent updates to models, policies, or world models; classified here when learned parameters or decision rules are the main improvement target. |
| [Memory & Knowledge](#memory-knowledge) | Persistent storage, revision, consolidation, and retrieval of learned knowledge; classified by changes to what the agent remembers and reuses. |
| [Skills & Behaviors](#skills-behaviors) | Acquisition, refinement, composition, and reuse of skills or behaviors; classified by changes to the agent's executable capability repertoire. |
| [Harness & System](#harness-system) | Mutable middleware, tools, context, orchestration, and runtime infrastructure; classified here when the external system around the agent is improved. |
| [Embodiment](#embodiment) | Adaptation of morphology, sensors, actuators, or control interfaces; classified by persistent changes to the agent's physical form or embodiment coupling. |
| [Lifelong & Collective Evolution](#lifelong-collective-evolution) | Accumulation across time, tasks, robots, or agents; classified by long-horizon retention, transfer, fleet learning, or collective evolution. |
| [Safety & Alignment](#safety-alignment) | Constraints, oversight, auditing, rollback, and recovery for changing embodied systems; classified by how self-improvement remains controlled and aligned. |

<a id="foundations-definitions"></a>

### 🧱 Foundations & Definitions

_Concepts, definitions, boundaries, and theory; classified here when framing Embodied RSI is the work's primary contribution._

- **Intelligent Robot Manipulation Requires Self-Directed Learning** (2026-03-04) `L1 Adaptive` `paper`. [Paper](https://openreview.net/forum?id=5IpSR7v4gj)<br>
  <sub><b>Authors:</b> Li Chen, Chonghao Sima, Kashyap Chitta, Antonio Loquercio, Ping Luo, Yi Ma, Hongyang Li</sub><br>
  This perspective argues that intelligent manipulation must move beyond imitation toward self-directed goal identification, skill acquisition, and performance evaluation without assuming resets or clean reward signals.
- **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents** (2025-05-29) `L1 Adaptive` `paper`. [Paper](https://arxiv.org/abs/2505.22954) · [Project](https://sakana.ai/dgm/) · [Code](https://github.com/jennyzzt/dgm)<br>
  <sub><b>Authors:</b> Jenny Zhang, Shengran Hu, Cong Lu, Robert Lange, Jeff Clune</sub><br>
  The Darwin Gödel Machine iteratively modifies and empirically evaluates its own coding-agent codebase while maintaining an archive of discovered variants for open-ended exploration.

<a id="goal-curriculum-generation"></a>

### 🎯 Goal & Curriculum Generation

_Autonomous generation of goals, tasks, rewards, experiments, or curricula; classified by what drives the agent's next learning objective._

- **OMNI-EPIC: Open-endedness via Models of human Notions of Interestingness with Environments Programmed in Code** (2024-05-24) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2405.15568) · [Project](https://omni-epic.vercel.app/)<br>
  <sub><b>Authors:</b> Maxence Faldor, Jenny Zhang, Antoine Cully, Jeff Clune</sub><br>
  OMNI-EPIC uses foundation models to continually generate learnable and interesting simulated tasks, environments, and rewards conditioned on an agent's current learning progress.

<a id="autonomous-experience-acquisition"></a>

### 🔄 Autonomous Experience Acquisition

_Autonomous collection, generation, and selection of interaction experience; classified by how the agent obtains its own improvement data._

- **Autonomous Improvement of Instruction Following Skills via Foundation Models** (2024-07-30) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2407.20635)<br>
  <sub><b>Authors:</b> Zhiyuan Zhou, Pranav Atreya, Abraham Lee, Homer Walke, Oier Mees, Sergey Levine</sub><br>
  The method uses vision-language models to autonomously collect and evaluate meaningful real-robot experience, then improves instruction-following policies without human annotations.

<a id="self-evaluation-feedback"></a>

### 🪞 Self-Evaluation & Feedback

_Critics, rewards, verifiers, reflection, and outcome diagnosis; classified by how the system measures performance and produces feedback._

- **RFTF: Reinforcement Fine-tuning for Vision-language-action Models with Temporal Feedback** (2025-09-19) `L1 Adaptive` `paper`. [Paper](https://openreview.net/forum?id=v8fZ1PbV4D)<br>
  <sub><b>Authors:</b> Junyang Shu, Zhiwei Lin, Yongtao Wang</sub><br>
  RFTF trains a value model from temporal information to provide dense feedback for reinforcement fine-tuning of VLA policies and reports rapid task adaptation on CALVIN.

<a id="self-improvement-mechanisms"></a>

### ♻️ Self-Improvement Mechanisms

_Persistent self-improvement is organized by the system component that changes and remains available to later episodes._

<a id="model-policy"></a>

#### 🧠 Model & Policy

_Persistent updates to models, policies, or world models; classified here when learned parameters or decision rules are the main improvement target._

- **Self-Improving Loops for Visual Robotic Planning** (2026-05-27) `L2 Self-Improving` `paper`. [Paper](https://openreview.net/forum?id=HK9OWSMgoq)<br>
  <sub><b>Authors:</b> Calvin Luo, Zilai Zeng, Mingxi Jia, Yilun Du, Chen Sun</sub><br>
  SILVR repeatedly updates a visual planning model on self-produced trajectories and reports continuing gains on unseen simulated tasks and real-arm manipulation.
- **VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model** (2026-02-12) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2602.12063) · [Project](https://sites.google.com/view/vla-w)<br>
  <sub><b>Authors:</b> Yanjiang Guo, Tony Lee, Lucy Xiaoyang Shi, Jianyu Chen, Percy Liang, Chelsea Finn</sub><br>
  VLAW alternates between improving an action-conditioned video world model with real robot rollouts and improving a VLA policy with synthetic rollouts generated by that world model.
- **π*0.6: a VLA That Learns From Experience** (2025-11-18) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2511.14759) · [Official](https://www.pi.website/blog/pistar06)<br>
  <sub><b>Authors:</b> Physical Intelligence, Ali Amin, Raichelle Aniceto, Ashwin Balakrishna, Kevin Black, Ken Conley, Grace Connors, James Darpinian, Karan Dhabalia, Jared DiCarlo, Danny Driess, Michael Equi, Adnan Esmail, Yunhao Fang, Chelsea Finn, Catherine Glossop, Thomas Godden, Ivan Goryachev, Lachy Groom, Hunter Hancock, Karol Hausman, Gashon Hussein, Brian Ichter, Szymon Jakubczak, Rowan Jen, Tim Jones, Ben Katz, Liyiming Ke, Chandra Kuchi, Marinda Lamb, Devin LeBlanc, Sergey Levine, Adrian Li-Bell, Yao Lu, Vishnu Mano, Mohith Mothukuri, Suraj Nair, Karl Pertsch, Allen Z. Ren, Charvi Sharma, Lucy Xiaoyang Shi, Laura Smith, Jost Tobias Springenberg, Kyle Stachowicz, Will Stoeckle, Alex Swerdlow, James Tanner, Marcel Torne, Quan Vuong, Anna Walling, Haohuan Wang, Blake Williams, Sukwon Yoo, Lili Yu, Ury Zhilinsky, Zhiyuan Zhou</sub><br>
  RECAP improves the π*0.6 vision-language-action model through iterative real-robot rollouts, reward feedback, and corrective interventions on long-horizon manipulation tasks.
- **Self-Improving Embodied Foundation Models** (2025-09-18) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2509.15155) · [Project](https://self-improving-efms.github.io/)<br>
  <sub><b>Authors:</b> Seyed Kamyar Seyed Ghasemipour, Ayzaan Wahid, Jonathan Tompson, Pannag Sanketi, Igor Mordatch</sub><br>
  A two-stage post-training recipe derives rewards and success detection from a pretrained embodied foundation model, enabling robot fleets to practice autonomously and acquire new skills.
- **SELFI: Autonomous Self-Improvement with RL for Vision-Based Navigation around People** (2024-09-05) `L2 Self-Improving` `paper`. [Paper](https://openreview.net/forum?id=rRpmVq6yHv) · [Project](https://sites.google.com/view/selfi-rl/)<br>
  <sub><b>Authors:</b> Noriaki Hirose, Dhruv Shah, Kyle Stachowicz, Ajay Sridhar, Sergey Levine</sub><br>
  SELFI fine-tunes pretrained visual navigation policies from online real-robot experience, improving collision avoidance and socially compliant behavior with limited intervention.
- **RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation** (2023-06-20) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2306.11706) · [Official](https://deepmind.google/blog/robocat-a-self-improving-robotic-agent)<br>
  <sub><b>Authors:</b> Konstantinos Bousmalis, Giulia Vezzani, Dushyant Rao, Coline Devin, Alex X. Lee, Maria Bauza, Todor Davchev, Yuxiang Zhou, Agrim Gupta, Akhil Raju, Antoine Laurens, Claudio Fantacci, Valentin Dalibard, Martina Zambelli, Murilo Martins, Rugile Pevceviciute, Michiel Blokzijl, Misha Denil, Nathan Batchelor, Thomas Lampe, Emilio Parisotto, Konrad Żołna, Scott Reed, Sergio Gómez Colmenarejo, Jon Scholz, Abbas Abdolmaleki, Oliver Groth, Jean-Baptiste Regli, Oleg Sushkov, Tom Rothörl, José Enrique Chen, Yusuf Aytar, Dave Barker, Joy Ortiz, Martin Riedmiller, Jost Tobias Springenberg, Raia Hadsell, Francesco Nori, Nicolas Heess</sub><br>
  RoboCat adapts to new robot arms and tasks, generates additional practice trajectories, and incorporates them into later generalist training rounds.
- **Self-Improving Robots: End-to-End Autonomous Visuomotor Reinforcement Learning** (2023-03-02) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2303.01488) · [Project](https://architsharma97.github.io/self-improving-robots/)<br>
  <sub><b>Authors:</b> Archit Sharma, Ahmed M. Ahmed, Rehaan Ahmad, Chelsea Finn</sub><br>
  MEDAL++ lets real robots autonomously practice manipulation by learning both task completion and reset behaviors, improving success over behavior cloning with minimal ongoing supervision.

<a id="memory-knowledge"></a>

#### 🗃️ Memory & Knowledge

_Persistent storage, revision, consolidation, and retrieval of learned knowledge; classified by changes to what the agent remembers and reuses._

_No entries yet._

<a id="skills-behaviors"></a>

#### 🧰 Skills & Behaviors

_Acquisition, refinement, composition, and reuse of skills or behaviors; classified by changes to the agent's executable capability repertoire._

- **EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents** (2026-05-11) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2605.10332)<br>
  <sub><b>Authors:</b> Ruofei Ju, Xinrui Wang, Xin Ding, Yifan Yang, Hao Wu, Shiqi Jiang, Qianxi Zhang, Hao Wen, Xiangyu Li, Weijun Wang, Kun Li, Yunxin Liu, Haipeng Dai, Wei Wang, Ting Cao</sub><br>
  EmbodiSkill reflects on trajectories to distinguish flawed skill guidance from execution lapses and persistently revises reusable procedural skills around a frozen model.
- **Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models** (2024-06-26) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2406.18746) · [Project](https://gtziafas.github.io/LRLL_project)<br>
  <sub><b>Authors:</b> Georgios Tziafas, Hamidreza Kasaei</sub><br>
  LRLL grows a composable robot skill library by proposing tasks, storing experience in memory, and distilling successful experience into reusable policies.
- **Voyager: An Open-Ended Embodied Agent with Large Language Models** (2023-05-25) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2305.16291) · [Project](https://voyager.minedojo.org/)<br>
  <sub><b>Authors:</b> Guanzhi Wang, Yuqi Xie, Yunfan Jiang, Ajay Mandlekar, Chaowei Xiao, Yuke Zhu, Linxi Fan, Anima Anandkumar</sub><br>
  Voyager autonomously proposes tasks, refines executable skills from environment feedback, and accumulates a reusable code library during continual exploration in Minecraft.

<a id="harness-system"></a>

#### 🛠️ Harness & System

_Mutable middleware, tools, context, orchestration, and runtime infrastructure; classified here when the external system around the agent is improved._

- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) `L2 Self-Improving` `paper`. [Paper](https://arxiv.org/abs/2608.11350)<br>
  <sub><b>Authors:</b> Peidong Wang, Zhiming Ma, Ying Chang, Xufang Luo, Xiaocui Yang, Shi Feng, Yuqing Yang, Dongsheng Li</sub><br>
  SHAPER keeps model weights frozen while using target-environment rollouts to evolve reusable skills and the context-code harness that surrounds an embodied agent.
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) `L1 Adaptive` `paper`. [Paper](https://arxiv.org/abs/2606.09416) · [PDF](https://arxiv.org/pdf/2606.09416) · [Zhihu Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)<br>
  <sub><b>Authors:</b> Sanghoon Lee, Jiyeong Chae, Kyung-Joon Park</sub><br>
  This position paper argues that robot middleware should become the harness layer for Physical AI, enforcing projection, isolation, and transfer across control, compute, and communication.
- **PhyAgentOS: A Session-Centered Runtime for Embodied Intelligence** (2026-03-12) `L1 Adaptive` `system` `open source`. [Code](https://github.com/PhyAgentOS-dev/PhyAgentOS) · [Project](https://phy-agent-os.net/)<br>
  <sub><b>Authors:</b> Sun Yat-sen University HCP Lab, Peng Cheng Laboratory, X-Era Lab</sub><br>
  PhyAgentOS is an open-source embodied-agent harness built around cognitive-physical decoupling and a session-centered runtime, with target and policy adapters, verification and recovery, auditable workspace protocols, safety checks, and simulation-to-real deployment.

<a id="embodiment"></a>

#### 🦾 Embodiment

_Adaptation of morphology, sensors, actuators, or control interfaces; classified by persistent changes to the agent's physical form or embodiment coupling._

_No entries yet._

<a id="lifelong-collective-evolution"></a>

### 🌱 Lifelong & Collective Evolution

_Accumulation across time, tasks, robots, or agents; classified by long-horizon retention, transfer, fleet learning, or collective evolution._

- **Lifelong Autonomous Improvement of Navigation Foundation Models in the Wild** (2024-09-05) `L2 Self-Improving` `paper`. [Paper](https://openreview.net/forum?id=vBj5oC60Lk) · [Project](https://kylestach.github.io/lifelong-nav-rl/) · [Code](https://github.com/kylestach/lifelong-nav-rl)<br>
  <sub><b>Authors:</b> Kyle Stachowicz, Lydia Ignatova, Sergey Levine</sub><br>
  LiReN combines offline reinforcement-learning pretraining with continual autonomous operation so a navigation foundation model can fine-tune from online experience in new deployment environments.

<a id="safety-alignment"></a>

### 🛡️ Safety & Alignment

_Constraints, oversight, auditing, rollback, and recovery for changing embodied systems; classified by how self-improvement remains controlled and aligned._

_No entries yet._

<a id="resources"></a>

## 🧪 Benchmarks & Datasets

- **EmbodiedGovBench: A Benchmark for Governance, Recovery, and Upgrade Safety in Embodied Agent Systems** (2026-04-13) `L1 Adaptive` `benchmark`. [Paper](https://arxiv.org/abs/2604.11174)<br>
  <sub><b>Authors:</b> Xue Qin, Simin Luan, John See, Cong Yang, Zhijun Li</sub><br>
  EmbodiedGovBench proposes governance-oriented evaluation of capability boundaries, runtime drift, recovery, policy portability, upgrade safety, human override, and audit completeness.

## 🏭 Industry & Lab Updates

- **LeRobot v0.6.0: Imagine, Evaluate, Improve** (2026-07-07) `L1 Adaptive` `news`. [Official](https://huggingface.co/blog/lerobot-release-v060)<br>
  LeRobot v0.6.0 adds world-model policies, a unified reward-model API, simulation benchmarks, rollout tooling, and human-in-the-loop corrections for robot-learning workflows.
- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) `L1 Adaptive` `news`. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)<br>
  NVIDIA's GR00T development platform connects simulation, teleoperation, policy training, evaluation, and deployment in an integrated humanoid-robot workflow, alongside the GR00T 1.7 model release.
- **SIMA 2: A Gemini-Powered AI Agent for 3D Virtual Worlds** (2025-12-05) `L2 Self-Improving` `news`. [Official](https://deepmind.google/blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/) · [Report](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/SIMA_Tech_Report_2025.pdf)<br>
  Google DeepMind reports that SIMA 2 can use Gemini-generated tasks and feedback to train successive agents from self-generated experience in previously unseen 3D worlds.

## 📚 Surveys

- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) `L1 Adaptive` `survey`. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)<br>
  <sub><b>Authors:</b> Che Jiang, Jincheng Zhong, Yu Fu, Kai Tian, Junlin Yang, Kaikai Zhao, Yuchong Wang, Tianwei Luo, Weizhi Wang, Yuxin Zuo, Guoli Jia, Xingtai Lv, Dianqiao Lei, Sihang Zeng, Yuru Wang, Zhenzhao Yuan, Xinwei Long, Ermo Hua, Can Ren, Xin Jiang, Shulei Xie, Yuanchun Zheng, Youbang Sun, Biqing Qi, Ning Ding, Kaiyan Zhang, Bowen Zhou</sub><br>
  This survey organizes experience-driven self-improving agents from runtime adaptation of skills, memory, context, tools, and environments through agent reinforcement learning to meta-agents and evolution orchestration.
- **Self-evolving Embodied AI** (2026-02-04) `L1 Adaptive` `survey`. [Paper](https://arxiv.org/abs/2602.04411)<br>
  <sub><b>Authors:</b> Tongtong Feng, Xin Wang, Wenwu Zhu</sub><br>
  This survey frames self-evolving embodied AI around memory updating, task switching, environment prediction, embodiment adaptation, and model evolution.

<a id="contributing"></a>

## 🤝 Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md). Every proposed resource is checked against its primary source and reviewed before it enters this list.

## 📄 License

MIT
