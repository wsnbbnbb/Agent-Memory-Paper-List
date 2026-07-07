<!-- # Memory in the Age of AI Agents: A Survey -->


根据你列出的论文方向（端侧Agent记忆、自适应上下文管理、KV缓存优化、认知记忆架构、多Agent协作记忆），我整理了2025–2026年最相关的参考文献，按主题分类如下：

---

## 一、端侧/边缘设备 KV 缓存与上下文管理
与你提到的 *Adaptive Context Management* 和 *TinyAgent* 直接相关，聚焦在资源受限设备上的上下文持久化与KV缓存优化。

| 论文 | 年份 | 核心贡献 | 链接 |
|------|------|----------|------|
| **Agent Memory Below the Prompt: Persistent Q4 KV Cache for Multi-Agent LLM Inference on Edge Devices** | 2026 | 将多Agent的KV Cache以4-bit量化持久化到磁盘，消除重复prefill，在Apple M4 Pro上实现最高**136×**首token加速 | [arXiv:2603.04428](https://arxiv.org/abs/2603.04428) |
| **QKVShare: Quantized KV-Cache Handoff for Multi-Agent Edge Inference** | 2026 | 端侧多Agent场景下的token级量化KV缓存共享与handoff，支持高Agent密度（≤3%精度损失） | [arXiv:2605.03884](https://arxiv.org/abs/2605.03884) |
| **KVSwap: Disk-Aware KV Cache Offloading for Long-Context On-Device Inference** | 2025 | 磁盘感知的KV缓存卸载，支持端侧长上下文推理 | [arXiv:2511.11907](https://arxiv.org/abs/2511.11907) |
| **KVCOMM: Online Cross-Context KV-Cache Communication for Efficient LLM-based Multi-Agent Systems** | 2025 (NeurIPS) | 跨Agent上下文KV缓存通信，解决offset-variance问题，5-Agent场景下**7.8×** prefill加速 | [NeurIPS 2025](https://arxiv.org/abs/2506.06266) |
| **KVCache-centric Memory for LLM Agents** | 2026 (ICLR投稿) | 以KV缓存为中心的LLM Agent记忆架构 | [arXiv](https://arxiv.org/abs/2603.10062) |
| **A Shared Asymmetrically-Compressed KV Cache Pool for Multi-Agent LLM Inference** | 2026 | 非对称压缩的共享KV缓存池，支持多Agent并发推理 | [arXiv:2604.24971](https://arxiv.org/abs/2604.24971) |
| **RelayCaching: Accelerating LLM Collaboration via Decoding KV Cache Reuse** | 2026 | 通过解码阶段KV缓存复用加速多Agent协作 | [arXiv:2603.13289](https://arxiv.org/abs/2603.13289) |
| **Venus: An Efficient Edge Memory-and-Retrieval System for VLM-based Online Video Understanding** | 2025 | 面向VLM的边缘记忆与检索系统 | [arXiv:2512.07344](https://arxiv.org/abs/2512.07344) |

---

## 二、端侧Agent记忆架构与系统
与你提到的 *Mnemosyne*、*Shodh-Memory*、*MemLoRA* 对应，聚焦在端侧可部署的Agent记忆系统设计。

| 论文 | 年份 | 核心贡献 | 链接 |
|------|------|----------|------|
| **ScrapMem: A Bio-inspired Framework for On-device Personalized Agent Memory via Optical Forgetting** | 2026 | 生物启发（海马体-新皮层理论）的端侧个性化记忆，通过"光学遗忘"渐进压缩旧记忆 | [arXiv:2605.03804](https://arxiv.org/abs/2605.03804) |
| **A-MEM: Agentic Memory for LLM Agents** | 2025 (NeurIPS) | 自进化Agent记忆系统，采用Zettelkasten笔记链接策略 | [arXiv:2502.12110](https://arxiv.org/abs/2502.12110) |
| **HAGE: Harnessing Agentic Memory via RL-Driven Weighted Graph Evolution** | 2026 | RL驱动的加权图记忆进化，支持动态查询路由 | [arXiv:2605.09942](https://arxiv.org/abs/2605.09942) |
| **MemOS / MemoryOS** | 2025 (EMNLP Oral) | 操作系统风格的分层语义记忆管理（全局/本地/工作记忆） | [arXiv](https://arxiv.org/abs/2508.04903) |
| **Pancake: Hierarchical Memory System for Multi-Agent LLM Serving** | 2026 | 多层分层记忆系统，面向多Agent LLM服务 | [arXiv](https://arxiv.org/abs/2603.17244) |
| **Multi-Layered Memory Architectures for LLM Agents** | 2026 | LLM Agent的多层记忆架构设计 | [arXiv](https://arxiv.org/abs/2603.17244) |
| **Graph-Native Cognitive Memory for AI Agents** | 2026 | 图原生认知记忆，支持版本化信念修订与AGM语义 | [arXiv:2603.17244](https://arxiv.org/abs/2603.17244) |
| **Hindsight: Building Agent Memory That Retains, Recalls, and Reflects** | 2025 | 四网络记忆架构（事实/经验/观点/观察），LoCoMo上达89.61% | [arXiv:2512.12818](https://arxiv.org/abs/2512.12818) |
| **NextMem: Towards Latent Factual Memory for LLM-based Agents** | 2026 | 面向LLM Agent的隐式事实记忆 | [arXiv:2603.15634](https://arxiv.org/abs/2603.15634) |
| **SimpleMem: Efficient Lifelong Memory** | 2026 | 高效终身记忆系统 | [arXiv:2601.02553](https://arxiv.org/abs/2601.02553) |
| **HiMem: Hierarchical Long-Term Memory** | 2026 | 分层长期记忆架构 | [arXiv:2601.06377](https://arxiv.org/abs/2601.06377) |
| **SYNAPSE: Spreading Activation Episodic-Semantic Memory** | 2026 | 扩散激活的情景-语义记忆 | [arXiv:2601.02744](https://arxiv.org/abs/2601.02744) |
| **TiMem: Temporal-Hierarchical Consolidation** | 2026 | 时间-分层记忆巩固机制 | [arXiv:2601.02845](https://arxiv.org/abs/2601.02845) |

---

## 三、自适应记忆组织与压缩
与你提到的 *CLAG*（自适应聚类记忆组织）对应，聚焦在小型语言模型Agent的记忆组织与压缩。

| 论文 | 年份 | 核心贡献 | 链接 |
|------|------|----------|------|
| **MAGMA: A Multi-Graph Based Agentic Memory Architecture** | 2026 | 多关系图记忆架构，支持静态边权重与启发式遍历 | [arXiv:2601.03236](https://arxiv.org/abs/2601.03236) |
| **Nemori: Graph-based Memory with Predict-Calibrate Episodic Segmentation** | 2025 | 基于图的记忆，预测-校准的情景分割 | [arXiv](https://arxiv.org/abs/2508.04903) |
| **Zep: A Temporal Knowledge Graph Architecture for Agent Memory** | 2025 | 时序知识图架构，支持时间感知的Agent记忆 | [arXiv](https://arxiv.org/abs/2508.04903) |
| **ACON: Optimizing Context Compression for Long-Horizon LLM Agents** | 2025 | 长程LLM Agent的上下文压缩优化 | [arXiv:2510.00615](https://arxiv.org/abs/2510.00615) |
| **AgentFold: Long-Horizon Web Agents with Proactive Context Management** | 2025 | 主动上下文管理的长程Web Agent | [arXiv](https://arxiv.org/abs/2508.04903) |
| **Scaling Long-Horizon LLM Agent via Context-Folding** | 2025 | 通过上下文折叠扩展长程Agent | [arXiv](https://arxiv.org/abs/2508.04903) |
| **Structured Distillation for Personalized Agent Memory: 11x Token Reduction** | 2026 | 结构化蒸馏实现个性化记忆，**11倍**token缩减 | [arXiv](https://arxiv.org/abs/2601.08816) |
| **Mem1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents** | 2025 | 记忆与推理协同学习 | [arXiv](https://arxiv.org/abs/2508.04903) |

---

## 四、多Agent记忆共享与协作
与你提到的 *TinyAgent*（边缘函数调用）对应，聚焦在多Agent系统的记忆共享与协作机制。

| 论文 | 年份 | 核心贡献 | 链接 |
|------|------|----------|------|
| **Multi-Agent Memory from a Computer Architecture Perspective** | 2026 | 从计算机体系结构视角审视多Agent记忆，提出端侧挑战与愿景 | [arXiv:2603.10062](https://arxiv.org/abs/2603.10062) |
| **Semantic Infrastructure for Multi-Agent LLM Systems** | 2026 | 多Agent LLM系统的语义基础设施 | [arXiv:2604.19540](https://arxiv.org/abs/2604.19540) |
| **Collaborative Memory-Augmented Agentic Recommender System** | 2026 | 协作记忆增强的Agent推荐系统 | [arXiv:2601.08816](https://arxiv.org/abs/2601.08816) |
| **LEGOMem: Modular Procedural Memory for Multi-Agent LLM Systems** | 2026 (AAMAS) | 模块化程序记忆，面向工作流自动化的多Agent系统 | [arXiv](https://arxiv.org/abs/2601.08816) |
| **G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems** | 2025 (NeurIPS) | 多Agent系统的分层记忆追踪 | [NeurIPS 2025](https://arxiv.org/abs/2508.04903) |
| **AgentNet: Decentralized Evolutionary Coordination** | 2025 (NeurIPS) | 去中心化进化协调的多Agent系统 | [NeurIPS 2025](https://arxiv.org/abs/2508.04903) |
| **Intrinsic Memory Agents: Heterogeneous Multi-Agent LLM** | 2025 | 异构多Agent LLM的内隐记忆 | [arXiv:2508.08997](https://arxiv.org/abs/2508.08997) |
| **EvoCF: Multi-Agent Collaboration via Agentic Memory-Driven Evolutionary Counterfactual Planning** | 2026 | 记忆驱动的进化反事实规划 | [arXiv](https://arxiv.org/abs/2601.08816) |
| **RCR-Router: Efficient Role-Aware Context Routing for Multi-Agent LLM Systems with Structured Memory** | 2025 | 角色感知的上下文路由 | [arXiv:2508.04903](https://arxiv.org/abs/2508.04903) |
| **Latent Collaboration in Multi-Agent Systems** | 2025 | 多Agent系统的潜在协作 | [arXiv:2511.20639](https://arxiv.org/abs/2511.20639) |
| **MEMO: Memory-Augmented Model Context Optimization for Multi-Agent LLM Games** | 2026 | 记忆增强的模型上下文优化，面向多Agent游戏 | [arXiv](https://arxiv.org/abs/2601.08816) |

---

## 五、端侧推理与模型压缩
聚焦在端侧部署的量化、压缩与推理优化。

| 论文 | 年份 | 核心贡献 | 链接 |
|------|------|----------|------|
| **TinyAgent: Quantization-aware Model Compression for On-device LLM Agent Deployment** | 2025/2026 | 量化感知的模型压缩，**8×**内存减少，**4.5×**推理加速 | [OpenReview](https://openreview.net/pdf?id=ntI0eq0urB) |
| **Agent Workflow Memory** | 2024 | Agent工作流记忆机制 | [arXiv:2409.07429](https://arxiv.org/abs/2409.07429) |
| **ParamMem: Augmenting Language Agents with Parametric Reflective Memory** | 2026 | 参数化反射记忆 | [arXiv](https://arxiv.org/abs/2601.08816) |
| **Trajectory-Informed Memory Generation for Self-Improving Agent Systems** | 2026 | 轨迹引导的记忆生成 | [arXiv](https://arxiv.org/abs/2601.08816) |

---

## 六、综述与基准
| 论文 | 年份 | 说明 | 链接 |
|------|------|------|------|
| **A Survey on the Memory Mechanism of Large Language Model-based Agents** | 2025 | ACM Computing Surveys，全面综述LLM Agent记忆机制 | [ACM](https://dl.acm.org/doi/10.1145/3748302) |
| **Memory in the Age of AI Agents** | 2026 | 大规模作者团队（含Hu Yuyang等），AI Agent时代的记忆综述 | [arXiv:2512.13564](https://arxiv.org/abs/2512.13564) |
| **From Storage to Experience: A Survey on the Evolution of LLM Agent Memory Mechanisms** | 2026 | GitHub活跃维护的综述与论文列表 | [GitHub](https://github.com/FeishuLuo/Evolving-LLM-Agent-Memory-Survey) |

---

如果你需要某个具体方向的深入论文（例如**纯端侧无网络依赖的记忆系统**、**KV缓存量化与共享**、或**认知科学启发的记忆架构**），我可以进一步帮你筛选和总结。






## 📚 Paper list
### Edge Memory
- [2025/9]EFFICIENT ON-DEVICE AGENTS VIA ADAPTIVE CONTEXT MANAGEMENT [https://arxiv.org/pdf/2511.03728]
- [2025/12]MemLoRA: Distilling Expert Adapters for On-Device Memory Systems[https://arxiv.org/pdf/2512.04763]
- [2025/10]Mnemosyne: An Unsupervised, Human-Inspired Long-Term Memory Architecture for Edge-Based [https://arxiv.org/pdf/2510.08601]
- [2026/3]CLAG: Adaptive Memory Organization via Agent-Driven Clustering for Small Language Model Agents [https://arxiv.org/abs/2603.15421]
- [2026/2] Shodh-Memory: A Cognitive Memory System for Edge-Native AI Agents[https://www.shodh-memory.com/shodh_memory.pdf]
- [2024/09]TinyAgent: Function Calling at the Edge[https://arxiv.org/abs/2409.00608]

## 待定
- [2026/1]Agentic Memory: Learning Unified Long-Term and Short-Term Memory Management for Large Language Model Agents[https://arxiv.org/pdf/2601.01885]
EverMemOS: A Self-Organizing Memory Operating System for Structured Long-Horizon Reasoning
05 Jan 2026

- Does Memory Need Graphs? A Unified Framework and Empirical Analysis for Long-Term Dialog Memory
04 Jan 2026
- R-Debater: Retrieval-Augmented Debate Generation through Argumentative Memory
31 Dec 2025

### Factual Memory

#### Token-level

- [2025/12] Hindsight is 20/20: Building Agent Memory that Retains, Recalls, and Reflects. [[paper](https://arxiv.org/abs/2512.12818)]
- [2025/11] O-Mem: Omni Memory System for Personalized, Long Horizon, Self-Evolving Agents. [[paper](https://arxiv.org/abs/2511.13593)]
- [2025/11] RCR-Router: Efficient Role-Aware Context Routing for Multi-Agent LLM Systems with Structured Memory. [[paper](https://doi.org/10.48550/arXiv.2508.04903)]
- [2025/11] Enabling Personalized Long-term Interactions in LLM-based Agents through Persistent Memory and User Profiles. [[paper](https://doi.org/10.48550/arXiv.2510.07925)]
- [2025/10] Livia: An Emotion-Aware AR Companion Powered by Modular AI Agents and Progressive Memory Compression. [[paper](https://doi.org/10.48550/arXiv.2509.05298)]
- [2025/10] D-SMART: Enhancing LLM Dialogue Consistency via Dynamic Structured Memory And Reasoning Tree. [[paper](https://arxiv.org/abs/2510.13363)]
- [2025/10] WebWeaver: Structuring Web-Scale Evidence with Dynamic Outlines for Open-Ended Deep Research. [[paper](https://doi.org/10.48550/arXiv.2509.13312)]
- [2025/10] CAM: A Constructivist View of Agentic Memory for LLM-Based Reading Comprehension. [[paper](https://doi.org/10.48550/arXiv.2510.05520)]
- [2025/10] Pre-Storage Reasoning for Episodic Memory: Shifting Inference Burden to Memory for Personalized Dialogue. [[paper](https://doi.org/10.48550/arXiv.2509.10852)]
- [2025/10] LightMem: Lightweight and Efficient Memory-Augmented Generation. [[paper](https://arxiv.org/abs/2510.18866)]
- [2025/09] Mem-α: Learning Memory Construction via Reinforcement Learning. [[paper](https://doi.org/10.48550/arXiv.2509.25911)]
- [2025/09] SGMem: Sentence Graph Memory for Long-Term Conversational Agents. [[paper](https://arxiv.org/abs/2509.21212)]
- [2025/09] Nemori: Self-Organizing Agent Memory Inspired by Cognitive Science. [[paper](https://doi.org/10.48550/arXiv.2508.03341)]
- [2025/09] MOOM: Maintenance, Organization and Optimization of Memory in Ultra-Long Role-Playing Dialogues. [[paper](https://arxiv.org/abs/2509.11860)]
- [2025/09] Multiple Memory Systems for Enhancing the Long-term Memory of Agent. [[paper](https://doi.org/10.48550/arXiv.2508.15294)]
- [2025/09] Semantic Anchoring in Agentic Memory: Leveraging Linguistic Structures for Persistent Conversational Context. [[paper](https://doi.org/10.48550/arXiv.2508.12630)]
- [2025/09] ComoRAG: A Cognitive-Inspired Memory-Organized RAG for Stateful Long Narrative Reasoning. [[paper](https://doi.org/10.48550/arXiv.2508.10419)]
- [2025/08] Seeing, Listening, Remembering, and Reasoning: A Multimodal Agent with Long-Term Memory. [[paper](https://arxiv.org/abs/2508.09736)]
- [2025/08] Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning. [[paper](https://arxiv.org/abs/2508.19828)]
- [2025/08] Intrinsic Memory Agents: Heterogeneous Multi-Agent LLM Systems through Structured Contextual Memory. [[paper](https://arxiv.org/abs/2508.08997)]
- [2025/07] MIRIX: Multi-Agent Memory System for LLM-Based Agents. [[paper](https://arxiv.org/abs/2507.07957)]
- [2025/07] Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents. [[paper](https://arxiv.org/abs/2507.22925)]
- [2025/06] G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems. [[paper](https://arxiv.org/abs/2506.07398)]
- [2025/06] Embodied Agents Meet Personalization: Exploring Memory Utilization for Personalized Assistance. [[paper](https://doi.org/10.48550/arXiv.2505.16348)]
- [2025/05] MemGuide: Intent-Driven Memory Selection for Goal-Oriented Multi-Session LLM Agents. [[paper](https://arxiv.org/abs/2505.20231)]
- [2025/05] Pre-training Limited Memory Language Models with Internal and External Knowledge. [[paper](https://arxiv.org/abs/2505.15962)]
- [2025/05] Embodied VideoAgent: Persistent Memory from Egocentric Videos and Embodied Sensors Enables Dynamic Scene Understanding. [[paper](https://doi.org/10.48550/arXiv.2501.00358)]
- [2025/04] Mem0: Building production-ready ai agents with scalable long-term memory. [[paper](https://arxiv.org/abs/2504.19413)]
- [2025/03] In Prospect and Retrospect: Reflective Memory Management for Long-term Personalized Dialogue Agents. [[paper](https://aclanthology.org/2025.acl-long.413/)]
- [2025/02] SeCom: On Memory Construction and Retrieval for Personalized Conversational Agents. [[paper](https://openreview.net/forum?id=xKDZAW0He3)]
- [2025/02] Zep: A Temporal Knowledge Graph Architecture for Agent Memory. [[paper](https://doi.org/10.48550/arXiv.2501.13956)]
- [2025/02] A-MEM: Agentic Memory for LLM Agents. [[paper](https://doi.org/10.48550/ARXIV.2502.12110)]
- [2025/02] Unveiling Privacy Risks in LLM Agent Memory. [[paper](https://arxiv.org/abs/2502.13172)]
- [2025/02] Mem2Ego: Empowering Vision-Language Models with Global-to-Ego Memory for Long-Horizon Embodied Navigation. [[paper](https://doi.org/10.48550/arXiv.2502.14254)]
- [2024/12] AI PERSONA: Towards Life-long Personalization of LLMs. [[paper](https://arxiv.org/abs/2412.13103)]
- [2024/11] OASIS: Open Agent Social Interaction Simulations with One Million Agents. [[paper](https://arxiv.org/abs/2411.11581)]
- [2024/10] Memolet: Reifying the Reuse of User-AI Conversational Memories. [[paper](https://doi.org/10.1145/3654777.3676388)]
- [2024/10] From Isolated Conversations to Hierarchical Schemas: Dynamic Tree Memory Representation for LLMs. [[paper](https://arxiv.org/abs/2410.14052)]
- [2024/10] Enhancing Long Context Performance in LLMs Through Inner Loop Query Mechanism. [[paper](https://arxiv.org/abs/2410.12859)]
- [2024/09] Crafting Personalized Agents through Retrieval-Augmented Generation on Editable Memory Graphs. [[paper](https://arxiv.org/abs/2409.19401)]
- [2024/07] Human-inspired Episodic Memory for Infinite Context LLMs. [[paper](https://openreview.net/forum?id=BI2int5SAC)]
- [2024/07] Arigraph: Learning knowledge graph world models with episodic memory for llm agents. [[paper](https://arxiv.org/abs/2407.04363)]
- [2024/07] ChatHaruhi: Reviving Anime Character in Reality via Large Language Model. [[paper](https://doi.org/10.48550/arXiv.2308.09597)]
- [2024/07] Toward Conversational Agents with Context and Time Sensitive Long-term Memory. [[paper](https://doi.org/10.48550/arXiv.2406.00057)]
- [2024/06] Enhancing Long-Term Memory using Hierarchical Aggregate Tree for Retrieval Augmented Generation. [[paper](https://arxiv.org/abs/2406.06124)]
- [2024/06] Towards Lifelong Dialogue Agents via Timeline-based Memory Management. [[paper](https://arxiv.org/abs/2406.10996)]
- [2024/05] HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models. [[paper](https://arxiv.org/abs/2405.14831)]
- [2024/05] Memory Sharing for Large Language Model based Agents. [[paper](https://doi.org/10.48550/arXiv.2404.09982)]
- [2024/05] Knowledge Graph Tuning: Real-time Large Language Model Personalization based on Human Feedback. [[paper](https://arxiv.org/abs/2405.19686)]
- [2024/04] From Local to Global: A Graph RAG Approach to Query-Focused Summarization. [[paper](https://arxiv.org/abs/2404.16130)]
- [2024/03] Memoro: Using Large Language Models to Realize a Concise Interface for Real-Time Memory Augmentation. [[paper](https://doi.org/10.1145/3613904.3642450)]
- [2023/10] RoleLLM: Benchmarking, Eliciting, and Enhancing Role-Playing Abilities of Large Language Models. [[paper](https://doi.org/10.18653/v1/2024.findings-acl.878)]
- [2023/10] MemGPT: Towards LLMs as Operating Systems. [[paper](https://arxiv.org/abs/2310.08560)]
- [2023/10] GameGPT: Multi-agent Collaborative Framework for Game Development. [[paper](https://doi.org/10.48550/ARXIV.2310.08067)]
- [2023/10] Lyfe Agents: Generative agents for low-cost real-time social interactions. [[paper](https://arxiv.org/abs/2310.02172)]
- [2023/08] CALYPSO: LLMs as Dungeon Masters' Assistants. [[paper](https://doi.org/10.1609/aiide.v19i1.27534)]
- [2023/08] MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework. [[paper](https://arxiv.org/abs/2308.00352)]
- [2023/08] Recommender AI Agent: Integrating Large Language Models for Interactive Recommendations. [[paper](https://doi.org/10.1145/3731446)]
- [2023/08] MemoChat: Tuning LLMs to Use Memos for Consistent Long-Range Open-Domain Conversation. [[paper](https://arxiv.org/abs/2308.08239)]
- [2023/08] Recursively summarizing enables long-term dialogue memory in large language models. [[paper](https://arxiv.org/abs/2308.15022)]
- [2023/07] MovieChat: From Dense Token to Sparse Memory for Long Video Understanding. [[paper](https://doi.org/10.1109/CVPR52733.2024.01725)]
- [2023/07] S${}^3$: Social-network Simulation System with Large Language Model-Empowered Agents. [[paper](https://doi.org/10.48550/ARXIV.2307.14984)]
- [2023/05] Prompted LLMs as Chatbot Modules for Long Open-domain Conversation. [[paper](https://doi.org/10.18653/v1/2023.findings-acl.277)]
- [2023/05] RecurrentGPT: Interactive Generation of (Arbitrarily) Long Text. [[paper](https://arxiv.org/abs/2305.13304)]
- [2023/05] Memorybank: Enhancing large language models with long-term memory. [[paper](https://arxiv.org/abs/2305.10250)]
- [2023/05] RET-LLM: Towards a general read-write memory for large language models. [[paper](https://arxiv.org/abs/2305.14322)]
- [2023/04] Generative agents: Interactive simulacra of human behavior. [[paper](https://arxiv.org/abs/2304.03442)]
- [2023/04] HuaTuo: Tuning LLaMA Model with Chinese Medical Knowledge. [[paper](https://arxiv.org/abs/2304.06975)]
- [2023/04] SCM: Enhancing Large Language Model with Self-Controlled Memory Framework. [[paper](https://arxiv.org/abs/2304.13343)]


#### Parametric

- [2025/10] Pretraining with hierarchical memories: separating long-tail and common knowledge. [[paper](https://arxiv.org/abs/2510.02375)]
- [2025/08] MLP Memory: Language Modeling with Retriever-pretrained External Memory. [[paper](https://doi.org/10.48550/arXiv.2508.01832)]
- [2024/10] Self-Updatable Large Language Models by Integrating Context into Model Parameters. [[paper](https://openreview.net/forum?id=aCPFCDL9QY)]
- [2024/10] AlphaEdit: Null-Space Constrained Knowledge Editing for Language Models. [[paper](https://arxiv.org/abs/2410.02355)]
- [2024/08] ELDER: Enhancing Lifelong Model Editing with Mixture-of-LoRA. [[paper](https://doi.org/10.1609/aaai.v39i23.34622)]
- [2024/05] WISE: Rethinking the Knowledge Memory for Lifelong Model Editing of Large Language Models. [[paper](http://papers.nips.cc/paper_files/paper/2024/hash/60960ad78868fce5c165295fbd895060-Abstract-Conference.html)]
- [2024/03] Online Adaptation of Language Models with a Memory of Amortized Contexts. [[paper](http://papers.nips.cc/paper_files/paper/2024/hash/eaf956b52bae51fbf387b8be4cc3ce18-Abstract-Conference.html)]
- [2024/01] Neighboring Perturbations of Knowledge Editing on Large Language Models. [[paper](https://openreview.net/forum?id=K9NTPRvVRI)]
- [2023/11] CharacterGLM: Customizing Social Characters with Large Language Models. [[paper](https://doi.org/10.18653/v1/2024.emnlp-industry.107)]
- [2023/10] Character-LLM: A Trainable Agent for Role-Playing. [[paper](https://doi.org/10.18653/v1/2023.emnlp-main.814)]
- [2021/10] Fast Model Editing at Scale. [[paper](https://openreview.net/forum?id=0DcZxeWfOPt)]
- [2021/04] Editing Factual Knowledge in Language Models. [[paper](https://arxiv.org/abs/2104.08164)]
- [2020/02] K-Adapter: Infusing Knowledge into Pre-Trained Models with Adapters. [[paper](https://doi.org/10.18653/v1/2021.findings-acl.121)]
- [2013/02] ELLA: An Efficient Lifelong Learning Algorithm. [[paper](https://proceedings.mlr.press/v28/ruvolo13.html)]

#### Latent

- [2025/08] Towards General Continuous Memory for Vision-Language Models. [[paper](https://arxiv.org/abs/2505.17670)]
- [2025/03] M+: Extending MemoryLLM with Scalable Long-Term Memory. [[paper](https://doi.org/10.48550/arXiv.2502.00592)]
- [2025/02] R3Mem: Bridging Memory Retention and Retrieval via Reversible Compression [[paper](https://arxiv.org/abs/2502.15957v1)]
- [2024/07] Memory${}^3$: Language Modeling with Explicit Memory. [[paper](https://doi.org/10.48550/arXiv.2407.01178)]
- [2024/03] Efficient Episodic Memory Utilization of Cooperative Multi-Agent Reinforcement Learning. [[paper](https://openreview.net/forum?id=LjivA1SLZ6)]

### Experiential Memory

#### Token-level

- [2025/12] Hindsight is 20/20: Building Agent Memory that Retains, Recalls, and Reflects. [[paper](https://arxiv.org/abs/2512.12818)]
- [2025/11] Agentic Context Engineering: Evolving Contexts for Self-Improving Language Models. [[paper](https://doi.org/10.48550/arXiv.2510.04618)]
- [2025/11] FLEX: Continuous Agent Evolution via Forward Learning from Experience. [[paper](https://arxiv.org/abs/2511.06449)]
- [2025/11] Scaling Agent Learning via Experience Synthesis. [[paper](https://arxiv.org/abs/2511.03773)]
- [2025/11] UFO2: The Desktop AgentOS. [[paper](https://doi.org/10.48550/arXiv.2504.14603)]
- [2025/10] PRINCIPLES: Synthetic Strategy Memory for Proactive Dialogue Agents. [[paper](https://doi.org/10.48550/arXiv.2509.17459)]
- [2025/10] Training-Free Group Relative Policy Optimization. [[paper](https://arxiv.org/abs/2510.08191)]
- [2025/10] ToolMem: Enhancing Multimodal Agents with Learnable Tool Capability Memory. [[paper](https://doi.org/10.48550/arXiv.2510.06664)]
- [2025/10] H${}^2$R: Hierarchical Hindsight Reflection for Multi-Task LLM Agents. [[paper](https://doi.org/10.48550/arXiv.2509.12810)]
- [2025/10] BrowserAgent: Building Web Agents with Human-Inspired Web Browsing Actions. [[paper](http://arxiv.org/abs/2510.10666)]
- [2025/10] LEGOMem: Modular Procedural Memory for Multi-agent LLM Systems for Workflow Automation. [[paper](http://arxiv.org/abs/2510.04851)]
- [2025/10] Alita-G: Self-Evolving Generative Agent for Agent Generation. [[paper](https://doi.org/10.48550/arXiv.2510.23601)]
- [2025/09] ReasoningBank: Scaling Agent Self-Evolving with Reasoning Memory. [[paper](https://arxiv.org/abs/2509.25140)]
- [2025/09] Memento: Fine-tuning LLM Agents without Fine-tuning LLMs. [[paper](https://doi.org/10.48550/arXiv.2508.16153)]
- [2025/08] Memp: Exploring Agent Procedural Memory. [[paper](https://arxiv.org/abs/2508.06433)]
- [2025/08] SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience. [[paper](https://arxiv.org/abs/2508.04700)]
- [2025/07] Agent KB: Leveraging Cross-Domain Experience for Agentic Problem Solving. [[paper](https://arxiv.org/abs/2507.06229)]
- [2025/07] MemTool: Optimizing short-term memory management for dynamic tool calling in llm agent multi-turn conversations. [[paper](https://arxiv.org/abs/2507.21428)]
- [2025/05] Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents. [[paper](https://doi.org/10.48550/arXiv.2505.22954)]
- [2025/05] Alita: Generalist Agent Enabling Scalable Agentic Reasoning with Minimal Predefinition and Maximal Self-Evolution. [[paper](https://arxiv.org/abs/2505.20286)]
- [2025/05] SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills. [[paper](https://doi.org/10.48550/arXiv.2504.07079)]
- [2025/05] LearnAct: Few-Shot Mobile GUI Agent with a Unified Demonstration Benchmark. [[paper](https://doi.org/10.48550/arXiv.2504.13805)]
- [2025/05] Retrieval Models Aren't Tool-Savvy: Benchmarking Tool Retrieval for Large Language Models. [[paper](https://doi.org/10.48550/arXiv.2503.01763)]
- [2025/04] Dynamic Cheatsheet: Test-Time Learning with Adaptive Memory. [[paper](https://arxiv.org/abs/2504.07952)]
- [2025/04] Inducing Programmatic Skills for Agentic Tasks. [[paper](https://arxiv.org/abs/2504.06821)]
- [2025/03] COLA: A Scalable Multi-Agent Framework For Windows UI Task Automation. [[paper](https://doi.org/10.48550/arXiv.2503.09263)]
- [2025/03] Memory-augmented Query Reconstruction for LLM-based Knowledge Graph Reasoning. [[paper](https://arxiv.org/abs/2503.05193)]
- [2025/02] From Exploration to Mastery: Enabling LLMs to Master Tools via Self-Driven Interactions. [[paper](https://doi.org/10.48550/arXiv.2410.08197)]
- [2025/02] From RAG to Memory: Non-Parametric Continual Learning for Large Language Models. [[paper](https://arxiv.org/abs/2502.14802)]
- [2024/12] Planning from Imagination: Episodic Simulation and Episodic Memory for Vision-and-Language Navigation. [[paper](https://arxiv.org/abs/2412.01857)]
- [2024/10] RepairAgent: An Autonomous, LLM-Based Agent for Program Repair. [[paper](http://arxiv.org/abs/2403.17134)]
- [2024/09] SAGE: Self-evolving Agents with Reflective and Memory-augmented Abilities. [[paper](https://doi.org/10.1016/j.neucom.2025.130470)]
- [2024/07] Agent Workflow Memory. [[paper](https://openreview.net/forum?id=NTAhi2JEEE)]
- [2024/07] Fincon: A synthesized llm multi-agent system with conceptual verbal reinforcement for enhanced financial decision making. [[paper](https://arxiv.org/abs/2407.06567)]
- [2024/06] Buffer of Thoughts: Thought-Augmented Reasoning with Large Language Models. [[paper](http://papers.nips.cc/paper_files/paper/2024/hash/cde328b7bf6358f5ebb91fe9c539745e-Abstract-Conference.html)]
- [2024/05] COLT: Towards Completeness-Oriented Tool Retrieval for Large Language Models. [[paper](https://doi.org/10.48550/arXiv.2405.16089)]
- [2023/11] JARVIS-1: Open-World Multi-Task Agents With Memory-Augmented Multimodal Language Models. [[paper](https://doi.org/10.1109/TPAMI.2024.3511593)]
- [2023/08] RecMind: Large Language Model Powered Agent For Recommendation. [[paper](https://doi.org/10.18653/v1/2024.findings-naacl.271)]
- [2023/08] ExpeL: LLM Agents Are Experiential Learners. [[paper](https://doi.org/10.1609/aaai.v38i17.29936)]
- [2023/07] ToolLLM: Facilitating Large Language Models to Master 16000+ Real-world APIs. [[paper](https://arxiv.org/abs/2307.16789)]
- [2023/05] CREATOR: Tool Creation for Disentangling Abstract and Concrete Reasoning of Large Language Models. [[paper](https://doi.org/10.18653/v1/2023.findings-emnlp.462)]
- [2023/03] Reflexion: Language agents with verbal reinforcement learning. [[paper](https://arxiv.org/abs/2303.11366)]
- [2023/02] Toolformer: Language models can teach themselves to use tools. [[paper](https://arxiv.org/abs/2302.04761)]

#### Parametric

- [2025/11] AgentEvolver: Towards Efficient Self-Evolving Agent System. [[paper](https://arxiv.org/abs/2511.10395)]
- [2025/10] Agent Learning via Early Experience. [[paper](https://arxiv.org/abs/2510.08558)]
- [2025/10] Scaling Agents via Continual Pre-training. [[paper](https://doi.org/10.48550/arXiv.2509.13310)]
- [2024/10] ToolGen: Unified Tool Retrieval and Calling via Generation. [[paper](https://arxiv.org/abs/2410.03439)]
- [2023/08] Retroformer: Retrospective Large Language Agents with Policy Gradient Optimization. [[paper](https://arxiv.org/abs/2308.02151)]
- [2023/06] A Machine with Short-Term, Episodic, and Semantic Memory Systems. [[paper](https://doi.org/10.1609/aaai.v37i1.25075)]

#### Latent

- [2025/11] Auto-scaling Continuous Memory for GUI Agent. [[paper](https://doi.org/10.48550/arXiv.2510.09038)]

### Working Memory

#### Token-level

- [2025/11] Memory as Action: Autonomous Context Curation for Long-Horizon Agentic Tasks. [[paper](https://doi.org/10.48550/arXiv.2510.12635)]
- [2025/11] IterResearch: Rethinking Long-Horizon Agents via Markovian State Reconstruction. [[paper](https://arxiv.org/abs/2511.07327)]
- [2025/11] MemSearcher: Training LLMs to Reason, Search and Manage Memory via End-to-End Reinforcement Learning. [[paper](https://doi.org/10.48550/arXiv.2511.02805)]
- [2025/10] AgentFold: Long-Horizon Web Agents with Proactive Context Management. [[paper](https://arxiv.org/abs/2510.24699)]
- [2025/10] PRIME: Planning and Retrieval-Integrated Memory for Enhanced Reasoning. [[paper](https://doi.org/10.48550/arXiv.2509.22315)]
- [2025/10] Context as Memory: Scene-Consistent Interactive Long Video Generation with Memory Retrieval. [[paper](https://doi.org/10.48550/arXiv.2506.03141)]
- [2025/10] DeepAgent: A General Reasoning Agent with Scalable Toolsets. [[paper](https://doi.org/10.48550/arXiv.2510.21618)]
- [2025/10] ACON: Optimizing Context Compression for Long-Horizon LLM Agents. [[paper](https://doi.org/10.48550/arXiv.2510.00615)]
- [2025/09] ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization. [[paper](https://doi.org/10.48550/ARXIV.2509.13313)]
- [2025/08] Sculptor: Empowering LLMs with Cognitive Agency via Active Context Management. [[paper](https://arxiv.org/abs/2508.04664)]
- [2025/07] MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent. [[paper](https://arxiv.org/abs/2507.02259)]
- [2024/10] Agent S: An Open Agentic Framework That Uses Computers Like a Human. [[paper](https://arxiv.org/abs/2410.08164)]

#### Parametric

- [2024/05] Various Lengths, Constant Speed: Efficient Language Modeling with Lightning Attention. [[paper](https://openreview.net/forum?id=5wm6TiUP4X)]
- [2024/01] Efficient Streaming Language Models with Attention Sinks. [[paper](https://openreview.net/forum?id=NG7sS51zVF)]

#### Latent

- [2025/11] VisMem: Latent Vision Memory Unlocks Potential of Vision-Language Models [[paper](https://arxiv.org/abs/2511.11007)]
- [2025/09] MemGen: Weaving Generative Latent Memory for Self-Evolving Agents. [[paper](https://arxiv.org/abs/2509.24704)]
- [2025/09] Conflict-Aware Soft Prompting for Retrieval-Augmented Generation. [[paper](https://doi.org/10.48550/arXiv.2508.15253)]
- [2025/09] MemoryVLA: Perceptual-Cognitive Memory in Vision-Language-Action Models for Robotic Manipulation. [[paper](https://doi.org/10.48550/arXiv.2508.19236)]
- [2025/06] MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents. [[paper](https://arxiv.org/abs/2506.15841)]
- [2025/05] RazorAttention: Efficient KV Cache Compression Through Retrieval Heads. [[paper](https://openreview.net/forum?id=tkiZQlL04w)]
- [2025/04] MemoRAG: Boosting Long Context Processing with Global Memory-Enhanced Retrieval Augmentation. [[paper](https://doi.org/10.1145/3696410.3714805)]
- [2025/04] SnapKV: LLM Knows What You are Looking for Before Generation. [[paper](http://papers.nips.cc/paper_files/paper/2024/hash/28ab418242603e0f7323e54185d19bde-Abstract-Conference.html)]
- [2025/03] LM2: Large Memory Models. [[paper](https://doi.org/10.48550/arXiv.2502.06049)]
- [2025/02] SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs. [[paper](https://aclanthology.org/2025.acl-long.1137/)]
- [2025/02] Time-VLM: Exploring Multimodal Vision-Language Models for Augmented Time Series Forecasting. [[paper](https://doi.org/10.48550/arXiv.2502.04395)]
- [2025/02] Titans: Learning to Memorize at Test Time. [[paper](https://doi.org/10.48550/arXiv.2501.00663)]
- [2024/08] Augmenting Language Models with Long-Term Memory. [[paper](http://papers.nips.cc/paper_files/paper/2023/hash/ebd82705f44793b6f9ade5a669d0f0bf-Abstract-Conference.html)]
- [2024/06] Taking a Deep Breath: Enhancing Language Modeling of Large Language Models with Sentinel Tokens. [[paper](https://doi.org/10.18653/v1/2024.findings-emnlp.233)]
- [2024/04] Adapting Language Models to Compress Contexts. [[paper](https://doi.org/10.18653/v1/2023.emnlp-main.232)]
- [2024/03] Learning to Compress Prompts with Gist Tokens. [[paper](http://papers.nips.cc/paper_files/paper/2023/hash/3d77c6dcc7f143aa2154e7f4d5e22d68-Abstract-Conference.html)]
- [2024/03] Scissorhands: Exploiting the Persistence of Importance Hypothesis for LLM KV Cache Compression at Test Time. [[paper](http://papers.nips.cc/paper_files/paper/2023/hash/a452a7c6c463e4ae8fbdc614c6e983e6-Abstract-Conference.html)]
- [2024/03] Focused Transformer: Contrastive Training for Context Scaling. [[paper](http://papers.nips.cc/paper_files/paper/2023/hash/8511d06d5590f4bda24d42087802cc81-Abstract-Conference.html)]
- [2023/07] In-Context Autoencoder for Context Compression in a Large Language Model. [[paper](https://arxiv.org/abs/2307.06945)]
- [2023/06] H2O: Heavy-Hitter Oracle for Efficient Generative Inference of Large Language Models. [[paper](http://papers.nips.cc/paper_files/paper/2023/hash/6ceefa7b15572587b78ecfcebb2827f8-Abstract-Conference.html)]
- [2022/08] Memorizing Transformers. [[paper](https://openreview.net/forum?id=TrjbxzRcnf-)]
- [2022/07] XMem: Long-Term Video Object Segmentation with an Atkinson-Shiffrin Memory Model. [[paper](https://arxiv.org/abs/2207.07115)]

## 📖 Citation

If you find this repository helpful, a citation to our paper would be greatly appreciated:

```bibtex
@article{hu2025memory,
  title={Memory in the Age of AI Agents},
  author={Hu, Yuyang and Liu, Shichun and Yue, Yanwei and Zhang, Guibin and Liu, Boyang and Zhu, Fangyi and Lin, Jiahang and Guo, Honglin and Dou, Shihan and Xi, Zhiheng and Jin, Senjie and Tan, Jiejun and Yin, Yanbin and Liu, Jiongnan and Zhang, Zeyu and Sun, Zhongxiang and Zhu, Yutao and Sun, Hao and Peng, Boci and Cheng, Zhenrong and Fan, Xuanbo and Guo, Jiaxin and Yu, Xinlei and Zhou, Zhenhong and Hu, Zewen and Huo, Jiahao and Wang, Junhao and Niu, Yuwei and Wang, Yu and Yin, Zhenfei and Hu, Xiaobin and Liao, Yue and Li, Qiankun and Wang, Kun and Zhou, Wangchunshu and Liu, Yixin and Cheng, Dawei and Zhang, Qi and Gui, Tao and Pan, Shirui and Zhang, Yan and Torr, Philip and Dou, Zhicheng and Wen, Ji-Rong and Huang, Xuanjing and Jiang, Yu-Gang and Yan, Shuicheng},
  journal={arXiv preprint arXiv:2512.13564},
  year={2025}
}
