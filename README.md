<div align="center">
  <img src="assets/embodied-rsi-banner.svg" width="100%" alt="Awesome Embodied RSI banner">
  <br><br>
  <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <img src="https://img.shields.io/badge/curation-human--reviewed-2ea44f?style=flat-square" alt="Human reviewed">
  <img src="https://img.shields.io/badge/update-weekly-6366f1?style=flat-square" alt="Updated weekly">
  <img src="https://img.shields.io/badge/RSI-L0%20%E2%86%92%20L4-f97316?style=flat-square" alt="RSI levels L0 through L4">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-0ea5e9?style=flat-square" alt="MIT license"></a>
  <br><br>
  <strong>Making "Robot improving Robot" possible.<br>A curated map toward experience-driven embodied agents that improve—and improve how they improve.</strong>
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

<p align="center"><b>61</b> research works &nbsp;·&nbsp; <b>7</b> industry updates &nbsp;·&nbsp; <b>5</b> benchmark &nbsp;·&nbsp; <b>7</b> surveys</p>

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

`N/A Digital Reference` marks a relevant method tested only on digital agents; it is not evidence of an embodied RSI level.

<a id="highlights"></a>

## 🔥 Latest Weekly Highlights

<!-- WEEKLY_HIGHLIGHTS -->
- **SenseNova-RoboRSI: Recursive Self-Improvement for Embodied Agents** (2026-10-22) · *Open-source system release* · `L2 Self-Improving` `system` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Code](https://github.com/OpenSenseNova/SenseNova-RoboRSI) · [Weights](https://huggingface.co/sensenova/sensenova-roborsi-27b-preview)<br>
  <sub><b>Authors:</b> Hanming Deng, Zhongang Cai, Haiwen Diao, Zhi Hou, Zhonghua Wu, Qingyi Tao, SenseNova RoboRSI Team</sub><br>
  SenseNova-RoboRSI releases an Apache-2.0 runtime that tests harness revisions against execution traces and feedback, plus preview model weights trained from validated interaction experience. Its October 22 update provides RoboCasa365 Target50 code and guides and reports model use in simulation and on real robots; the full technical report is forthcoming. Published benchmark comparisons are project-reported, so the precise contribution of each improvement component remains to be independently assessed.
- **Toward Recursive Self-Improvement in Physical AI** (2026-10-21) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2610.29677) · [Project](https://physical2rsi.github.io/)<br>
  <sub><b>Authors:</b> Meng Luo, Zechen Bai, Shanqing Xu, Yanlin Li, Kaixin Li, Mengchen Qian, Weifeng Lu, Ran Zhang, Yingtian Zou, Ziyang Luo, Wei Chen, Hongzhan Lin</sub><br>
  This review distinguishes improvement in robot behavior from improvement in the procedure that generates future improvements. It surveys physical-experience feedback, transfer across tasks and hardware, and safety and cost constraints; the authors conclude that existing physical studies have not yet isolated gains caused by recursion itself. As a survey, it is tagged L0 rather than treated as an implemented RSI system.
- **Compile Once, Run Cheap: Frozen, Portable Skills for Embodied Agents, and What Recursive Self-Improvement Adds** (2026-10-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.25114) · [Code](https://github.com/Orillusion/embodied-skill-rsi)<br>
  <sub><b>Authors:</b> Jingwen Bai, Guochao Bai, Canbo Zhang, Shuangqi Li, Minchao Hu, Weichun Huang, Shuang Liu</sub><br>
  Skill-RSI uses an offline coding agent to write, test, and repair robot manipulation skills in RoboTwin 2.0 simulation, then freezes them for held-out evaluation and reuse without a frontier model in the control loop. Four of seven tasks yielded seven frozen skills; inherited repairs outperformed fresh rewrites in eight paired campaigns. The authors' controls attribute most of that gap to inheritance, with limited additional evidence for gains from development feedback, so this is classified as persistent skill improvement rather than demonstrated meta-improvement. The repository releases code, ledgers, and skills; experiments are simulation-only.
- **Learning to Compose: Recursive Self-Improvement of Shared Executable Stacks for Zero-Shot Long-Horizon Robot Manipulation** (2026-10-17) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.24464) · [Project](https://cocacola-lab.github.io/Recursia-website/) · [Code](https://github.com/cocacola-lab/Recursia)<br>
  <sub><b>Authors:</b> Yangzhi Chen, Feiran Liu, Zishuo Wang, Zijian Jin, Xin Zhu, Lecheng Ruan, Wenjuan Han</sub><br>
  Recursia uses execution traces to repair a shared stack of robot tools, skills, contracts, handoffs, and verifiers; validated revisions are frozen and reused on new task compositions. The paper evaluates LIBERO-Pro Long simulation and a physical Franka FR3, reporting gains over ASPIRE in simulation and over a skill-document baseline on three real-robot targets. The released Apache-2.0 repository currently includes the real-robot implementation; simulation code is still forthcoming.
- **InstAgent: A Recursively Self-Improving Agent Operating System for Heterogeneous Robot Collaboration** (2026-10-16) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2610.23098)<br>
  <sub><b>Authors:</b> Haoyang Luo, Junhao Qin, Jingyan Cao, Yi Huang, Guangjie Yang, Xiaoyu Chen, Haotao Lu, Tianxiang Gui, Ye Shi, Jingya Wang</sub><br>
  InstAgent encodes heterogeneous robot collaboration in behavior trees, revises coordination programs from execution feedback, and stores successful revisions for future tasks. On 20 real multi-robot tasks, the authors report gains in success, first-attempt completion, and efficiency. Persistent revision is documented, but stronger meta-improvement is not established.

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

- **Intelligent Robot Manipulation Requires Self-Directed Learning** (2026-03-04) · *OpenReview preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://openreview.net/forum?id=5IpSR7v4gj)<br>
  <sub><b>Authors:</b> Li Chen, Chonghao Sima, Kashyap Chitta, Antonio Loquercio, Ping Luo, Yi Ma, Hongyang Li</sub><br>
  This perspective argues that intelligent manipulation must move beyond imitation toward self-directed learning, in which agents learn from their own experience through real-world interaction. It highlights two challenges that distinguish this setting from conventional reinforcement learning—irreversible environments without resets and noisy, ambiguous feedback without explicit rewards—and identifies self-directed goal selection, skill acquisition, and performance evaluation as key research directions.
- **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents** (2025-05-29) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2505.22954) · [Project](https://sakana.ai/dgm/) · [Code](https://github.com/jennyzzt/dgm)<br>
  <sub><b>Authors:</b> Jenny Zhang, Shengran Hu, Cong Lu, Robert Lange, Jeff Clune</sub><br>
  The Darwin Gödel Machine iteratively modifies and empirically evaluates its own coding-agent codebase while maintaining an archive of discovered variants for open-ended exploration.

<a id="goal-curriculum-generation"></a>

### 🎯 Goal & Curriculum Generation

_Autonomous generation of goals, tasks, rewards, experiments, or curricula; classified by what drives the agent's next learning objective._

- **Playful Agentic Robot Learning** (2026-06-17) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.19419) · [Project](https://playful-rats.github.io/) · [Code](https://github.com/Playful-RATs/RATs)<br>
  <sub><b>Authors:</b> Junyi Zhang, Jiaxin Ge, Hanjun Yoo, Letian Fu, Zihan Yang, Yaowei Liu, Raj Saravanan, Shaofeng Yin, Justin Yu, Dantong Niu, Zirui Wang, Roei Herzig, Ken Goldberg, Yutong Bai, David M. Chan, Ion Stoica, Angjoo Kanazawa, Jiahui Lei, Haiwen Feng, Trevor Darrell</sub><br>
  RATs uses self-directed play to propose learnable manipulation tasks, execute and diagnose code policies, and distill successful attempts into a persistent skill library that transfers to downstream simulated and real-robot tasks.
- **OMNI-EPIC: Open-endedness via Models of human Notions of Interestingness with Environments Programmed in Code** (2024-05-24) · *NeurIPS 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2405.15568) · [Project](https://omni-epic.vercel.app/)<br>
  <sub><b>Authors:</b> Maxence Faldor, Jenny Zhang, Antoine Cully, Jeff Clune</sub><br>
  OMNI-EPIC uses foundation models to continually generate learnable and interesting simulated tasks, environments, and rewards conditioned on an agent's current learning progress.

<a id="autonomous-experience-acquisition"></a>

### 🔄 Autonomous Experience Acquisition

_Autonomous collection, generation, and selection of interaction experience; classified by how the agent obtains its own improvement data._

- **Data-Centric Recursive Self-Improvement for Navigation via Policy-Synchronized Language-Action Dual Bootstrapping** (2026-10-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.15782)<br>
  <sub><b>Authors:</b> Songze Li, Haoming Gu, Ziyang Gong, Zhitong Wang, Gengze Zhou, Zun Wang, Yuhan Zhu, Tianxiang Jiang, Juanzi Li, Qi Wu, Weinan Zhang, Yu Qiao, Wenwei Zhang, Yi Wang</sub><br>
  RSI-Nav processes unlabeled navigation trajectories in successive shards: its current policy generates instructions, executes and filters trajectories, and trains on retained samples before the next shard. It reports 68.6% success on R2R-CE and 72.4% on RxR-CE. The experiments show iterative policy improvement in simulated navigation, without evidence that the improvement procedure itself becomes better.
- **Exploratory, Communicative, and Deployable: Vision-Driven Embodied Agents for Open-World Mobile Manipulation** (2026-07-15) · *ECCV 2026* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.13653) · [Project](https://internrobotics.github.io/REAL/) · [Code](https://github.com/InternRobotics/REAL)<br>
  <sub><b>Authors:</b> Boyu Mi, Mengchen Ma, Yifei Yao, Xing Gao, Junting Chen, Yangzi Li, Zihou Zhu, Guohao Li, Zhenfei Yin, Tai Wang, Yao Mu, Jiangmiao Pang, Hanqing Wang</sub><br>
  REAL combines active exploration, interactive intent disambiguation, supervised fine-tuning, and online reinforcement learning through simulator-consistent APIs, then transfers the resulting agent to a physical dual-arm mobile robot.
- **Autonomous Improvement of Instruction Following Skills via Foundation Models** (2024-07-30) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2407.20635)<br>
  <sub><b>Authors:</b> Zhiyuan Zhou, Pranav Atreya, Abraham Lee, Homer Walke, Oier Mees, Sergey Levine</sub><br>
  The method uses vision-language models to autonomously collect and evaluate meaningful real-robot experience, then improves instruction-following policies without human annotations. The entire system proposes an end-to-end self-improvement loop: the VLM observes the current environment to propose tasks, followed by robot execution, success detection, hindsight relabeling, and learning; hindsight relabeling also allows failed data to be reused.

