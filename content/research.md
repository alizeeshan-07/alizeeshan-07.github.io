---
title: "Research"
showTableOfContents: true
---

My work pairs **systems engineering with provable guarantees** (CMDP / Lyapunov / finite-time bounds), organized around three themes.

## Efficient & agentic LLMs at the edge

*Thesis spine.*

Large models are moving onto phones, drones, and gateways, but every query still poses a decision: answer locally, escalate to an edge server, or pay the cloud's cost in latency, money, and bandwidth. I study **inference-time compute allocation** — routing, cascades, budgeted escalation, quantized on-device models — treated as a decision problem with enforceable promises on reliability and cost, rather than a pile of tuned thresholds.

**Representative work:** LLM-based retrieval-augmented generation for resource optimization in 6G networks (*IEEE Communications Magazine*, accepted).

## AI-native wireless networks

I work on learning-driven resource management for 5G-Advanced and 6G: deep reinforcement learning and cooperative multi-agent RL for scheduling, power, and spectrum; language-model intent layers above millisecond controllers; and digital twins (ray-traced channel simulation) as the gym where network policies are trained and stress-tested before deployment. Grounded in the 3GPP standards timeline and evaluated on modern GPU-native simulation stacks.

**Representative work:** DDPG-based sum-rate optimization for opportunistic backscatter NOMA networks (*IEEE GLOBECOM 2023*).

## Safe & verifiable autonomy

Learned controllers optimize well but promise nothing. I attach the promises: constrained Markov decision processes, Lyapunov stability, control-barrier safety filters, and conformal prediction — applied to UAV systems, integrated sensing and communication, and network control, so that a learned policy can be deployed with a certificate instead of a hope.

---

A rule I work by: **never propose a language model where a millisecond control policy belongs — and never ship a learned controller without a certificate.**

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
