---
title: "Research"
showTableOfContents: true
---

My work pairs **systems engineering with provable guarantees** (CMDP / Lyapunov / finite-time bounds). Selected directions:

- **Agentic AI & reasoning models** — training LLM agents (RL fine-tuning, RLVR, process reward models, tool-use RL) rather than only prompting them, plus the underlying convergence and sample-complexity theory.
- **Agents for optimization** — LLM agents that plan and adapt over optimization and control loops; budget- and cost-aware decision making, routing, and cascades. *When to think, how long, on which model.*
- **Safe & verifiable autonomy** — CMDPs, Lyapunov/ISS, shields/CBFs, MPC filters, runtime monitors, and conformal-prediction guarantees for learned controllers and LLM agents.
- **AI-native 6G / AI-RAN** — DRL/MARL schedulers, LLM intent layers, GNNs, and digital twins, aligned to the 3GPP Rel-20/21 and ITU IMT-2030 window.
- **Edge AI & efficient inference** — device–edge–cloud cascades and escalation, quantized small models, system-level efficiency (budgets, caching, energy).
- **World models & learned simulators** — RSSM/Dreamer-class and transformer/diffusion dynamics, twins as agent gyms, sim-to-real with causal analysis.
- **Multi-agent RL** — cooperative MARL (QMIX/MAPPO) for distributed resource allocation, swarms, and UAV coordination.
- **Online / continual adaptation of deployed agents** — online LoRA/PEFT, continual RL, two-timescale slow-weights/fast-policy analysis, drift detection.
- **Federated / distributed learning** — federated LoRA/PEFT and decentralized optimization for device and agent fleets under wireless constraints.
- **Modern retrieval topologies** — agentic RAG, retrieval as a budgeted action, groundedness guarantees.
- **Security of agentic systems** — adversarial RL, robust shields, anomaly probes, and red-team benchmarks.

**Application domains:** satellite–terrestrial networks · UAV swarms and the low-altitude economy · integrated sensing and communication (ISAC) · IoT and industrial edge

## Toolbox

**ML / RL** — PyTorch · QMIX/MAPPO (EPyMARL, BenchMARL) · PPO/SAC · verl/TRL · HF Transformers & PEFT · LoRA/QLoRA · AWQ/GPTQ

**Agents & LLM systems** — LangGraph · CrewAI · MCP · RouteLLM · multi-agent orchestration · tool use and function calling

**Wireless & twins** — NVIDIA Sionna · Aerial Omniverse Digital Twin (AODT) · cuMAC · OpenNTN (3GPP TR 38.811) · Hypatia · srsRAN/OAI

**Edge & serving** — vLLM · llama.cpp · ExecuTorch · Jetson Orin · SmolVLM / Qwen-VL class models

**Control & guarantees** — CBF-QP safety filters (OSQP/cvxpy) · constrained MDPs · conformal prediction · two-timescale stochastic approximation

**Methodology** — pre-registered hypotheses · explicit ablations · causal DAGs · validated LLM-as-judge evaluation · negative results treated as results

## Currently learning

- **Large reasoning models** — RLVR/GRPO pipelines, process reward models, test-time scaling and budget forcing.
- **LLM pretraining from scratch** — small-scale, aimed at domain foundation models (RF/telemetry), not frontier chasing.
- **Edge AI deployment** — on-device training and adaptation, NPU profiling, energy-aware inference.

Every track ends in an artifact — a from-scratch reproduction, a benchmarked system, or a paper. Never a course certificate.

## Interest areas

LLMs · Quantization · IoT + AI + Wireless · MARL · Edge AI · Digital Twins · Agentic / GenAI · Collaborative & Distributed AI · World Models · Agent Safety & Verifiable Autonomy · ISAC & Semantic Communication · Agentic RL & Test-Time Compute · Security of Agentic Systems