<a id="self-evaluation-feedback"></a>

### 🪞 Self-Evaluation & Feedback

_Critics, rewards, verifiers, reflection, and outcome diagnosis; classified by how the system measures performance and produces feedback._

- **TraceDance: An Automated System for Building Agent Behavior Benchmarks from Real-World Agent Deployment Traces** (2026-09-27) · *arXiv preprint* · `N/A Digital Reference` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Digital-only](https://img.shields.io/badge/Digital--only-6e7781?style=flat-square). [Paper](https://arxiv.org/abs/2609.33295) · [Project](https://zhishanq.github.io/TraceDance/) · [Repository](https://github.com/ZhishanQ/TraceDance)<br>
  <sub><b>Authors:</b> Dehai Min, Daoan Zhang, Yiming Zeng, Huayi Zhang, Ziyi Chen, Yan Zhang, Qinbo Bai, Mengyuan Chao, Jing Ning, Qiyue Hua, Huiyi Chen, Hanrong Zhang, Henry Peng Zou, Jie Yang, Wei Xu, Philip S. Yu</sub><br>
  TraceDance turns undesirable behaviors found in deployed coding and tool-use agent traces into targeted decision-point benchmarks and rubrics. Across 252,557 sessions it constructs 107 benchmarks with 4,125 instances, providing a possible feedback component for future RSI loops. Its experiments are digital-only, not robotic; the public repository says implementation code is still under internal review.
- **Intrinsic Robot Rewarding: Reusing VLA Representations for Autonomous Evaluation and Policy Improvement** (2026-09-15) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2609.17115)<br>
  <sub><b>Authors:</b> Tobias Schaffer, Mohab Elkhayat, Daniela Nicklas, Mustafa Almohamad, Elham Al-Fuqara</sub><br>
  Intrinsic Robot Rewarding reuses a frozen VLA visual encoder and successful demonstration endpoints as a reference bank for scoring new robot outcomes, aiming to reduce recurring human outcome labeling and connect internal evaluation to policy improvement. The work reports an operational COMAU Racer 3 demonstrator at TRL 4, while positioning physical policy improvement as the next step.
- **A Closed-Loop Multi-Agent Framework for Robust Multi-Robot Manipulation** (2026-07-08) · *RSS 2026* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2607.06990)<br>
  <sub><b>Authors:</b> Yi-Xiang He, Lan Wei, Haoming Cen, Jian-Jian Jiang, Zhuohao Li, Guanxing Lu, Yihan Yang, Dandan Zhang, Wei-Shi Zheng</sub><br>
  A planning agent allocates subtasks, per-robot manipulation agents execute adaptive tools, and a verification agent monitors physical outcomes and returns semantic corrections to close the loop in multi-robot manipulation.
- **From Reaction to Anticipation: Proactive Failure Recovery through Agentic Task Graph for Robotic Manipulation** (2026-05-12) · *RSS 2026* · `L1 Adaptive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.11951) · [Project](https://shengxu.net/AgentChord/) · [Code](https://github.com/EDEM-AI/AgentChord)<br>
  <sub><b>Authors:</b> Sheng Xu, Ruixing Jin, Huayi Zhou, Bo Yue, Guanren Qiao, Yunxin Tai, Yueci Deng, Kui Jia, Guiliang Liu</sub><br>
  AgentChord builds a task graph before execution and enriches it with anticipated, context-aware recovery branches so low-latency monitors can trigger corrective behaviors without waiting for full replanning.
- **CycleVLA: Proactive Self-Correcting Vision-Language-Action Models via Subtask Backtracking and Minimum Bayes Risk Decoding** (2026-01-05) · *arXiv preprint* · `L1 Adaptive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2601.02295) · [Project](https://dannymcy.github.io/cyclevla/) · [Code](https://github.com/dannymcy/cyclevla_code)<br>
  <sub><b>Authors:</b> Chenyang Ma, Kai Lu, Guangyu Yang, Jiuming Liu, Shitong Xu, Bill Byrne, Ioannis Havoutis, Niki Trigoni, Andrew Markham</sub><br>
  CycleVLA predicts incipient failures at subtask transitions, backtracks before execution collapses, and uses Minimum Bayes Risk decoding to improve retries. It is an inference-time adaptive loop rather than persistent RSI, evaluated on LIBERO/LIBERO-Plus and an AgileX PiPER arm with natural and human-injected perturbations.
- **MindPower: Enabling Theory-of-Mind Reasoning in VLM-based Embodied Agents** (2025-11-28) · *CVPR 2026* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2511.23055)<br>
  <sub><b>Authors:</b> Ruoxuan Zhang, Qiyun Zheng, Zhiyu Zhou, Ziqi Liao, Siyu Wu, Jian-Yu Jiang-Lin, Bin Wen, Hongxia Xie, Jianlong Fu, Wen-Huang Cheng</sub><br>
  MindPower adds robot-centric theory-of-mind reasoning over the agent's and humans' beliefs, desires, and intentions, and uses Mind-Reward to optimize consistency between the reasoning chain and generated actions.
- **RFTF: Reinforcement Fine-tuning for Vision-language-action Models with Temporal Feedback** (2025-09-19) · *OpenReview preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://openreview.net/forum?id=v8fZ1PbV4D)<br>
  <sub><b>Authors:</b> Junyang Shu, Zhiwei Lin, Yongtao Wang</sub><br>
  RFTF trains a value model from temporal information to provide dense feedback for reinforcement fine-tuning of VLA policies and reports rapid task adaptation on CALVIN.

<a id="self-improvement-mechanisms"></a>

### ♻️ Self-Improvement Mechanisms

_Persistent self-improvement is organized by the system component that changes and remains available to later episodes._

<a id="model-policy"></a>

#### 🧠 Model & Policy

_Persistent updates to models, policies, or world models; classified here when learned parameters or decision rules are the main improvement target._

- **AdaRSI: On-Demand Recursive Self-Improvement for Embodied Agents** (2026-10-14) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.20474)<br>
  <sub><b>Authors:</b> Peidong Wang, Ying Chang, Zhiming Ma, Xiaocui Yang, Shi Feng, Daqi Liu, Yuzhe Yang, Xu Cao, Chuang Wang, Jian Su, Daling Wang</sub><br>
  AdaRSI first repairs skills and harness components, then replays persistent failures from saved states and selectively fine-tunes unreliable VLA substeps using self-collected demonstrations. On 50 RoboCasa365 simulation tasks, it reports unseen composite-task success rising from 4.6% to 13.8%. The paper supports persistent system and policy improvement, but does not establish that the improvement process itself improves across cycles.
