---
title: "Research"
showTableOfContents: true
---

By 2035, a large share of network traffic is forecast to come from machines rather than people: software agents talking to each other, and robots, drones, and vehicles streaming what they see. Today's networks were built for people who watch and scroll, not for machines that act. My research asks how 6G and the Internet of Things should be built for them.

**Working thesis title:** *Physical AI over 6G IoT Networks: World Models, Agents and Safe Intelligence at the Wireless Edge.*

**The central question:** how should prediction, computation, and coordination be shared between a machine and the network, so that physical AI stays capable and safe over an imperfect wireless link?

The programme stands on four pillars. The first two are the core, the third is a further line of work, and the fourth is a requirement inside each of the others. It is at an early stage: the questions are set and the first problems are being tested, so the manuscripts named below are related groundwork, not finished answers.

## 1. World models for the wireless physical world

*Can a machine learn one predictive model of both its physical surroundings and its radio link, and plan its actions with it?*

A good driver does not only see the road; she predicts what happens next. I want a drone or robot to predict two things at once: the scene around it and the radio signal it depends on. A machine that knows its connection will drop around the next corner can plan its route, and what it sends, before that happens. The emphasis is on models small enough to run on the device or at the edge, and on knowing how far to trust the prediction.

**Related work:** geometry-aware world models for resource management in LEO satellite-terrestrial networks (under revision).

## 2. Energy-aware edge compute

*Where should computation run — on the device, at the network edge, or in the cloud — when energy is a hard limit and the link keeps changing?*

A small sensor or drone cannot carry a large AI model, and these machines send far more data than they receive, the opposite of how today's networks are built. I study the step-by-step decision of what a device computes locally, what it compresses and sends, and what it offloads entirely. The result is judged by whether the physical task succeeds and by measured joules, not by simulated delay alone.

**Related work:** transmitted resolution as an escalation action for multimodal models at the edge (submitted).

## 3. Agent networking

*How should a 6G network carry and coordinate traffic between AI agents, physical and software?*

Soon, large numbers of AI agents will ask the network for service at once and talk to each other through it. Most work so far proposes protocols and architectures. I am interested in what that traffic actually looks like on a radio link, whether existing schedulers serve it, and what it reveals about the machines that generate it.

**Related work:** intent leakage in agentic service discovery for low-altitude wireless networks (submitted); TwinLoop-LLM, token-budgeted LLM strategists above cooperative multi-agent RL for 5G RAN scheduling (in preparation).

## 4. Safe intelligence

*What keeps a machine safe, with a stated guarantee, when its link or its model fails?*

Learned policies optimize well but promise nothing. Safety runs through the other three pillars as a requirement: a learned controller should come with a stated bound on how badly things can go, including when the connection drops. Each result states its level of proof, from a theorem to a measured violation rate.

**Related work:** safety-constrained deep RL for UAV trajectory optimization via composite barrier functions (under revision); deep RL for backscatter IoT communication under quality-of-service constraints (*IEEE Open Journal of the Communications Society*, 2025).

## Alongside the thesis

**Security of non-terrestrial links.** On the [NATO SPS project SHAILLA](/work/#research-projects) I work on the access link of high-altitude platform stations: how it stays secure against an attacker that learns, while keeping a secrecy guarantee.

**AI-native physical layer.** Learned transceivers that are adapted across cells with federated low-rank adapters, exchanging far less data than standard federated training (*IEEE GLOBECOM 2026*, to appear).

**LLMs for network optimization.** Earlier published work: retrieval-augmented generation for resource optimization in 6G networks (*IEEE Communications Magazine*, 2025).

## How I work

I frame these systems as a **timescale hierarchy**: slow, adapting reasoners (LLM agents) set intent and plans over seconds to minutes; fast learned controllers (multi-agent and deep RL) handle scheduling, power, and resource allocation in milliseconds; and a **runtime assurance layer** keeps every level inside its safety envelope — all trained and validated inside digital twins before touching real hardware.

**Method.** Standards-based channel models and ray-traced scenes, recorded 5G traces, and at least one small hardware platform so that energy and latency are measured rather than assumed. Joules are reported beside accuracy. Each make-or-break test is written down before it is run, with explicit ablations, pre-registered hypotheses, and negative results given equal billing with positive ones.

A rule I work by: **never propose a language model where a millisecond control policy belongs — and never ship a learned controller without a stated guarantee.**

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

Physical & Embodied AI over Wireless · World Models · Agent Traffic & Agent-Native Networking · Edge AI · Agent Safety & Verifiable Autonomy · LLMs · Quantization · IoT + AI + Wireless · MARL · Digital Twins · Agentic / GenAI · Collaborative & Distributed AI · ISAC & Semantic Communication · Agentic RL & Test-Time Compute · Security of Agentic Systems · AI-Native PHY & Learned Transceivers · Federated PEFT · Physical-Layer Security for Non-Terrestrial Links · Learning in Deployment under Budgets
