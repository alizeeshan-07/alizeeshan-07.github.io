---
title: "Research"
showTableOfContents: true
---

My work sits where **agentic AI meets edge deployment**: systems that reason, but under hard limits on latency, energy, bandwidth, and cost — and that ship with measurable guarantees rather than benchmark scores. Three themes.

I frame these systems as a **timescale hierarchy**: slow, adapting reasoners (LLM agents) set intent and plans over seconds to minutes; fast learned controllers (multi-agent and deep RL) handle scheduling, power, and resource allocation in milliseconds; and a **runtime assurance layer** keeps every level inside its safety envelope — all trained and validated inside digital twins before touching real hardware. The unifying thread is *closed-loop systems where learning happens under hard physical, communication, energy, or cost budgets.*

In short: **the learning does the optimizing, the mathematics does the promising.**

**Methodological signature.** Explicit ablations, pre-registered hypotheses, causal-inference rigor, validated evaluation, and negative results given equal billing with positive ones.

## Efficient & agentic LLMs at the edge

*Thesis spine.*

Large models are moving onto phones, drones, and gateways, but every query still poses a decision: answer locally, escalate to an edge server, or pay the cloud's cost in latency, money, and bandwidth. I study **inference-time compute allocation** — routing, cascades, budgeted escalation, quantized on-device models — treated as a decision problem with enforceable promises on reliability and cost, rather than a pile of tuned thresholds.

**Representative work:** LLM-based retrieval-augmented generation for resource optimization in 6G networks (*IEEE Communications Magazine*, accepted).

## AI-native wireless networks

I work on learning-driven resource management for 5G-Advanced and 6G: deep reinforcement learning and cooperative multi-agent RL for scheduling, power, and spectrum; language-model intent layers above millisecond controllers; and digital twins (ray-traced channel simulation) as the gym where network policies are trained and stress-tested before deployment. Grounded in the 3GPP standards timeline and evaluated on modern GPU-native simulation stacks.

**Representative work:** DDPG-based sum-rate optimization for opportunistic backscatter NOMA networks (*IEEE GLOBECOM 2023*).

## Trustworthy & verifiable AI

Learned policies optimize well but promise nothing. I attach the promises: **runtime guardrails** that hold a policy inside its safety envelope, **constrained policy optimization** so limits are trained in rather than bolted on, and **calibrated uncertainty** so a model knows when to abstain or escalate instead of confidently guessing. Applied to UAV autonomy, integrated sensing and communication, and network control — so a learned policy ships with a certificate rather than a hope, and keeps it under distribution shift.

---

A rule I work by: **never propose a language model where a millisecond control policy belongs — and never ship a learned controller without a certificate.**

## Toolbox

**ML / RL** — PyTorch · QMIX/MAPPO (EPyMARL, BenchMARL) · PPO/SAC · verl/TRL · HF Transformers & PEFT · LoRA/QLoRA · AWQ/GPTQ

**Agents & LLM systems** — LangGraph · CrewAI · MCP · RouteLLM · multi-agent orchestration · tool use and function calling

**Wireless & twins** — NVIDIA Sionna · Aerial Omniverse Digital Twin (AODT) · cuMAC · OpenNTN (3GPP TR 38.811) · Hypatia · srsRAN/OAI

**Edge & serving** — vLLM · llama.cpp · ExecuTorch · Jetson Orin · SmolVLM / Qwen-VL class models

**Safety & assurance** — runtime safety filters (OSQP/cvxpy) · constrained policy optimization · conformal prediction · uncertainty quantification · distribution-shift robustness

**Methodology** — pre-registered hypotheses · explicit ablations · causal DAGs · validated LLM-as-judge evaluation · negative results treated as results

## Currently learning

- **Large reasoning models** — RLVR/GRPO pipelines, process reward models, test-time scaling and budget forcing.
- **LLM pretraining from scratch** — small-scale, aimed at domain foundation models (RF/telemetry), not frontier chasing.
- **Edge AI deployment** — on-device training and adaptation, NPU profiling, energy-aware inference.

Every track ends in an artifact — a from-scratch reproduction, a benchmarked system, or a paper. Never a course certificate.

## Interest areas

LLMs · Quantization · IoT + AI + Wireless · MARL · Edge AI · Digital Twins · Agentic / GenAI · Collaborative & Distributed AI · World Models · Agent Safety & Verifiable Autonomy · ISAC & Semantic Communication · Agentic RL & Test-Time Compute · Security of Agentic Systems