- **SEES: A Self-Evolving Embodied System via Failure-Guided VLA Policy Adaptation** (2026-09-26) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.32698)<br>
  <sub><b>Authors:</b> Ziwen Li, Hanlue Zhang, Zhenyang Ren, Tianyu Huang, Runqi Lin, Haoyu Wang, Zhengqing Gao, Yandong Guo, Fakhri Karray, Tongliang Liu, Chris Russell, Mingming Gong</sub><br>
  SEES monitors long-horizon executions for repeatedly failing atomic skills, reconstructs encountered states in simulation, generates task-specific success criteria, and updates shared VLA adapters with online reinforcement learning. It reports cumulative gains across rounds and transfer to unseen tasks without new expert demonstrations.
- **Robot Self-Improvement via Human-Video Dynamics Models** (2026-06-19) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2606.21406) · [Project](https://ethz-mrl.github.io/)<br>
  <sub><b>Authors:</b> Hanzhi Chen, Anran Zhang, Simon Schaefer, Kejia Chen, Shi Chen, Daniel Cremers, Oier Mees, Stefan Leutenegger</sub><br>
  The paper learns embodiment-agnostic action, dynamics, and value representations from human videos, then introduces Dynamics-Guided Action Correction to rank corrective actions for failed robot states. Across seven real-world manipulation tasks on mobile and static arms, it improves success from 40% to 81% across policy backbones.
- **Self-Improving Loops for Visual Robotic Planning** (2026-05-27) · *OpenReview preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://openreview.net/forum?id=HK9OWSMgoq)<br>
  <sub><b>Authors:</b> Calvin Luo, Zilai Zeng, Mingxi Jia, Yilun Du, Chen Sun</sub><br>
  SILVR repeatedly updates a visual planning model (namely, a video generation model) on self-produced trajectories and reports continuing gains on unseen simulated tasks and real-arm manipulation.
- **RoboClaw: An Agentic Framework for Scalable Long-Horizon Robotic Tasks** (2026-03-12) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2603.11558) · [Project](https://roboclaw-agibot.github.io/) · [Code](https://github.com/RoboClaw-Robotics/RoboClaw)<br>
  <sub><b>Authors:</b> Ruiying Li, Yunlang Zhou, YuYao Zhu, Kylin Chen, Jingyuan Wang, Sukai Wang, Kongtao Hu, Minhui Yu, Bowen Jiang, Zhan Su, Jiayao Ma, Xin He, Yongjian Shen, Yang Yang, Guanghui Ren, Maoqing Yao, Wenhao Wang, Yao Mu</sub><br>
  RoboClaw unifies data collection, policy learning, and deployment under one VLM controller, using paired forward and inverse behaviors for self-resetting on-policy collection and iterative policy refinement on real robots.
- **VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model** (2026-02-12) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2602.12063) · [Project](https://sites.google.com/view/vla-w)<br>
  <sub><b>Authors:</b> Yanjiang Guo, Tony Lee, Lucy Xiaoyang Shi, Jianyu Chen, Percy Liang, Chelsea Finn</sub><br>
  VLAW alternates between improving an action-conditioned video world model with real robot rollouts and improving a VLA policy with synthetic rollouts generated by that world model.
- **π*0.6: a VLA That Learns From Experience** (2025-11-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2511.14759) · [Official](https://www.pi.website/blog/pistar06)<br>
  <sub><b>Authors:</b> Physical Intelligence, Ali Amin, Raichelle Aniceto, Ashwin Balakrishna, Kevin Black, Ken Conley, Grace Connors, James Darpinian, Karan Dhabalia, Jared DiCarlo, Danny Driess, Michael Equi, Adnan Esmail, Yunhao Fang, Chelsea Finn, Catherine Glossop, Thomas Godden, Ivan Goryachev, Lachy Groom, Hunter Hancock, Karol Hausman, Gashon Hussein, Brian Ichter, Szymon Jakubczak, Rowan Jen, Tim Jones, Ben Katz, Liyiming Ke, Chandra Kuchi, Marinda Lamb, Devin LeBlanc, Sergey Levine, Adrian Li-Bell, Yao Lu, Vishnu Mano, Mohith Mothukuri, Suraj Nair, Karl Pertsch, Allen Z. Ren, Charvi Sharma, Lucy Xiaoyang Shi, Laura Smith, Jost Tobias Springenberg, Kyle Stachowicz, Will Stoeckle, Alex Swerdlow, James Tanner, Marcel Torne, Quan Vuong, Anna Walling, Haohuan Wang, Blake Williams, Sukwon Yoo, Lili Yu, Ury Zhilinsky, Zhiyuan Zhou</sub><br>
  RECAP improves the π*0.6 vision-language-action model through iterative real-robot rollouts, reward feedback, and corrective interventions on long-horizon manipulation tasks. It engineers a three-stage demonstration-to-correction-to-practice process through offline RL pretraining and online RL fine-tuning, sparse rewards and remote human correction, and learning from unsuccessful data.
- **Self-Improving Embodied Foundation Models** (2025-09-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2509.15155) · [Project](https://self-improving-efms.github.io/)<br>
  <sub><b>Authors:</b> Seyed Kamyar Seyed Ghasemipour, Ayzaan Wahid, Jonathan Tompson, Pannag Sanketi, Igor Mordatch</sub><br>
  A two-stage post-training recipe derives rewards (Steps-to-Go Head as reward) and success detection from a pretrained embodied foundation model, enabling robot fleets to practice autonomously and acquire new skills. The model itself generate reward without manually-designed reward engineering.
- **RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation** (2023-06-20) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2306.11706) · [Official](https://deepmind.google/blog/robocat-a-self-improving-robotic-agent)<br>
  <sub><b>Authors:</b> Konstantinos Bousmalis, Giulia Vezzani, Dushyant Rao, Coline Devin, Alex X. Lee, Maria Bauza, Todor Davchev, Yuxiang Zhou, Agrim Gupta, Akhil Raju, Antoine Laurens, Claudio Fantacci, Valentin Dalibard, Martina Zambelli, Murilo Martins, Rugile Pevceviciute, Michiel Blokzijl, Misha Denil, Nathan Batchelor, Thomas Lampe, Emilio Parisotto, Konrad Żołna, Scott Reed, Sergio Gómez Colmenarejo, Jon Scholz, Abbas Abdolmaleki, Oliver Groth, Jean-Baptiste Regli, Oleg Sushkov, Tom Rothörl, José Enrique Chen, Yusuf Aytar, Dave Barker, Joy Ortiz, Martin Riedmiller, Jost Tobias Springenberg, Raia Hadsell, Francesco Nori, Nicolas Heess</sub><br>
  RoboCat adapts to new robot arms and tasks, generates additional practice trajectories, and incorporates them into later generalist training rounds.
- **Self-Improving Robots: End-to-End Autonomous Visuomotor Reinforcement Learning** (2023-03-02) · *CoRL 2023* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2303.01488) · [Project](https://architsharma97.github.io/self-improving-robots/)<br>
  <sub><b>Authors:</b> Archit Sharma, Ahmed M. Ahmed, Rehaan Ahmad, Chelsea Finn</sub><br>
  MEDAL++ lets real robots autonomously practice manipulation by learning both task completion and reset behaviors, improving success over behavior cloning with minimal ongoing supervision.

<a id="memory-knowledge"></a>

#### 🗃️ Memory & Knowledge

_Persistent storage, revision, consolidation, and retrieval of learned knowledge; classified by changes to what the agent remembers and reuses._

- **ME-Brain-1.0: Memory, Cognition and Action for Evolving Embodied Intelligence** (2026-09-21) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.24271)<br>
  <sub><b>Authors:</b> Wei He, Hengtao Li, Chenfeng Wang, Zhongrui Yu, Xuhan Zhu, Maokui He, Zide Liu, Xiyue Zhang, Xianwei Mao, Chunpeng Zhou, Jia Shi, Yanze Xin, Jingwen Li, Jingxie Zheng, Sijie Zeng, Fan Lu, Zeyu Zhang, Shuai Guo, Hengxuan Zhang, Pengfei Yu, Yu Liu, Kun Zhan, Yan Xie</sub><br>
  ME-Brain links experience acquisition, hierarchical memory consolidation, skill abstraction, and action execution into a persistent adaptation loop without retraining the model. It reports results on RoboMME and RoboDojo and evaluates six manipulation tasks on a physical Piper dual-arm robot; the paper does not isolate the gain from online evolution in the real-robot benchmark.
- **Safe Task Planning with Long-Term Graph Memory for Embodied Agents** (2026-09-08) · *CoRL 2026* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.08444) · [Project](https://sites.google.com/view/safemem)<br>
  <sub><b>Authors:</b> Siyuan Li, Taiyan Lang, Aoqi Yan, Jia Yu, Feifan Liu, Yihan Du, Yu Zheng, Xun Wang, Peng Liu</sub><br>
  SafeMem incrementally builds a long-term semantic graph of dynamic surroundings and uses an LLM risk predictor to score candidate actions, trigger conservative replanning, and explain hazards. It reports safer task planning on IS-Bench and a real-world robot platform.
- **Don't Drop the BATON: Long-Horizon Robot Manipulation via Agentic Subtask Exploration and Transition-aware Memory** (2026-08-17) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.16889)<br>
  <sub><b>Authors:</b> Bingxin Xu, Yuzhang Shang, Emilio Ferrara</sub><br>
  BATON freezes the VLA but learns reusable subtask solutions through agentic test-time exploration and stores them in transition-aware language memory. Invocation verification, handoff restoration, and lookahead strategy selection make long-horizon composition more reliable on RoboMemArena without parameter updates.
- **When Robots Do the Chores: A Benchmark and Agent for Long-Horizon Household Task Execution** (2026-05-14) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.14504)<br>
  <sub><b>Authors:</b> Zilin Zhu, Longteng Guo, Yanghong Mei, Bowen Pang, Zongxun Zhang, Xingjian He, Ruyi Ji, Jing Liu</sub><br>
  LongAct isolates planning-level autonomy in free-form household chores, while HoloMind combines a DAG planner, multimodal spatial memory, episodic experience reuse, and a global critic for reflective supervision.
- **ABot-Claw: A Foundation for Persistent, Cooperative, and Self-Evolving Robotic Agents** (2026-04-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2604.10096) · [Code](https://github.com/amap-cvlab/ABot-Claw)<br>
  <sub><b>Authors:</b> Dongjie Huo, Haoyun Liu, Guoqing Liu, Dekang Qi, Zhiming Sun, Maoguo Gao, Jianxin He, Yandan Yang, Xinyuan Chang, Feng Xiong, Xing Wei, Zhiheng Ma, Mu Xu</sub><br>
  ABot-Claw extends an agent runtime with capability-driven multi-robot scheduling, cross-embodiment multimodal memory, and critic-based feedback for online progress evaluation, correction, and replanning in real environments.

<a id="skills-behaviors"></a>

#### 🧰 Skills & Behaviors

_Acquisition, refinement, composition, and reuse of skills or behaviors; classified by changes to the agent's executable capability repertoire._

- **Compile Once, Run Cheap: Frozen, Portable Skills for Embodied Agents, and What Recursive Self-Improvement Adds** (2026-10-18) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.25114) · [Code](https://github.com/Orillusion/embodied-skill-rsi)<br>
  <sub><b>Authors:</b> Jingwen Bai, Guochao Bai, Canbo Zhang, Shuangqi Li, Minchao Hu, Weichun Huang, Shuang Liu</sub><br>
  Skill-RSI uses an offline coding agent to write, test, and repair robot manipulation skills in RoboTwin 2.0 simulation, then freezes them for held-out evaluation and reuse without a frontier model in the control loop. Four of seven tasks yielded seven frozen skills; inherited repairs outperformed fresh rewrites in eight paired campaigns. The authors' controls attribute most of that gap to inheritance, with limited additional evidence for gains from development feedback, so this is classified as persistent skill improvement rather than demonstrated meta-improvement. The repository releases code, ledgers, and skills; experiments are simulation-only.
- **Skill-Space Shooting for Autonomous Robot Policy Improvement** (2026-09-29) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2609.38178) · [Project](https://skill-space-shooting.github.io/)<br>
  <sub><b>Authors:</b> Zihang Rui, Renhao Wang, Haoxu Huang, Yang Gao</sub><br>
  Skill-Space Shooting uses foundation-model guidance to explore corrective actions as reusable short skills, then turns successful real-robot trials into policy training signals. The paper reports repeated autonomous policy improvement and cross-task sharing of skills, with policy-only evaluation videos distinguishing learned changes from online repair assistance.
- **ASPIRE: Agentic /Skills Discovery for Robotics** (2026-06-30) · *arXiv preprint* · `L3 Recursive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.00272) · [Project](https://research.nvidia.com/labs/gear/aspire/) · [Code](https://github.com/NVlabs/ASPIRE)<br>
  <sub><b>Authors:</b> Runyu Lu, Yubo Wu, Ethan Kou, Letian Fu, Wenli Xiao, Ajay Mandlekar, Yinzhen Xu, Guanya Shi, Ken Goldberg, Ang Chen, Mosharaf Chowdhury, Yuke Zhu, Linxi "Jim" Fan, Guanzhi Wang</sub><br>
  ASPIRE autonomously writes, executes, diagnoses, repairs, and validates code-as-policy robot programs, then distills successful repairs into a continually expanding skill library that improves later tasks. Its evolutionary search explores diverse task sequences and programs, while experiments across LIBERO-Pro, Robosuite, BEHAVIOR-1K, and YAM bimanual hardware provide evidence of persistent skill reuse, zero-shot transfer, and cross-embodiment sim-to-real transfer.
- **EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents** (2026-05-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2605.10332) · [Code](https://github.com/air-embodied-brain/EmbodiSkill)<br>
  <sub><b>Authors:</b> Ruofei Ju, Xinrui Wang, Xin Ding, Yifan Yang, Hao Wu, Shiqi Jiang, Qianxi Zhang, Hao Wen, Xiangyu Li, Weijun Wang, Kun Li, Yunxin Liu, Haipeng Dai, Wei Wang, Ting Cao</sub><br>
  EmbodiSkill reflects on trajectories to distinguish flawed skill guidance from execution lapses and persistently revises reusable procedural skills around a frozen model. Simulation, no real machine.
- **Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models** (2024-06-26) · *ICRA 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2406.18746) · [Project](https://gtziafas.github.io/LRLL_project)<br>
  <sub><b>Authors:</b> Georgios Tziafas, Hamidreza Kasaei</sub><br>
  LRLL grows a composable robot skill library by proposing tasks, storing experience in memory, and distilling successful experience into reusable policies. LRLL does not perform gradient updates, its goal is to upgrade the paradigm of 'fixed skill library+manual prompts' to a lifelong learning cycle that will grow and summarize skills on its own. The entire learning process is completed through LLM coding, memory retrieval, and experience distillation.
- **Voyager: An Open-Ended Embodied Agent with Large Language Models** (2023-05-25) · *TMLR 2024* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2305.16291) · [Project](https://voyager.minedojo.org/)<br>
  <sub><b>Authors:</b> Guanzhi Wang, Yuqi Xie, Yunfan Jiang, Ajay Mandlekar, Chaowei Xiao, Yuke Zhu, Linxi Fan, Anima Anandkumar</sub><br>
  Voyager autonomously proposes tasks, refines executable skills from environment feedback, and accumulates a reusable code library during continual exploration in Minecraft.

<a id="harness-system"></a>

#### 🛠️ Harness & System

_Mutable middleware, tools, context, orchestration, and runtime infrastructure; classified here when the external system around the agent is improved._

- **SenseNova-RoboRSI: Recursive Self-Improvement for Embodied Agents** (2026-10-22) · *Open-source system release* · `L2 Self-Improving` `system` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Code](https://github.com/OpenSenseNova/SenseNova-RoboRSI) · [Weights](https://huggingface.co/sensenova/sensenova-roborsi-27b-preview)<br>
  <sub><b>Authors:</b> Hanming Deng, Zhongang Cai, Haiwen Diao, Zhi Hou, Zhonghua Wu, Qingyi Tao, SenseNova RoboRSI Team</sub><br>
  SenseNova-RoboRSI releases an Apache-2.0 runtime that tests harness revisions against execution traces and feedback, plus preview model weights trained from validated interaction experience. Its October 22 update provides RoboCasa365 Target50 code and guides and reports model use in simulation and on real robots; the full technical report is forthcoming. Published benchmark comparisons are project-reported, so the precise contribution of each improvement component remains to be independently assessed.
- **Learning to Compose: Recursive Self-Improvement of Shared Executable Stacks for Zero-Shot Long-Horizon Robot Manipulation** (2026-10-17) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.24464) · [Project](https://cocacola-lab.github.io/Recursia-website/) · [Code](https://github.com/cocacola-lab/Recursia)<br>
  <sub><b>Authors:</b> Yangzhi Chen, Feiran Liu, Zishuo Wang, Zijian Jin, Xin Zhu, Lecheng Ruan, Wenjuan Han</sub><br>
  Recursia uses execution traces to repair a shared stack of robot tools, skills, contracts, handoffs, and verifiers; validated revisions are frozen and reused on new task compositions. The paper evaluates LIBERO-Pro Long simulation and a physical Franka FR3, reporting gains over ASPIRE in simulation and over a skill-document baseline on three real-robot targets. The released Apache-2.0 repository currently includes the real-robot implementation; simulation code is still forthcoming.
- **Harness^2: Recursive Agent Harnessing for an Open World** (2026-10-09) · *arXiv preprint* · `N/A Digital Reference` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Digital-only](https://img.shields.io/badge/Digital--only-6e7781?style=flat-square). [Paper](https://arxiv.org/abs/2610.14224) · [Code](https://github.com/google-research/harness2)<br>
  <sub><b>Authors:</b> Ruiyao Xu, Yanfei Chen, Zhongying CuiZhu, Bhavana Dalvi Mishra, Yifei Ming, Han Yu, Rujun Han, Chen-Yu Lee, Tomas Pfister</sub><br>
  Harness^2 combines task-level harness edits with a persistent harness that learns how to improve future tasks from earlier edits. The authors evaluate office, professional-work, and legal agent benchmarks, not robots. Its two-level recursion is a relevant design reference for embodied harnesses, but does not establish an embodied RSI level.
- **Self-Evolving Coding Agents: From Digital Programs to Physical-World Intelligence** (2026-09-28) · *arXiv technical report* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.35432) · [Repository](https://github.com/HexaFuture/PhysicalCoding)<br>
  <sub><b>Authors:</b> Hongcheng Gao, Jingjing Zhou, Zelin Zheng, Shijia Ge, Jay Zhu, Yazhe Wang, Jianshu Zeng, Xuan Shangguan, Di Wu, Lingyu He, Zhiqi Jia, Sihang Wu, Xiao He</sub><br>
  Physical Coding represents task state as Code as World and executable planning, checking, and recovery as Code as Policy. HexaAnything reuses verified traces for harness, tool, and initial data-to-model updates; the report evaluates RoboCasa365, a simulated physics laboratory, and a real AgileX dual-arm robot. Evidence supports partial persistent improvement, while autonomous co-evolution of models and hardware remains future work; the public repository currently contains the report and assets, not implementation code.
- **RoboFoundry: System-as-Policy Evolution for Self-Learning Embodied Agents** (2026-09-26) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.32862) · [Project](https://jingsongliang.com/robofoundry/) · [Repository](https://github.com/robofoundry2026/RoboFoundry)<br>
  <sub><b>Authors:</b> Jingsong Liang, Shuhao Liao, Shizhe Zhang, Diyuan Hou, Yuxin Cai, Xinjian Deng, Chengyang He, Wenhui Huang, Runjia Tan, Zhidong Wang, Lan Yu, Xuesong Tian, Guillaume Sartoretti, Jie Luo, Yao Mu, Wenjun Wu, Wanhua Li, Chen Lv</sub><br>
  RoboFoundry treats context management, persistent memory, and hierarchical skills as an evolvable system policy. It validates task-specific changes before promoting recurring improvements to the general system, with evaluations on EmbodiedBench, RoboMemArena, LIBERO-PRO, and real robots. Its public repository presently lists code release as a TODO, so implementation openness is not assumed.
- **HarnessPAI: An Evolving Harness for Physical AI** (2026-09-24) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.29166) · [Project](https://darwin-agent.github.io/HarnessPAI/) · [Repository](https://github.com/Darwin-Agent/HarnessPAI)<br>
  <sub><b>Authors:</b> Xin Wang, Wenhao Wu, Menghao Zhang, Zhi Wang, Kun Shao, Jian Luan, Yang Li, Qing Li, Shangding Gu, Huichi Zhou, Shuqing Shi, Fei Ni, Shuo Lu, Weicheng Meng, Kang Li, Jin Wu, Kang Zhao, Shangmin Guo, Gen Li, Yongqiang Tang, Zhizhong Zhang, Yuan Xie, Heng Qu</sub><br>
  HarnessPAI keeps an executable task program fixed within each rollout, then uses execution feedback to revise it and retain failure-repair knowledge across rollouts. Across seven simulated settings it reports a 61.6-point gain over pi0.5 on LIBERO-PRO and a 27.2-point gain over WorldDreamer on RoboCasa atomic tasks; its public repository currently contains documentation rather than released implementation code.
- **AdaHVLA: Adaptive Harnesses for Long-Horizon Vision-Language-Action Execution** (2026-09-24) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.29204)<br>
  <sub><b>Authors:</b> Junyi Tang, Jie Peng, Zezhen Ding, Yuan Shen, Tianlong Chen</sub><br>
  AdaHVLA uses separate agents for evidence analysis, code-based harness revision, and behavioral assessment, retaining a graph of hypotheses, revisions, and observed effects across attempts. It reports simulated long-horizon gains on NaVILA-LH and manipulation backbones, plus a real-world deployment example; the evidence supports persistent harness adaptation, not yet stronger future adaptation cycles.
- **RegenHarness: A Robot Agent Harness with Evidence-Gated Recursive Self-Improvement** (2026-09-23) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2609.27612)<br>
  <sub><b>Authors:</b> Kailin Wang, Haoxiang Jie, Yaoyuan Yan, Zhiyou Heng, Zhaosong Li</sub><br>
  RegenHarness separates proposals, execution, verification, and recovery, and uses mission records to propose versioned changes to task templates, routing, and recovery rules. Regression checks and release authorization gate each harness update; a quadruped warehouse mission demonstrates physical execution. Despite its title, the paper does not establish that a revision improves a subsequent improvement cycle, so it is conservatively labeled L2.
- **RRSI: Regularized Recursive Self-Improvement of Agent Harnesses** (2026-09-21) · *arXiv preprint* · `N/A Digital Reference` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Digital-only](https://img.shields.io/badge/Digital--only-6e7781?style=flat-square). [Paper](https://arxiv.org/abs/2609.24972) · [Project](https://regularized-rsi.com/) · [Code](https://github.com/google-research/rrsi)<br>
  <sub><b>Authors:</b> Peng Xia, Rujun Han, Zifeng Wang, Yanfei Chen, Yufan Zhuang, Yoonho Lee, Chengsong Huang, Han Yu, Zhongying CuiZhu, Yifei Ming, Huaxiu Yao, Burak Gokturk, Tomas Pfister, Chen-Yu Lee</sub><br>
  RRSI regularizes how coding-agent harness edits are proposed and accepted: it limits bundled changes, uses an edit-history ledger, rejects benchmark leakage, and prunes noisy or costly additions. It reports gains on held-out digital coding, workspace, and engineering-design benchmarks. This is a methodological reference for embodied harness evolution, not an embodied experiment or evidence of an L0-L4 embodied RSI level.
- **EmbodiedSkills: A Unified Framework for Orchestrating, Training, and Deploying VLA Agents** (2026-09-01) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.01281)<br>
  <sub><b>Authors:</b> Wei Wang, Wenqiao Zhang, Yutong Lin, Yuqian Yuan, Tianwei Lin, Jinhao Mao, Zhenxuan Fan, Mingjian Gao, Yang Dai, Wentong Li, Zheqi Lv, Zheng Dong, Yingjie Niu, Jiaqi Zhu, Jun Xiao, Chao Li, Yueting Zhuang</sub><br>
  EmbodiedSkills treats each skill decision as an execution proposal: a fixed executable-skill interface checks prerequisites, bounds low-level VLA execution, verifies outcomes, and records structured trajectories for optional online adaptation. Qwen3-VL and OpenPI/pi0.5 are evaluated on RoboTwin 2.0 and LIBERO.
- **Physical Agentic AI: An Architecture for Orchestrating a Robot Crew with LLMs** (2026-08-23) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.22657)<br>
  <sub><b>Authors:</b> Xinyuan Liu, Eren Sadikoglu, Riana Chatterjee, Ransalu Senanayake</sub><br>
  Physical Agentic AI separates a non-actuating foundation-model Mission Planner from a deterministic Robot Orchestrator that validates each typed robot skill against capabilities, state, and workflow contracts before execution. Gazebo drone-UGV missions and Unitree G1/Go2 trials show that per-dispatch enforcement blocks injected faults before they produce robot motion.
- **Neurosymbolic Embodied Agents** (2026-08-17) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.16794)<br>
  <sub><b>Authors:</b> Mohammad Albinhassan, Yuming Feng, Alessandra Russo, Pranava Madhyastha</sub><br>
  This neurosymbolic agent first uses a VLM and an exploration harness to acquire goal-relevant predicates and object bindings, then combines PDDL-constrained decoding with Monte Carlo tree search to construct executable long-horizon plans. It reports over 90% success with open 4B-27B models in VirtualHome and ALFWorld without specialized training.
- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.11350)<br>
  <sub><b>Authors:</b> Peidong Wang, Zhiming Ma, Ying Chang, Xufang Luo, Xiaocui Yang, Shi Feng, Yuqing Yang, Dongsheng Li</sub><br>
  SHAPER keeps model weights frozen while using target-environment rollouts to evolve reusable skills and the context-code harness that surrounds an embodied agent. Simulation, no real machine.
- **ETA: A New Agentic Paradigm for Embodied Tasks** (2026-08-04) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.03924) · [Project](https://openmoss.ai/OpenETA/) · [Code](https://github.com/OpenMOSS/OpenETA)<br>
  <sub><b>Authors:</b> Yitong Chen, Zezheng Huai, Sixian Li, Yubang Wang, Haozhe Zhang, Yifei Zhang, Hechang Chen, Jingjing Gong, Yu-Gang Jiang, Xipeng Qiu</sub><br>
  ETA organizes embodied tasks around a Planner-Interface-World loop that verifies outcomes and converts interactions into reusable experience; OpenETA implements the paradigm with replaceable planners, tools, skills, memory, and replayable trajectories.
- **You Don't Need To Stay in The Loop: An Agentic Robotics Loop for Robot-Policy Improvement** (2026-08-02) · *arXiv preprint* · `L3 Recursive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2608.07555)<br>
  <sub><b>Authors:</b> Hang Yu</sub><br>
  AgenticRobotics turns train-evaluate-improve work into durable, evidence-gated transactions with commit-keyed recovery, measured tool quality, and auditable promotion so a robot-policy improvement loop can run without continuous operator attention.
- **Cortex: A Bidirectionally Aligned Embodied Agent Framework for Long-horizon Manipulation** (2026-07-06) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2607.05377) · [Project](https://steinate.github.io/Cortex/) · [Code](https://github.com/InternRobotics/Cortex)<br>
  <sub><b>Authors:</b> Jiaqi Peng, Xiqian Yu, Delin Feng, Yuqiang Yang, Wenzhe Cai, Jing Xiong, Ganlin Yang, Jinliang Zheng, Jiafei Cao, Xueyuan Wei, Jiangmiao Pang, Yuan Shen, Tai Wang</sub><br>
  Cortex aligns a high-level VLM planner and a low-level VLA through 32 canonical skill primitives, event-balanced training data, semantic memory, and closed-loop verification for long-horizon manipulation.
- **ENPIRE: Agentic Robot Policy Self-Improvement in the Real World** (2026-06-18) · *arXiv preprint* · `L3 Recursive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.19980) · [Project](https://research.nvidia.com/labs/gear/enpire/)<br>
  <sub><b>Authors:</b> Wenli Xiao, Jia Xie, Tonghe Zhang, Haotian Lin, Letian "Max" Fu, Haoru Xue, Jalen Lu, Yi Yang, Cunxi Dai, Zi Wang, Jimmy Wu, Guanzhi Wang, S. Shankar Sastry, Ken Goldberg, Linxi "Jim" Fan, Yuke Zhu, Guanya Shi</sub><br>
  ENPIRE gives coding agents a repeatable physical feedback loop for automatic reset, verification, rollout, policy refinement, and evolution of training infrastructure and algorithm code across individual robots and fleets.
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) · *arXiv preprint* · `L1 Adaptive` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2606.09416) · [PDF](https://arxiv.org/pdf/2606.09416) · [Zhihu Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)<br>
  <sub><b>Authors:</b> Sanghoon Lee, Jiyeong Chae, Kyung-Joon Park</sub><br>
  This position paper argues that robot middleware should become the harness layer for Physical AI, enforcing projection, isolation, and transfer across control, compute, and communication. (position paper)
- **ROSClaw: An OpenClaw ROS 2 Framework for Agentic Robot Control and Interaction** (2026-03-27) · *arXiv preprint* · `L1 Adaptive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2603.26997) · [Code](https://github.com/ros-claw/rosclaw)<br>
  <sub><b>Authors:</b> Irvin Steve Cardenas, Marcus Anthony Arnett, Natalie Catherine Yeo, Lucky Sah, Jong-Hoon Kim</sub><br>
  ROSClaw connects model-agnostic agent runtimes to ROS 2 through dynamic capability discovery, normalized observations, pre-execution safety validation, and audit logging, and evaluates the executive layer on three physical robot platforms.
- **CaP-X: A Framework for Benchmarking and Improving Coding Agents for Robot Manipulation** (2026-03-23) · *ICML 2026* · `L2 Self-Improving` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2603.22435) · [Project](https://capgym.github.io/) · [Code](https://github.com/capgym/cap-x)<br>
  <sub><b>Authors:</b> Letian Fu, Justin Yu, Karim El-Refai, Ethan Kou, Haoru Xue, Huang Huang, Wenli Xiao, Guanzhi Wang, Dantong Niu, Fei-Fei Li, Guanya Shi, Jiajun Wu, Shankar Sastry, Yuke Zhu, Ken Goldberg, Linxi "Jim" Fan</sub><br>
  CaP-X combines CaP-Gym and CaP-Bench for controlled evaluation of Code-as-Policy agents, CaP-Agent0 for training-free improvement through execution feedback and synthesized skills, and CaP-RL for persistent reinforcement-learning updates that transfer from simulation to real robots.
- **PhyAgentOS: A Session-Centered Runtime for Embodied Intelligence** (2026-03-12) · *Open-source project* · `L1 Adaptive` `system` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Code](https://github.com/PhyAgentOS-dev/PhyAgentOS) · [Project](https://phy-agent-os.net/)<br>
  <sub><b>Authors:</b> Sun Yat-sen University HCP Lab, Peng Cheng Laboratory, X-Era Lab</sub><br>
  PhyAgentOS is an open-source embodied-agent harness built around cognitive-physical decoupling and a session-centered runtime, with target and policy adapters, verification and recovery, auditable workspace protocols, safety checks, and simulation-to-real deployment.

<a id="embodiment"></a>

#### 🦾 Embodiment

_Adaptation of morphology, sensors, actuators, or control interfaces; classified by persistent changes to the agent's physical form or embodiment coupling._

_No entries yet._

<a id="lifelong-collective-evolution"></a>

### 🌱 Lifelong & Collective Evolution

_Accumulation across time, tasks, robots, or agents; classified by long-horizon retention, transfer, fleet learning, or collective evolution._

- **InstAgent: A Recursively Self-Improving Agent Operating System for Heterogeneous Robot Collaboration** (2026-10-16) · *arXiv preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2610.23098)<br>
  <sub><b>Authors:</b> Haoyang Luo, Junhao Qin, Jingyan Cao, Yi Huang, Guangjie Yang, Xiaoyu Chen, Haotao Lu, Tianxiang Gui, Ye Shi, Jingya Wang</sub><br>
  InstAgent encodes heterogeneous robot collaboration in behavior trees, revises coordination programs from execution feedback, and stores successful revisions for future tasks. On 20 real multi-robot tasks, the authors report gains in success, first-attempt completion, and efficiency. Persistent revision is documented, but stronger meta-improvement is not established.
