# Embodied RSI taxonomy

[English](TAXONOMY.md) · [中文](TAXONOMY.zh-CN.md)

## Working definition

Embodied Recursive Self-Improvement is the study of embodied agents that convert their own interaction experience into persistent changes and, at higher levels, improve the process that produces subsequent improvements.

The definition has three tests:

1. **Embodied loop:** improvement evidence comes from acting in a physical or simulated environment, not text-only reasoning alone.
2. **Persistence:** something learned survives the current episode or prompt.
3. **Recursion:** for L3 and above, the changed system measurably strengthens a later improvement cycle.

Reflection, replanning, adaptation, continual learning, and agentic behavior are relevant mechanisms, but none alone proves recursive self-improvement.

## RSI levels

- **L0 — Embodied:** perception and action without persistent self-improvement.
- **L1 — Adaptive:** within-task reflection, replanning, correction, or temporary adaptation.
- **L2 — Self-Improving:** persistent changes to a model, policy, memory, skill, harness, or embodiment using the agent's own experience.
- **L3 — Recursive:** the persistent change improves later goal generation, data collection, evaluation, learning, or system modification.
- **L4 — Open-Ended:** the system autonomously accumulates expanding capabilities over long horizons and in open-ended spaces.

Use the level directly supported by reported evidence.

## Academic sections

- **Foundations & Definitions:** theory, definitions and perspectives.
- **Goal & Curriculum Generation:** capability-gap discovery, task generation, curricula, autonomous experiments, and open-ended exploration.
- **Autonomous Experience Acquisition:** self-directed rollouts, data collection, simulation, imagination, active learning, and fleet experience.
- **Self-Evaluation & Feedback:** success detection, critics, verifiers, rewards, diagnosis, uncertainty, and credit assignment.
- **Model & Policy:** parameter, policy, world-model, online-RL, and test-time improvements.
- **Memory & Knowledge:** persistent episodic or semantic memory and knowledge consolidation.
- **Skills & Behaviors:** skill discovery, synthesis, composition, libraries.
- **Harness & System:** context, tools, interfaces, planners, executors, runtime architecture, and workflow evolution.
- **Embodiment Adaptation:** sensor, action-space, morphology, hardware-software, and cross-embodiment adaptation.
- **Lifelong & Collective Evolution:** retention, transfer, continual learning, fleet learning, and multi-agent knowledge sharing.
- **Safety & Alignment:** safe exploration, oversight, constraints, rollback, auditing, robustness, and self-modification boundaries.

## Orthogonal metadata

RSI level is separate from artifact type, provenance, topic, and openness. Code is marked `open-source` only when an explicit open-source license is present; public code without such a license is `source-available`.
