<div align="center">
  <img src="assets/embodied-rsi-banner.svg" width="100%" alt="Awesome Embodied RSI banner">
  <br><br>
  <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge-flat2.svg" alt="Awesome"></a>
  <img src="https://img.shields.io/badge/curation-human--reviewed-2ea44f?style=flat-square" alt="Human reviewed">
  <img src="https://img.shields.io/badge/update-weekly-6366f1?style=flat-square" alt="Updated weekly">
  <img src="https://img.shields.io/badge/RSI-E0%20%E2%86%92%20E4-f97316?style=flat-square" alt="RSI levels E0 through E4">
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
| `E0` | **Embodied** | Perception and action, without persistent improvement | Background |
| `E1` | **Adaptive** | In-task adaptation, reflection, or replanning | Related work |
| `E2` | **Self-Improving** | Persistent changes from the agent's own experience | **Core** |
| `E3` | **Recursive** | Components that strengthen later improvement cycles | **Core RSI** |
| `E4` | **Open-Ended** | Autonomous goals and expanding capability accumulation | Frontier |

The core collection prioritizes E2–E4. E0–E1 items are included only when they establish an important foundation or benchmark.

<a id="highlights"></a>

## 🔥 Latest Weekly Highlights

<!-- WEEKLY_HIGHLIGHTS -->
- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) `E2 Self-Improving` `paper` — SHAPER keeps model weights frozen while using target-environment rollouts to evolve reusable skills and the context-code harness that surrounds an embodied agent. [Paper](https://arxiv.org/abs/2608.11350)
- **LeRobot v0.6.0: Imagine, Evaluate, Improve** (2026-07-07) `E1 Adaptive` `news` — LeRobot v0.6.0 adds world-model policies, a unified reward-model API, simulation benchmarks, rollout tooling, and human-in-the-loop corrections for robot-learning workflows. [Official](https://huggingface.co/blog/lerobot-release-v060)
- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) `E1 Adaptive` `news` — NVIDIA's GR00T development platform connects simulation, teleoperation, policy training, evaluation, and deployment in an integrated humanoid-robot workflow, alongside the GR00T 1.7 model release. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)
- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) `E1 Adaptive` `survey` — This survey organizes experience-driven self-improving agents from runtime adaptation of skills, memory, context, tools, and environments through agent reinforcement learning to meta-agents and evolution orchestration. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) `E1 Adaptive` `paper` — This position paper argues that robot middleware should become the harness layer for Physical AI, enforcing projection, isolation, and transfer across control, compute, and communication. [Paper](https://arxiv.org/abs/2606.09416) · [Pdf](https://arxiv.org/pdf/2606.09416) · [Zhihu_Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)

<a id="research"></a>

## 🧠 Academic Research

### 🧱 Foundations & Definitions

- **Intelligent Robot Manipulation Requires Self-Directed Learning** (2026-03-04) `E1 Adaptive` `paper` — This perspective argues that intelligent manipulation must move beyond imitation toward self-directed goal identification, skill acquisition, and performance evaluation without assuming resets or clean reward signals. [Paper](https://openreview.net/forum?id=5IpSR7v4gj)
- **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents** (2025-05-29) `E1 Adaptive` `paper` — The Darwin Gödel Machine iteratively modifies and empirically evaluates its own coding-agent codebase while maintaining an archive of discovered variants for open-ended exploration. [Paper](https://arxiv.org/abs/2505.22954) · [Project](https://sakana.ai/dgm/) · [Code](https://github.com/jennyzzt/dgm)

### 🎯 Goal & Curriculum Generation

- **OMNI-EPIC: Open-endedness via Models of human Notions of Interestingness with Environments Programmed in Code** (2024-05-24) `E2 Self-Improving` `paper` — OMNI-EPIC uses foundation models to continually generate learnable and interesting simulated tasks, environments, and rewards conditioned on an agent's current learning progress. [Paper](https://arxiv.org/abs/2405.15568) · [Project](https://omni-epic.vercel.app/)

### 🔄 Autonomous Experience Acquisition

- **Autonomous Improvement of Instruction Following Skills via Foundation Models** (2024-07-30) `E2 Self-Improving` `paper` — The method uses vision-language models to autonomously collect and evaluate meaningful real-robot experience, then improves instruction-following policies without human annotations. [Paper](https://arxiv.org/abs/2407.20635)

### 🪞 Self-Evaluation & Feedback

- **RFTF: Reinforcement Fine-tuning for Vision-language-action Models with Temporal Feedback** (2025-09-19) `E1 Adaptive` `paper` — RFTF trains a value model from temporal information to provide dense feedback for reinforcement fine-tuning of VLA policies and reports rapid task adaptation on CALVIN. [Paper](https://openreview.net/forum?id=v8fZ1PbV4D)

### ♻️ Self-Improvement Mechanisms

#### 🧠 Model & Policy

- **Self-Improving Loops for Visual Robotic Planning** (2026-05-27) `E2 Self-Improving` `paper` — SILVR repeatedly updates a visual planning model on self-produced trajectories and reports continuing gains on unseen simulated tasks and real-arm manipulation. [Paper](https://openreview.net/forum?id=HK9OWSMgoq)
- **VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model** (2026-02-12) `E2 Self-Improving` `paper` — VLAW alternates between improving an action-conditioned video world model with real robot rollouts and improving a VLA policy with synthetic rollouts generated by that world model. [Paper](https://arxiv.org/abs/2602.12063) · [Project](https://sites.google.com/view/vla-w)
- **π*0.6: a VLA That Learns From Experience** (2025-11-18) `E2 Self-Improving` `paper` — RECAP improves the π*0.6 vision-language-action model through iterative real-robot rollouts, reward feedback, and corrective interventions on long-horizon manipulation tasks. [Paper](https://arxiv.org/abs/2511.14759) · [Official](https://www.pi.website/blog/pistar06)
- **Self-Improving Embodied Foundation Models** (2025-09-18) `E2 Self-Improving` `paper` — A two-stage post-training recipe derives rewards and success detection from a pretrained embodied foundation model, enabling robot fleets to practice autonomously and acquire new skills. [Paper](https://arxiv.org/abs/2509.15155) · [Project](https://self-improving-efms.github.io/)
- **SELFI: Autonomous Self-Improvement with RL for Vision-Based Navigation around People** (2024-09-05) `E2 Self-Improving` `paper` — SELFI fine-tunes pretrained visual navigation policies from online real-robot experience, improving collision avoidance and socially compliant behavior with limited intervention. [Paper](https://openreview.net/forum?id=rRpmVq6yHv) · [Project](https://sites.google.com/view/selfi-rl/)
- **RoboCat: A Self-Improving Generalist Agent for Robotic Manipulation** (2023-06-20) `E2 Self-Improving` `paper` — RoboCat adapts to new robot arms and tasks, generates additional practice trajectories, and incorporates them into later generalist training rounds. [Paper](https://arxiv.org/abs/2306.11706) · [Official](https://deepmind.google/blog/robocat-a-self-improving-robotic-agent)
- **Self-Improving Robots: End-to-End Autonomous Visuomotor Reinforcement Learning** (2023-03-02) `E2 Self-Improving` `paper` — MEDAL++ lets real robots autonomously practice manipulation by learning both task completion and reset behaviors, improving success over behavior cloning with minimal ongoing supervision. [Paper](https://arxiv.org/abs/2303.01488) · [Project](https://architsharma97.github.io/self-improving-robots/)

#### 🗃️ Memory & Knowledge

_No entries yet._

#### 🧰 Skills & Behaviors

- **EmbodiSkill: Skill-Aware Reflection for Self-Evolving Embodied Agents** (2026-05-11) `E2 Self-Improving` `paper` — EmbodiSkill reflects on trajectories to distinguish flawed skill guidance from execution lapses and persistently revises reusable procedural skills around a frozen model. [Paper](https://arxiv.org/abs/2605.10332)
- **Lifelong Robot Library Learning: Bootstrapping Composable and Generalizable Skills for Embodied Control with Language Models** (2024-06-26) `E2 Self-Improving` `paper` — LRLL grows a composable robot skill library by proposing tasks, storing experience in memory, and distilling successful experience into reusable policies. [Paper](https://arxiv.org/abs/2406.18746) · [Project](https://gtziafas.github.io/LRLL_project)
- **Voyager: An Open-Ended Embodied Agent with Large Language Models** (2023-05-25) `E2 Self-Improving` `paper` — Voyager autonomously proposes tasks, refines executable skills from environment feedback, and accumulates a reusable code library during continual exploration in Minecraft. [Paper](https://arxiv.org/abs/2305.16291) · [Project](https://voyager.minedojo.org/)

#### 🛠️ Harness & System

- **Self-Evolving Embodied Agents via Skill-Harness Evolution** (2026-08-11) `E2 Self-Improving` `paper` — SHAPER keeps model weights frozen while using target-environment rollouts to evolve reusable skills and the context-code harness that surrounds an embodied agent. [Paper](https://arxiv.org/abs/2608.11350)
- **Harness Engineering for Physical AI: Robot Middleware Is the Harness Layer** (2026-06-08) `E1 Adaptive` `paper` — This position paper argues that robot middleware should become the harness layer for Physical AI, enforcing projection, isolation, and transfer across control, compute, and communication. [Paper](https://arxiv.org/abs/2606.09416) · [Pdf](https://arxiv.org/pdf/2606.09416) · [Zhihu_Commentary](https://zhuanlan.zhihu.com/p/2049821645158756713)
- **PhyAgentOS: A Session-Centered Runtime for Embodied Intelligence** (2026-03-12) `E1 Adaptive` `system` `open source` — PhyAgentOS is an open-source embodied-agent harness built around cognitive-physical decoupling and a session-centered runtime, with target and policy adapters, verification and recovery, auditable workspace protocols, safety checks, and simulation-to-real deployment. [Code](https://github.com/PhyAgentOS-dev/PhyAgentOS) · [Project](https://phy-agent-os.net/)

#### 🦾 Embodiment

_No entries yet._

### 🌱 Lifelong & Collective Evolution

- **Lifelong Autonomous Improvement of Navigation Foundation Models in the Wild** (2024-09-05) `E2 Self-Improving` `paper` — LiReN combines offline reinforcement-learning pretraining with continual autonomous operation so a navigation foundation model can fine-tune from online experience in new deployment environments. [Paper](https://openreview.net/forum?id=vBj5oC60Lk) · [Project](https://kylestach.github.io/lifelong-nav-rl/) · [Code](https://github.com/kylestach/lifelong-nav-rl)

### 🛡️ Safety & Alignment

_No entries yet._

<a id="resources"></a>

## 🧪 Benchmarks & Datasets

- **EmbodiedGovBench: A Benchmark for Governance, Recovery, and Upgrade Safety in Embodied Agent Systems** (2026-04-13) `E1 Adaptive` `benchmark` — EmbodiedGovBench proposes governance-oriented evaluation of capability boundaries, runtime drift, recovery, policy portability, upgrade safety, human override, and audit completeness. [Paper](https://arxiv.org/abs/2604.11174)

## 🏭 Industry & Lab Updates

- **LeRobot v0.6.0: Imagine, Evaluate, Improve** (2026-07-07) `E1 Adaptive` `news` — LeRobot v0.6.0 adds world-model policies, a unified reward-model API, simulation benchmarks, rollout tooling, and human-in-the-loop corrections for robot-learning workflows. [Official](https://huggingface.co/blog/lerobot-release-v060)
- **Develop Humanoid Robot Policies End-to-End with NVIDIA Isaac GR00T** (2026-07-07) `E1 Adaptive` `news` — NVIDIA's GR00T development platform connects simulation, teleoperation, policy training, evaluation, and deployment in an integrated humanoid-robot workflow, alongside the GR00T 1.7 model release. [Official](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/)
- **SIMA 2: A Gemini-Powered AI Agent for 3D Virtual Worlds** (2025-12-05) `E2 Self-Improving` `news` — Google DeepMind reports that SIMA 2 can use Gemini-generated tasks and feedback to train successive agents from self-generated experience in previously unseen 3D worlds. [Official](https://deepmind.google/blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/) · [Report](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/SIMA_Tech_Report_2025.pdf)

## 📚 Surveys

- **Self-Improving Agents in the Era of Experience: A Survey of Self- to Meta-Evolution** (2026-06-25) `E1 Adaptive` `survey` — This survey organizes experience-driven self-improving agents from runtime adaptation of skills, memory, context, tools, and environments through agent reinforcement learning to meta-agents and evolution orchestration. [Paper](https://openreview.net/pdf?id=IUltZSgLMm) · [Code](https://github.com/FrontisAI/Awesome-Self-Improving-Agents)
- **Self-evolving Embodied AI** (2026-02-04) `E1 Adaptive` `survey` — This survey frames self-evolving embodied AI around memory updating, task switching, environment prediction, embodiment adaptation, and model evolution. [Paper](https://arxiv.org/abs/2602.04411)

<a id="contributing"></a>

## 🤝 Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md). Every proposed resource is checked against its primary source and reviewed before it enters this list.

## 📄 License

MIT