- **Recursive Self-Improvement through Multi-Agent Self-Supervision** (2026-10-08) · *arXiv preprint* · `N/A Digital Reference` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Digital-only](https://img.shields.io/badge/Digital--only-6e7781?style=flat-square). [Paper](https://arxiv.org/abs/2610.12176) · [Project](https://pub.sakana.ai/mass/) · [Repository](https://github.com/SakanaAI/mass)<br>
  <sub><b>Authors:</b> Hyunin Lee, Jinglue Xu, Jeffrey Seely, Donghyun Lee, Somayeh Sojoudi, Matei Zaharia, Yujin Tang</sub><br>
  MASS alternates multi-agent workflow search and model fine-tuning on self-generated traces, reporting two improvement cycles on open-ended digital benchmarks. It is a reference for collective self-supervision, with no robot execution or embodied RSI evidence. The public repository has code, but its license was not verified here.
- **Hyperagents** (2026-03-19) · *arXiv preprint* · `L3 Recursive` `paper` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2603.19461) · [Code](https://github.com/facebookresearch/Hyperagents)<br>
  <sub><b>Authors:</b> Jenny Zhang, Bingchen Zhao, Wannan Yang, Jakob Foerster, Jeff Clune, Minqi Jiang, Sam Devlin, Tatiana Shavrina</sub><br>
  DGM-Hyperagents unifies a task agent and an editable meta agent so that the mechanism producing future modifications can itself evolve. The manuscript dated August 24 reports persistent memory and performance-tracking improvements that accumulate across runs and transfer among coding, paper review, robotics reward design, and math grading; its robotics evidence is simulated reward design rather than real-machine control.
- **Lifelong Autonomous Improvement of Navigation Foundation Models in the Wild** (2024-09-05) · *OpenReview preprint* · `L2 Self-Improving` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://openreview.net/forum?id=vBj5oC60Lk) · [Project](https://kylestach.github.io/lifelong-nav-rl/) · [Code](https://github.com/kylestach/lifelong-nav-rl)<br>
  <sub><b>Authors:</b> Kyle Stachowicz, Lydia Ignatova, Sergey Levine</sub><br>
  LiReN combines offline reinforcement-learning pretraining with continual autonomous operation so a navigation foundation model can fine-tune from online experience in new deployment environments.

<a id="safety-alignment"></a>

### 🛡️ Safety & Alignment

_Constraints, oversight, auditing, rollback, and recovery for changing embodied systems; classified by how self-improvement remains controlled and aligned._

- **AGENTSAFE: Benchmarking the Safety of Embodied Agents on Hazardous Instructions** (2025-06-17) · *CVPR 2026* · `L0 Embodied` `paper` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2506.14697)<br>
  <sub><b>Authors:</b> Zonghao Ying, Le Wang, Yisong Xiao, Jiakai Wang, Yuqing Ma, Jinyang Guo, Zhenfei Yin, Mingchuan Zhang, Aishan Liu, Xianglong Liu</sub><br>
  AGENTSAFE introduces SAFE-THOR, SAFE-VERSE, and SAFE-DIAGNOSE to evaluate how embodied VLM agents perceive, plan, and execute hazardous instructions across 1,350 adversarial simulated tasks.

<a id="resources"></a>

## 🧪 Benchmarks & Datasets

- **RoboQuest: Generalist Physical Agents that Search, Inspect and Test** (2026-10-07) · *arXiv preprint* · `L1 Adaptive` `benchmark` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2610.10388) · [Project](https://declare-lab.github.io/RoboQuest/) · [Code](https://github.com/declare-lab/RoboQuest) · [Data](https://huggingface.co/datasets/declare-lab/RoboQuest)<br>
  <sub><b>Authors:</b> Liu Renhang, Navonil Majumder, Tej Deep Pala, Soujanya Poria</sub><br>
  RoboQuest evaluates within-episode adaptation as mobile manipulators search for hidden objects, inspect properties, and test unfamiliar mechanisms in ten RoboCasa365 kitchen tasks simulated with MuJoCo. It releases 5,000 verified demonstrations. The agents use evidence gathered during an episode, but no improvement persists across episodes; the paper reports that trial-and-error learning remains difficult for most evaluated models. This is an L1 enabling benchmark, not evidence of embodied RSI.
- **EmbodiedMemory-Bench: Benchmarking Embodied Memory for Long-Horizon Embodied Tasks** (2026-09-23) · *arXiv preprint* · `L0 Embodied` `benchmark` ![Open-source](https://img.shields.io/badge/Open--source-2ea44f?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square). [Paper](https://arxiv.org/abs/2609.28236) · [Project](https://zju-omniai.github.io/EmbodiedMemoryBench/) · [Code](https://github.com/ZJU-OmniAI/Embodied-Omni/tree/main/embodied_memory) · [Data](https://huggingface.co/datasets/lzLiang/EmbodiedMemoryBench)<br>
  <sub><b>Authors:</b> Lizhou Liang, Xinyu Zhong, Miao Pan, Xiaohe Zhou, Xuanyu Liu, Qinfeng Li, Peng Li, Jintao Chen, Xuhong Zhang, Wenqi Zhang</sub><br>
  EmbodiedMemory-Bench tests whether memory built from earlier observations and interactions supports later embodied actions across 2,554 simulated episodes covering visual recall, dynamic state tracking, interaction outcomes, and experience generalization. It is an enabling evaluation resource, not evidence of recursive self-improvement. Benchmark code is Apache-2.0 licensed in its subdirectory; the public dataset is CC BY-NC 4.0, and policy-weight release is not verified.
- **X2Real: an eXtensive simulation benchmark for real-world generalist policies** (2026-09-23) · *arXiv preprint* · `L0 Embodied` `benchmark` ![Closed-source](https://img.shields.io/badge/Closed--source-d73a49?style=flat-square) ![Simulation](https://img.shields.io/badge/Simulation-8250df?style=flat-square) ![Real-machine](https://img.shields.io/badge/Real--machine-0969da?style=flat-square). [Paper](https://arxiv.org/abs/2609.27449) · [Data](https://huggingface.co/datasets/x-square-robot/X2Real-Dataset)<br>
  <sub><b>Authors:</b> Lian Ruan, Jade Yang, Sherphylan Gao, Felix Gao, Kyson Liang, Galen Liu, Ligo Wu, Lane Jin, Guu Gu, Bevan Xie, Cloud Yan, Zongzi Yuan, Kino Luo, Emma Chen, Shuwen Chen, Yang Ping, Miles Guo, Rain Sun, Kayden Zhang, Alex Du, Ruihai Wu, Liang Hao, Zhaoshuo Li, Roy Gan, Hao Wang, Qian Wang</sub><br>
  X2Real proposes a simulation benchmark calibrated against physical robot results, spanning 10 capability dimensions, 44 long-horizon tasks, and nearly 300 hours of annotated simulated trajectories. It reports a 0.84 correlation between simulation and real-robot evaluations. This is infrastructure for testing generalist policies and future self-improvement, not a demonstration of RSI itself.
- **Embodied-BenchForge: A Closed-Loop Agentic Workflow for Embodied Benchmark Construction** (2026-09-11) · `L1 Adaptive` `benchmark`. [Paper](https://arxiv.org/abs/2609.13082)<br>
  <sub><b>Authors:</b> Baoyang Jiang, Fengchun Zhang, Leyuan Wang, Haotian Li, Yida Wang, Zhe Ji, Jinshan Lai, Xi Ren, Danyang Li, Zheng Yang, Jianwei Hu, Qiang Ma</sub><br>
  Embodied-BenchForge turns evaluation intents into embodied benchmark artifacts through forward synthesis, backward verification, dependency tracking, and localized repair or rollback. It constructs offline and interactive tracks and studies how verification and skill reuse improve benchmark quality.
- **EmbodiedGovBench: A Benchmark for Governance, Recovery, and Upgrade Safety in Embodied Agent Systems** (2026-04-13) · `L1 Adaptive` `benchmark`. [Paper](https://arxiv.org/abs/2604.11174)<br>
  <sub><b>Authors:</b> Xue Qin, Simin Luan, John See, Cong Yang, Zhijun Li</sub><br>
  EmbodiedGovBench proposes governance-oriented evaluation of capability boundaries, runtime drift, recovery, policy portability, upgrade safety, human override, and audit completeness.

## 🏭 Industry & Lab Updates

- **NVIDIA demonstrates an agent-assisted Microduck simulation-to-policy workflow** (2026-10-23) · `L0 Embodied` `news`. [Official](https://developer.nvidia.com/blog/using-ai-agents-to-teach-robots-like-microduck-to-walk-in-simulation/)<br>
  NVIDIA describes agents helping plan and assemble a Microduck obstacle-course simulator, followed by Isaac Lab policy training in 4,096 parallel environments and local evaluation. The article frames hardware adaptation as a later step; it does not show the agent autonomously revising its own improvement procedure or retaining deployment feedback across cycles. This is an agent-assisted robotics-development example, classified L0.
- **NVIDIA expands Cosmos tools for physical-AI data, world-model adaptation and policy evaluation** (2026-10-21) · `L0 Embodied` `news`. [Official](https://blogs.nvidia.com/blog/cosmos-open-train-evaluate-deploy-world-models/) · [Framework](https://github.com/NVIDIA/cosmos-framework)<br>
  NVIDIA announced Cosmos Data Factory blueprints, agent skills for training and adapting world models, and simulation checkpoints for repeatable physical-AI policy tests. It reports uses in industrial inspection and robot-policy evaluation. These are enabling tools for an experience-and-evaluation loop; the announcement does not establish autonomous, persistent self-improvement of a deployed robot, so it is classified L0.
- **NVIDIA releases ASPIRE v1.0 with real-robot skill refinement and new simulation results** (2026-10-16) · `L2 Self-Improving` `news`. [Official](https://github.com/NVlabs/ASPIRE) · [Project](https://research.nvidia.com/labs/gear/aspire/) · [Announcement](https://x.com/DrJimFan/status/2111128797181567466)<br>
  NVIDIA released ASPIRE v1.0 with open code for iterative robot-program repair, reusable skills, and real-robot skill-discovery demos. The team reports 99% success across 80 LIBERO-Pro tasks. Its own model-scaling comparison shows that stronger backbone models substantially affect this result; the 99% figure should not be attributed solely to self-improvement, nor generalized to all physical tasks.
- **NVIDIA Isaac ROS 5.0 adds agent-ready robotics development workflows** (2026-09-22) · `L0 Embodied` `news`. [Official](https://blogs.nvidia.com/blog/isaac-ros-5-0-agentic-open-source-robotics/) · [Documentation](https://nvidia-isaac-ros.github.io/)<br>
  NVIDIA announced Isaac ROS 5.0 with agent-ready documentation and reusable setup, manipulation, and FoundationStereo fine-tuning skills for robotics developers. This is a relevant physical-AI harness and tooling update, but the announcement does not demonstrate an embodied agent persistently improving itself from execution experience, so it is classified L0.
- **OpenAI reports reaching its automated research intern milestone** (2026-09-06) · `L3 Recursive` `news`. [Official](https://openai.com/index/research-acceleration-view-inside-openai/)<br>
  OpenAI says its measurements have reached the previously announced goal of an automated research intern: a system that performs well-defined research tasks under human direction, including work that would take a skilled researcher several days. This is an industry-reported bounded-RSI signal, not evidence of fully autonomous recursive self-improvement; OpenAI says human researchers still set priorities and judge results.
- **Unitree describes a self-evolving Physical AI development loop** (2026-08-20) · `L3 Recursive` `news`. [Report](https://finance.sina.com.cn/stock/wbstock/2026-08-20/doc-ininxvfu2065291.shtml)<br>
  At the World Robot Conference after Unitree's listing, founder Wang Xingxing was reported as describing a Physical AI loop in which a frontier model generates robot control code, tests it in simulation, and deploys it to physical robots, with human teams still participating. We record this as a reported industry direction rather than a verified deployed RSI system.
- **SIMA 2: A Gemini-Powered AI Agent for 3D Virtual Worlds** (2025-12-05) · `L2 Self-Improving` `news`. [Official](https://deepmind.google/blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/) · [Report](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/SIMA_Tech_Report_2025.pdf)<br>
  Google DeepMind reports that SIMA 2 can use Gemini-generated tasks and feedback to train successive agents from self-generated experience in previously unseen 3D worlds.

## 📚 Surveys

- **Toward Recursive Self-Improvement in Physical AI** (2026-10-21) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2610.29677) · [Project](https://physical2rsi.github.io/)<br>
  <sub><b>Authors:</b> Meng Luo, Zechen Bai, Shanqing Xu, Yanlin Li, Kaixin Li, Mengchen Qian, Weifeng Lu, Ran Zhang, Yingtian Zou, Ziyang Luo, Wei Chen, Hongzhan Lin</sub><br>
  This review distinguishes improvement in robot behavior from improvement in the procedure that generates future improvements. It surveys physical-experience feedback, transfer across tasks and hardware, and safety and cost constraints; the authors conclude that existing physical studies have not yet isolated gains caused by recursion itself. As a survey, it is tagged L0 rather than treated as an implemented RSI system.
- **From Sliding Windows to Self-evolving Lifelong Memory: A Dual-perspective Survey of Memory Paradigms for Long-Horizon Robotics VLA Models** (2026-10-16) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2610.23319)<br>
  <sub><b>Authors:</b> Yong Wang, Boyu Shen, Xinwei Zhang, Yizheng Li, Keyuan Luo</sub><br>
  This survey organizes memory for long-horizon VLA agents by scope and persistence, comparing five established paradigms and an emerging lifelong-memory frontier. It discusses memory management and knowledge evolution as prerequisites for future embodied self-improvement. It is a review, not an experimental demonstration of RSI.
- **World Models for Embodied Intelligence: From Plausible to Controllable to Actionable** (2026-09-15) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2609.16697) · [Project](https://3dagentworld.github.io/)<br>
  <sub><b>Authors:</b> Nanjie Yao, Hao Wang, Chong Cheng, Zhikang Chen, Wenzhe Li, Jiafei Lyu, Li Shen, Peilin Zhao, Zongqing Lu, Gao Huang, Steven Hoi, Dacheng Tao, Deheng Ye</sub><br>
  This survey organizes world models by whether they are plausible, controllable, or actionable, and crosses geometry, physics, and action grounding with improvement loops over data, rewards, policies, and models. It shifts evaluation from visual fidelity toward measurable closed-loop behavioral gains.
- **The Last AI Built by Humans: Toward Genuine Recursive Self-Improvement** (2026-09-10) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2609.11873)<br>
  <sub><b>Authors:</b> Yi Duan, Ying Liu, Zirui Tang, Haodong Chen, Jun Zhou, Yumou Liu, Bangrui Xu, Yukai Wu, Sidi Chen, Yuhan Zhou, Haoyu Wang, Xiaoyou Yu, Shaokun Han, Xuzhou Zhu, Le Zhou, Bolin Lu, Wei Zhou, Jiachen Liu, Nuozhou Fang, Jiaxin Tian, Ruoyu Chen, Yuxuan Li, Kai Zuo, Kaiyan Zhang, Qianyu Yang, Zijie Wang, Jiantao Qiu, Conghui He, Guoliang Li, Bowen Zhou, Zhiyuan Liu, Zhoufutu Wen, Jihua Kang, Xuanhe Zhou, Fan Wu</sub><br>
  This position and survey paper introduces a roadmap from improvement-execution autonomy through strategy, experience acquisition, and environment adaptation to recursive meta-improvement. It compares RSI requirements across scientific discovery, embodied intelligence, and software engineering while emphasizing evaluation and human control.
- **Self-Evolving AI for Humanoids: Mechanisms, Safety, and Evaluation of Post-Deployment Self-Improvement** (2026-09-02) · `L0 Embodied` `survey`. [Paper](https://arxiv.org/abs/2609.13236)<br>
  <sub><b>Authors:</b> Loc X. Nguyen, Avi Deb Raha, Huy Q. Le, Eui-Nam Huh, Dusit Niyato, Choong Seon Hong</sub><br>
  This survey defines post-deployment self-evolution for humanoids over policy, perception, memory, workflow, and body, and organizes mechanisms from self-learning and self-adaptation to self-optimization and self-generation. It treats safety, uncertainty, world-model verification, and human oversight as constraints on admissible evolution.
- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) · `L0 Embodied` `survey`. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)<br>
  <sub><b>Authors:</b> Che Jiang, Jincheng Zhong, Yu Fu, Kai Tian, Junlin Yang, Kaikai Zhao, Yuchong Wang, Tianwei Luo, Weizhi Wang, Yuxin Zuo, Guoli Jia, Xingtai Lv, Dianqiao Lei, Sihang Zeng, Yuru Wang, Zhenzhao Yuan, Xinwei Long, Ermo Hua, Can Ren, Xin Jiang, Shulei Xie, Yuanchun Zheng, Youbang Sun, Biqing Qi, Ning Ding, Kaiyan Zhang, Bowen Zhou</sub><br>
  This survey organizes experience-driven self-improving agents from runtime adaptation of skills, memory, context, tools, and environments through agent reinforcement learning to meta-agents and evolution orchestration.(No Embodiment)
- **Self-evolving Embodied AI** (2026-02-04) · `L2 Self-Improving` `survey`. [Paper](https://arxiv.org/abs/2602.04411)<br>
  <sub><b>Authors:</b> Tongtong Feng, Xin Wang, Wenwu Zhu</sub><br>
  This survey frames self-evolving embodied AI around memory updating, task switching, environment prediction, embodiment adaptation, and model evolution.

<a id="contributing"></a>

## 🤝 Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md). Every proposed resource is checked against its primary source and reviewed before it enters this list.

## 📄 License

MIT
