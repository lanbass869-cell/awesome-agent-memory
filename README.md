# Awesome Agent Memory

A curated taxonomy of **agent memory systems**, organized along four axes: (1) memory system architectures — from flat sequential context, to structural topological graphs/trees, to multi-paradigm hybrid containers; (2) reference baselines for comparison; (3) benchmarks for evaluation; and (4) surveys on agent memory.

## 📣 Get Involved

- 📊 **Looking for a testbed to evaluate agent memory systems?** See our companion repo [OpenDataBox/MemoryData](https://github.com/OpenDataBox/MemoryData) — an integrated platform of memory systems and datasets.
- 📌 **Missing a paper, method, or benchmark?** [Open an issue](https://github.com/OpenDataBox/awesome-agent-memory/issues/new) to request it.
- 🤝 **Want to contribute directly?** [Submit a Pull Request](https://github.com/OpenDataBox/awesome-agent-memory/compare) — community PRs are warmly welcomed!

![](AgentMemory.png)

## Table of Contents

- [1. Memory Systems and Methods](#1-memory-systems-and-methods)
  - [1.1 Sequential Memory Systems](#11-sequential-memory-systems)
    - [1.1.1 Discrete Textual Memory](#111-discrete-textual-memory)
    - [1.1.2 Parameter and Latent Memory](#112-parameter-and-latent-memory)
  - [1.2 Structured Topological Memory Systems](#12-structured-topological-memory-systems)
    - [1.2.1 Graph-Based Memory](#121-graph-based-memory)
    - [1.2.2 Hierarchical Memory](#122-hierarchical-memory)
  - [1.3 Composite Memory Systems](#13-composite-memory-systems)
  - [1.4 Baselines and Supporting Methods](#14-baselines-and-supporting-methods)
- [2. Benchmarks and Datasets](#2-benchmarks-and-datasets)
  - [2.1 Effectiveness Evaluation](#21-effectiveness-evaluation)
  - [2.2 Retrieval Evaluation](#22-retrieval-evaluation)
  - [2.3 Robustness Evaluation](#23-robustness-evaluation)
  - [2.4 Efficiency Evaluation](#24-efficiency-evaluation)
- [3. Surveys, Tutorials, and Position Papers](#3-surveys-tutorials-and-position-papers)
- [4. Frameworks, Products, and Resources](#4-frameworks-products-and-resources)
- [Citation](#citation)

## 1. Memory Systems and Methods

### 1.1 Sequential Memory Systems

#### 1.1.1 Discrete Textual Memory

Memory represented as a flat sequence, textual summary, note, trajectory, or experience record without an explicit graph or tree topology.

1. **MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent**\
   Hongli Yu, Tinghong Chen, Jiangtao Feng, et al. *ICLR 2026*. [[Paper](https://arxiv.org/abs/2507.02259)] [[Code](https://github.com/BytedTsinghua-SIA/MemAgent)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-RL_based-orange)

1. **🆕 Agent Workflow Memory**\
   Zora Zhiruo Wang, Jiayuan Mao, Daniel Fried, Graham Neubig. *ICML 2025*. [[Paper](https://arxiv.org/abs/2409.07429)] [[Code](https://github.com/zorazrw/agent-workflow-memory)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Procedural-yellowgreen) ![](https://img.shields.io/badge/-Prompt_based-orange)

1. **🆕 Compress to Impress: Unleashing the Potential of Compressive Memory in Real-World Long-Term Conversations**\
   Nuo Chen, Hongguang Li, Jianhui Chang, et al. *COLING 2025*. [[Paper](https://arxiv.org/abs/2402.11975)] [[Code](https://github.com/nuochenpku/COMEDY)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Compression-orange)

1. **🆕 ExpeL: LLM Agents Are Experiential Learners**\
   Andrew Zhao, Daniel Huang, Quentin Xu, et al. *AAAI 2024*. [[Paper](https://arxiv.org/abs/2308.10144)] [[Code](https://github.com/LeapLabTHU/ExpeL)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Procedural-yellowgreen) ![](https://img.shields.io/badge/-Training_free-orange)

1. **MemoryBank: Enhancing Large Language Models with Long-Term Memory**\
   Wanjun Zhong, Lianghong Guo, Qiqi Gao, et al. *AAAI 2024*. [[Paper](https://arxiv.org/abs/2305.10250)] [[Code](https://github.com/zhongwanjun/MemoryBank-SiliconFriend)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Semantic-green)

1. **🆕 Generative Agents: Interactive Simulacra of Human Behavior**\
   Joon Sung Park, Joseph C. O'Brien, Carrie J. Cai, et al. *UIST 2023*. [[Paper](https://arxiv.org/abs/2304.03442)] [[Code](https://github.com/joonspk-research/generative_agents)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Reflection-yellowgreen)

1. **MemoChat: Tuning LLMs to Use Memos for Consistent Long-Range Open-Domain Conversation**\
   Junru Lu, Siyu An, Mingbao Lin, et al. *arXiv 2023*. [[Paper](https://arxiv.org/abs/2308.08239)] [[Code](https://github.com/LuJunru/MemoChat)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-SFT-orange)

1. **🆕 RET-LLM: Towards a General Read-Write Memory for Large Language Models**\
   Ali Modarressi, Ayyoob Imani, Mohsen Fayyaz, Hinrich Schütze. *arXiv 2023*. [[Paper](https://arxiv.org/abs/2305.14322)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Read_Write-orange)

[⬆️ top](#table-of-contents)

#### 1.1.2 Parameter and Latent Memory

Memory stored in model parameters, learned memory modules, hidden states, attention key-values, or other continuous latent representations.

1. **MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents**\
   Zijian Zhou, Ao Qu, Zhaoxuan Wu, et al. *ICLR 2026*. [[Paper](https://arxiv.org/abs/2506.15841)] [[Code](https://github.com/MIT-MI/MEM1)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Internal-orange) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-RL_based-orange)

1. **MemoRAG: Boosting Long Context Processing with Global Memory-Enhanced Retrieval Augmentation**\
   Hongjin Qian, Zheng Liu, Peitian Zhang, et al. *WWW 2025*. [[Paper](https://arxiv.org/abs/2409.05591)] [[Code](https://github.com/qhjqhj00/MemoRAG)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Retrieval-green)

1. **🆕 WISE: Rethinking the Knowledge Memory for Lifelong Model Editing of Large Language Models**\
   Peng Wang, Zexi Li, Ningyu Zhang, et al. *NeurIPS 2024*. [[Paper](https://arxiv.org/abs/2405.14768)] [[Code](https://github.com/zjunlp/EasyEdit)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Internal-orange) ![](https://img.shields.io/badge/-Parameter-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Model_Editing-orange)

1. **🆕 InfLLM: Training-Free Long-Context Extrapolation for LLMs with an Efficient Context Memory**\
   Chaojun Xiao, Pengle Zhang, Xu Han, et al. *NeurIPS 2024*. [[Paper](https://arxiv.org/abs/2402.04617)] [[Code](https://github.com/thunlp/InfLLM)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-Training_free-orange)

1. **🆕 Memory³: Language Modeling with Explicit Memory**\
   Hongkang Yang, Zehao Lin, Wenjin Wang, et al. *Journal of Machine Learning 2024*. [[Paper](https://arxiv.org/abs/2407.01178)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Explicit_Memory-purple)

1. **🆕 Larimar: Large Language Models with Episodic Memory Control**\
   Payel Das, Subhajit Chaudhury, Elliot Nelson, et al. *ICML 2024*. [[Paper](https://arxiv.org/abs/2403.11901)] [[Code](https://github.com/IBM/larimar)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Internal-orange) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Model_Editing-orange)

1. **🆕 MEMORYLLM: Towards Self-Updatable Large Language Models**\
   Yu Wang, Yifan Gao, Xiusi Chen, et al. *ICML 2024*. [[Paper](https://arxiv.org/abs/2402.04624)] [[Code](https://github.com/wangyu-ustc/MemoryLLM)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Internal-orange) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Self_Updating-orange)

1. **🆕 Efficient Streaming Language Models with Attention Sinks**\
   Guangxuan Xiao, Yuandong Tian, Beidi Chen, et al. *ICLR 2024*. [[Paper](https://arxiv.org/abs/2309.17453)] [[Code](https://github.com/mit-han-lab/streaming-llm)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Internal-orange) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-KV_Cache-purple)

1. **🆕 Augmenting Language Models with Long-Term Memory**\
   Weizhi Wang, Li Dong, Hao Cheng, et al. *NeurIPS 2023*. [[Paper](https://arxiv.org/abs/2306.07174)] [[Code](https://github.com/Victorwz/LongMem)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Retrieval-green)

1. **🆕 Memorizing Transformers**\
   Yuhuai Wu, Markus N. Rabe, DeLesley Hutchins, Christian Szegedy. *ICLR 2022 Spotlight*. [[Paper](https://arxiv.org/abs/2203.08913)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Latent-purple) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-kNN_Memory-purple)

[⬆️ top](#table-of-contents)

### 1.2 Structured Topological Memory Systems

#### 1.2.1 Graph-Based Memory

Memory organized as entities, relations, notes, events, or episodes connected by explicit graph edges.

1. **A-MEM: Agentic Memory for LLM Agents**\
   Wujiang Xu, Zujie Liang, Kai Mei, et al. *NeurIPS 2025*. [[Paper](https://arxiv.org/abs/2502.12110)] [[Code](https://github.com/agiresearch/A-mem)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Semantic-green)

1. **🆕 AriGraph: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents**\
   Petr Anokhin, Nikita Semenov, Artyom Sorokin, et al. *IJCAI 2025*. [[Paper](https://arxiv.org/abs/2407.04363)] [[Code](https://github.com/AIRI-Institute/AriGraph)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-World_Model-purple)

1. **From RAG to Memory: Non-Parametric Continual Learning for Large Language Models**\
   Bernal Jiménez Gutiérrez, Yiheng Shu, Weijian Qi, et al. *ICML 2025*. [[Paper](https://arxiv.org/abs/2502.14802)] [[Code](https://github.com/OSU-NLP-Group/HippoRAG)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Continual_Learning-orange)

1. **🆕 MemLLM: Finetuning LLMs to Use An Explicit Read-Write Memory**\
   Ali Modarressi, Abdullatif Köksal, Ayyoob Imani, et al. *TMLR 2025*. [[Paper](https://arxiv.org/abs/2404.11672)] [[Code](https://github.com/amodaresi/MemLLM)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-SFT-orange)

1. **Zep: A Temporal Knowledge Graph Architecture for Agent Memory**\
   Preston Rasmussen, Pavlo Paliychuk, Travis Beauvais, Jack Ryan. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2501.13956)] [[Code](https://github.com/getzep/graphiti)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Temporal-orange)

1. **🆕 On the Structural Memory of LLM Agents**\
   Ruihong Zeng, Jinyuan Fang, Siwei Liu, Zaiqiao Meng. *arXiv 2024*. [[Paper](https://arxiv.org/abs/2412.15266)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Multi_Hop-blue)

1. **HippoRAG: Neurobiologically Inspired Long-Term Memory for Large Language Models**\
   Bernal Jiménez Gutiérrez, Yiheng Shu, Yu Gu, et al. *NeurIPS 2024*. [[Paper](https://arxiv.org/abs/2405.14831)] [[Code](https://github.com/OSU-NLP-Group/HippoRAG)] [[Dataset](https://github.com/OSU-NLP-Group/HippoRAG)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Training_free-orange)

1. **🆕 Crafting Personalized Agents through Retrieval-Augmented Generation on Editable Memory Graphs**\
   Zheng Wang, Zhongyang Li, Zeren Jiang, et al. *EMNLP 2024*. [[Paper](https://arxiv.org/abs/2409.19401)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Personalization-green)

[⬆️ top](#table-of-contents)

#### 1.2.2 Hierarchical Memory

Memory organized across levels, layers, trees, subgoals, or progressively abstracted summaries.

1. **🆕 HiAgent: Hierarchical Working Memory Management for Solving Long-Horizon Agent Tasks with Large Language Model**\
   Mengkang Hu, Tianxing Chen, Qiguang Chen, et al. *ACL 2025*. [[Paper](https://aclanthology.org/2025.acl-long.1575/)] [[Code](https://github.com/HiAgent2024/HiAgent)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-Long_Horizon-purple)

1. **🆕 G-Memory: Tracing Hierarchical Memory for Multi-Agent Systems**\
   Guibin Zhang, Muxin Fu, Guancheng Wan, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2506.07398)] [[Code](https://github.com/bingreeky/GMemory)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Procedural-yellowgreen) ![](https://img.shields.io/badge/-Multi_Agent-purple)

1. **From Isolated Conversations to Hierarchical Schemas: Dynamic Tree Memory Representation for LLMs**\
   Alireza Rezazadeh, Zichao Li, Wei Wei, Yujia Bao. *ICLR 2025*. [[Paper](https://arxiv.org/abs/2410.14052)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Tree_Memory-purple)

1. **🆕 Enhancing Long-Term Memory using Hierarchical Aggregate Tree for Retrieval Augmented Generation**\
   Aadharsh Aadhithya A, Sachin Kumar S, Soman K. P. *arXiv 2024*. [[Paper](https://arxiv.org/abs/2406.06124)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Tree_Memory-purple)

1. **🆕 RAPTOR: Recursive Abstractive Processing for Tree-Organized Retrieval**\
   Parth Sarthi, Salman Abdullah, Aditi Tuli, et al. *ICLR 2024*. [[Paper](https://arxiv.org/abs/2401.18059)] [[Code](https://github.com/parthsarthi03/raptor)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Semantic-green) ![](https://img.shields.io/badge/-Retrieval-green)

1. **🆕 FinMem: A Performance-Enhanced LLM Trading Agent with Layered Memory and Character Design**\
   Yangyang Yu, Haohang Li, Zhi Chen, et al. *arXiv 2023*. [[Paper](https://arxiv.org/abs/2311.13743)] [[Code](https://github.com/pipiku915/FinMem-LLM-StockTrading)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Domain_Agent-purple)

[⬆️ top](#table-of-contents)

### 1.3 Composite Memory Systems

Systems combining multiple memory representations, stores, modalities, time scales, or operating-system-like management policies.

1. **LightMem: Lightweight and Efficient Memory-Augmented Generation**\
   Jizhan Fang, Xinle Deng, Haoming Xu, et al. *ICLR 2026*. [[Paper](https://arxiv.org/abs/2510.18866)] [[Code](https://github.com/zjunlp/LightMem)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Efficiency-red)

1. **Memory OS of AI Agent**\
   Jiazheng Kang, Mingming Ji, Zhe Zhao, Ting Bai. *EMNLP 2025*. [[Paper](https://arxiv.org/abs/2506.06326)] [[Code](https://github.com/BAI-LAB/MemoryOS)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Hierarchical-purple) ![](https://img.shields.io/badge/-Personalization-green)

1. **Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory**\
   Prateek Chhikara, Dev Khant, Saket Aryan, et al. *ECAI 2025*. [[Paper](https://arxiv.org/abs/2504.19413)] [[Code](https://github.com/mem0ai/mem0)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Semantic-green)

1. **MIRIX: Multi-Agent Memory System for LLM-Based Agents**\
   Yu Wang, Xi Chen. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2507.07957)] [[Code](https://github.com/Mirix-AI/MIRIX)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Multimodal-purple) ![](https://img.shields.io/badge/-Multi_Agent-purple)

1. **MemOS: A Memory OS for AI System**\
   Zhiyu Li, Chenyang Xi, Chunyu Li, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2507.03724)] [[Code](https://github.com/MemTensor/MemOS)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Memory_OS-purple) ![](https://img.shields.io/badge/-Lifecycle-orange)

1. **🆕 Optimus-1: Hybrid Multimodal Memory Empowered Agents Excel in Long-Horizon Tasks**\
   Zaijing Li, Yuquan Xie, Rui Shao, et al. *NeurIPS 2024*. [[Paper](https://arxiv.org/abs/2408.03615)] [[Code](https://github.com/JiuTian-VL/Optimus-1)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Multimodal-purple) ![](https://img.shields.io/badge/-Long_Horizon-purple)

1. **🆕 JARVIS-1: Open-World Multi-Task Agents with Memory-Augmented Multimodal Language Models**\
   Zihao Wang, Shaofei Cai, Anji Liu, et al. *IEEE TPAMI 2024*. [[Paper](https://arxiv.org/abs/2311.05997)] [[Code](https://github.com/CraftJarvis/JARVIS-1)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Multimodal-purple) ![](https://img.shields.io/badge/-Procedural-yellowgreen)

1. **MemGPT: Towards LLMs as Operating Systems**\
   Charles Packer, Sarah Wooders, Kevin Lin, et al. *arXiv 2023*. [[Paper](https://arxiv.org/abs/2310.08560)] [[Code](https://github.com/letta-ai/letta)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-Hybrid-purple) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Memory_OS-purple) ![](https://img.shields.io/badge/-Read_Write-orange)

1. **🆕 A Machine with Short-Term, Episodic, and Semantic Memory Systems**\
   Taewoon Kim, Michael Cochez, Vincent François-Lavet, et al. *AAAI 2023*. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25075)]\
   ![](https://img.shields.io/badge/-Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Composite-purple) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-RL_based-orange)

[⬆️ top](#table-of-contents)

### 1.4 Baselines and Supporting Methods

Foundational retrieval, reasoning, reflection, and context-management methods commonly used as baselines or components in agent-memory studies.

1. **🆕 Buffer of Thoughts: Thought-Augmented Reasoning with Large Language Models**\
   Ling Yang, Zhaochen Yu, Tianjun Zhang, et al. *NeurIPS 2024 Spotlight*. [[Paper](https://arxiv.org/abs/2406.04271)] [[Code](https://github.com/YangLing0818/buffer-of-thought-llm)]\
   ![](https://img.shields.io/badge/-Supporting_Method-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Procedural-yellowgreen) ![](https://img.shields.io/badge/-Reasoning-yellowgreen)

1. **Self-RAG: Learning to Retrieve, Generate, and Critique through Self-Reflection**\
   Akari Asai, Zeqiu Wu, Yizhong Wang, et al. *ICLR 2024*. [[Paper](https://arxiv.org/abs/2310.11511)] [[Code](https://github.com/AkariAsai/self-rag)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-SFT-orange)

1. **From Local to Global: A Graph RAG Approach to Query-Focused Summarization**\
   Darren Edge, Ha Trinh, Newman Cheng, et al. *arXiv 2024*. [[Paper](https://arxiv.org/abs/2404.16130)] [[Code](https://github.com/microsoft/graphrag)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Graph-purple) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Summarization-yellowgreen)

1. **🆕 Reflexion: Language Agents with Verbal Reinforcement Learning**\
   Noah Shinn, Federico Cassano, Edward Berman, et al. *NeurIPS 2023*. [[Paper](https://arxiv.org/abs/2303.11366)] [[Code](https://github.com/noahshinn/reflexion)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Episodic-green) ![](https://img.shields.io/badge/-Reflection-yellowgreen)

1. **🆕 ReAct: Synergizing Reasoning and Acting in Language Models**\
   Shunyu Yao, Jeffrey Zhao, Dian Yu, et al. *ICLR 2023*. [[Paper](https://arxiv.org/abs/2210.03629)] [[Code](https://github.com/ysymyth/ReAct)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-Prompt_based-orange) ![](https://img.shields.io/badge/-Working-purple) ![](https://img.shields.io/badge/-Reasoning-yellowgreen) ![](https://img.shields.io/badge/-Tool_Use-purple)

1. **Unsupervised Dense Information Retrieval with Contrastive Learning**\
   Gautier Izacard, Mathilde Caron, Lucas Hosseini, et al. *ICLR 2022*. [[Paper](https://arxiv.org/abs/2112.09118)] [[Code](https://github.com/facebookresearch/contriever)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Dense_Retrieval-blue) ![](https://img.shields.io/badge/-Training_free-orange) ![](https://img.shields.io/badge/-Embedding-blue)

1. **🆕 Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks**\
   Patrick Lewis, Ethan Perez, Aleksandra Piktus, et al. *NeurIPS 2020*. [[Paper](https://arxiv.org/abs/2005.11401)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Textual-blue) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Generation-green)

1. **🆕 The Probabilistic Relevance Framework: BM25 and Beyond**\
   Stephen Robertson, Hugo Zaragoza. *Foundations and Trends in Information Retrieval 2009*. [[Paper](https://doi.org/10.1561/1500000019)]\
   ![](https://img.shields.io/badge/-Baseline-lightgrey) ![](https://img.shields.io/badge/-External-blue) ![](https://img.shields.io/badge/-Sparse_Retrieval-blue) ![](https://img.shields.io/badge/-Lexical-blue) ![](https://img.shields.io/badge/-Training_free-orange)

[⬆️ top](#table-of-contents)

## 2. Benchmarks and Datasets

Each benchmark appears once under its primary evaluation purpose; third-line tags record secondary dimensions.

### 2.1 Effectiveness Evaluation

Benchmarks centered on answer quality, task success, action correctness, or end-to-end agent capability.

1. **LongBench v2: Towards Deeper Understanding and Reasoning on Realistic Long-context Multitasks**\
   Yushi Bai, Shangqing Tu, Jiajie Zhang, et al. *ACL 2025*. [[Paper](https://arxiv.org/abs/2412.15204)] [[Code](https://github.com/THUDM/LongBench)] [[Dataset](https://huggingface.co/datasets/zai-org/LongBench-v2)]\
   ![](https://img.shields.io/badge/-503_QA-lightgrey) ![](https://img.shields.io/badge/-single_doc_QA-blue) ![](https://img.shields.io/badge/-multi_doc_QA-blue) ![](https://img.shields.io/badge/-long_context-purple) ![](https://img.shields.io/badge/-structured_data-orange)

1. **🆕 OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments**\
   Tianbao Xie, Danyang Zhang, Jixuan Chen, et al. *NeurIPS 2024 Datasets and Benchmarks*. [[Paper](https://arxiv.org/abs/2404.07972)] [[Code](https://github.com/xlang-ai/OSWorld)] [[Dataset](https://github.com/xlang-ai/OSWorld)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Effectiveness-green) ![](https://img.shields.io/badge/-GUI-purple) ![](https://img.shields.io/badge/-Multimodal-purple) ![](https://img.shields.io/badge/-Long_Horizon-purple)

1. **🆕 MemSim: A Bayesian Simulator for Evaluating Memory of LLM-based Personal Assistants**\
   Zeyu Zhang, Quanyu Dai, Luyu Chen, et al. *arXiv 2024*. [[Paper](https://arxiv.org/abs/2409.20163)] [[Code](https://github.com/nuster1128/MemSim)] [[Dataset](https://github.com/nuster1128/MemSim)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Effectiveness-green) ![](https://img.shields.io/badge/-Personalization-green) ![](https://img.shields.io/badge/-QA-blue) ![](https://img.shields.io/badge/-Simulation-purple)

1. **🆕 AgentBench: Evaluating LLMs as Agents**\
   Xiao Liu, Hao Yu, Hanchen Zhang, et al. *ICLR 2024*. [[Paper](https://arxiv.org/abs/2308.03688)] [[Code](https://github.com/THUDM/AgentBench)] [[Dataset](https://github.com/THUDM/AgentBench)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Effectiveness-green) ![](https://img.shields.io/badge/-Agent-purple) ![](https://img.shields.io/badge/-Interactive-green) ![](https://img.shields.io/badge/-Multi_Environment-purple)

1. **🆕 WebArena: A Realistic Web Environment for Building Autonomous Agents**\
   Shuyan Zhou, Frank F. Xu, Hao Zhu, et al. *ICLR 2024*. [[Paper](https://arxiv.org/abs/2307.13854)] [[Code](https://github.com/web-arena-x/webarena)] [[Dataset](https://github.com/web-arena-x/webarena)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Effectiveness-green) ![](https://img.shields.io/badge/-Web-purple) ![](https://img.shields.io/badge/-Interactive-green) ![](https://img.shields.io/badge/-Long_Horizon-purple)

[⬆️ top](#table-of-contents)

### 2.2 Retrieval Evaluation

Benchmarks focused on recalling facts, evidence, events, or relevant context over long documents and multi-session interactions.

1. **🆕 MADial-Bench: Towards Real-world Evaluation of Memory-Augmented Dialogue Generation**\
   Junqing He, Liang Zhu, Rui Wang, et al. *NAACL 2025*. [[Paper](https://arxiv.org/abs/2409.15240)] [[Code](https://github.com/hejunqing/MADial-Bench)] [[Dataset](https://github.com/hejunqing/MADial-Bench)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Dialogue-purple) ![](https://img.shields.io/badge/-Memory_Recall-green) ![](https://img.shields.io/badge/-Generation-green)

1. **LongMemEval: Benchmarking Chat Assistants on Long-Term Interactive Memory**\
   Di Wu, Hongwei Wang, Wenhao Yu, et al. *ICLR 2025*. [[Paper](https://arxiv.org/abs/2410.10813)] [[Code](https://github.com/xiaowu0162/LongMemEval)] [[Dataset](https://github.com/xiaowu0162/LongMemEval)]\
   ![](https://img.shields.io/badge/-500_queries-lightgrey) ![](https://img.shields.io/badge/-115K_to_1.5M_tokens-lightgrey) ![](https://img.shields.io/badge/-cross_session_QA-green) ![](https://img.shields.io/badge/-knowledge_update-orange) ![](https://img.shields.io/badge/-temporal_reasoning-yellowgreen)

1. **RULER: What's the Real Context Size of Your Long-Context Language Models?**\
   Cheng-Ping Hsieh, Simeng Sun, Samuel Kriman, et al. *COLM 2024*. [[Paper](https://arxiv.org/abs/2404.06654)] [[Code](https://github.com/NVIDIA/RULER)] [[Dataset](https://github.com/NVIDIA/RULER)]\
   ![](https://img.shields.io/badge/-13_tasks-lightgrey) ![](https://img.shields.io/badge/-synthetic_benchmark-purple) ![](https://img.shields.io/badge/-needle_in_haystack-green) ![](https://img.shields.io/badge/-multi_hop_tracing-blue) ![](https://img.shields.io/badge/-aggregation-orange)

1. **Evaluating Very Long-Term Conversational Memory of LLM Agents**\
   Adyasha Maharana, Dong-Ho Lee, Sergey Tulyakov, et al. *ACL 2024*. [[Paper](https://arxiv.org/abs/2402.17753)] [[Code](https://github.com/snap-research/LoCoMo)] [[Dataset](https://github.com/snap-research/LoCoMo)]\
   ![](https://img.shields.io/badge/-1.9K_QA-lightgrey) ![](https://img.shields.io/badge/-10_dialogues-lightgrey) ![](https://img.shields.io/badge/-long_conversation-green) ![](https://img.shields.io/badge/-temporal_QA-orange) ![](https://img.shields.io/badge/-multimodal_dialogue-purple)

1. **🆕 ∞Bench: Extending Long Context Evaluation Beyond 100K Tokens**\
   Xinrong Zhang, Yingfa Chen, Shengding Hu, et al. *ACL 2024*. [[Paper](https://arxiv.org/abs/2402.13718)] [[Code](https://github.com/OpenBMB/InfiniteBench)] [[Dataset](https://github.com/OpenBMB/InfiniteBench)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Long_Context-purple) ![](https://img.shields.io/badge/-100K%2B-lightgrey) ![](https://img.shields.io/badge/-Bilingual-purple)

1. **🆕 LongBench: A Bilingual, Multitask Benchmark for Long Context Understanding**\
   Yushi Bai, Xin Lv, Jiajie Zhang, et al. *ACL 2024*. [[Paper](https://arxiv.org/abs/2308.14508)] [[Code](https://github.com/THUDM/LongBench)] [[Dataset](https://github.com/THUDM/LongBench)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Long_Context-purple) ![](https://img.shields.io/badge/-Multitask-purple) ![](https://img.shields.io/badge/-Bilingual-purple)

1. **🆕 Beyond Goldfish Memory: Long-Term Open-Domain Conversation**\
   Jing Xu, Arthur Szlam, Jason Weston. *ACL 2022*. [[Paper](https://arxiv.org/abs/2107.07567)] [[Dataset](https://parl.ai/projects/msc/)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Retrieval-green) ![](https://img.shields.io/badge/-Multi_Session-purple) ![](https://img.shields.io/badge/-Dialogue-purple) ![](https://img.shields.io/badge/-Personalization-green)

1. **HotpotQA: A Dataset for Diverse, Explainable Multi-hop Question Answering**\
   Zhilin Yang, Peng Qi, Saizheng Zhang, et al. *EMNLP 2018*. [[Paper](https://arxiv.org/abs/1809.09600)] [[Code](https://github.com/hotpotqa/hotpot)] [[Dataset](https://hotpotqa.github.io/)]\
   ![](https://img.shields.io/badge/-113K_QA-lightgrey) ![](https://img.shields.io/badge/-multi_hop_QA-blue) ![](https://img.shields.io/badge/-explainable_reasoning-yellowgreen) ![](https://img.shields.io/badge/-supporting_facts-orange)

[⬆️ top](#table-of-contents)

### 2.3 Robustness Evaluation

Benchmarks stressing continuous learning, conflict resolution, knowledge updates, selective forgetting, or hallucination propagation.

1. **Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions**\
   Yuanzhe Hu, Yu Wang, Julian McAuley. *ICLR 2026*. [[Paper](https://arxiv.org/abs/2507.05257)] [[Code](https://github.com/HUST-AI-HYZ/MemoryAgentBench)] [[Dataset](https://huggingface.co/datasets/ai-hyz/MemoryAgentBench)]\
   ![](https://img.shields.io/badge/-2,071_QA-lightgrey) ![](https://img.shields.io/badge/-accurate_retrieval-green) ![](https://img.shields.io/badge/-test_time_learning-orange) ![](https://img.shields.io/badge/-long_range_understanding-purple) ![](https://img.shields.io/badge/-conflict_resolution-yellowgreen)

1. **🆕 HaluMem: Evaluating Hallucinations in Memory Systems of Agents**\
   Ding Chen, Simin Niu, Kehang Li, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2511.03506)] [[Code](https://github.com/MemTensor/HaluMem)] [[Dataset](https://huggingface.co/datasets/IAAR-Shanghai/HaluMem)]\
   ![](https://img.shields.io/badge/-Benchmark-lightgrey) ![](https://img.shields.io/badge/-Robustness-red) ![](https://img.shields.io/badge/-Hallucination-red) ![](https://img.shields.io/badge/-Memory_Update-orange) ![](https://img.shields.io/badge/-Long_Context-purple)

1. **LifelongAgentBench: Evaluating LLM Agents as Lifelong Learners**\
   Junhao Zheng, Xidi Cai, Qiuke Li, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2505.11942)] [[Code](https://github.com/caixd-220529/LifelongAgentBench)] [[Dataset](https://huggingface.co/datasets/csyq/LifelongAgentBench)]\
   ![](https://img.shields.io/badge/-1.4K_tasks-lightgrey) ![](https://img.shields.io/badge/-database-purple) ![](https://img.shields.io/badge/-operating_system-purple) ![](https://img.shields.io/badge/-knowledge_graph-purple) ![](https://img.shields.io/badge/-skill_transfer-green) ![](https://img.shields.io/badge/-forgetting_drop-orange)

1. **StreamBench: Towards Benchmarking Continuous Improvement of Language Agents**\
   Cheng-Kuang Wu, Zhi Rui Tam, Chieh-Yen Lin, et al. *NeurIPS 2024 Datasets and Benchmarks*. [[Paper](https://arxiv.org/abs/2406.08747)] [[Code](https://github.com/stream-bench/stream-bench)] [[Dataset](https://github.com/stream-bench/stream-bench)]\
   ![](https://img.shields.io/badge/-9.7K_instances-lightgrey) ![](https://img.shields.io/badge/-streaming_learning-orange) ![](https://img.shields.io/badge/-conflict_resolution-yellowgreen) ![](https://img.shields.io/badge/-online_feedback-green)

[⬆️ top](#table-of-contents)

### 2.4 Efficiency Evaluation

Benchmarks and studies exposing latency, token use, context scaling, construction cost, maintenance overhead, or task-cost trade-offs.

1. **🆕 Are We Ready For An Agent-Native Memory System?**\
   Wei Zhou, Xuanhe Zhou, Shaokun Han, et al. *arXiv 2026*. [[Paper](https://arxiv.org/abs/2606.24775)] [[Code](https://github.com/OpenDataBox/MemoryData)] [[Dataset](https://github.com/OpenDataBox/MemoryData)]\
   ![](https://img.shields.io/badge/-Evaluation-lightgrey) ![](https://img.shields.io/badge/-Efficiency-red) ![](https://img.shields.io/badge/-Data_Management-blue) ![](https://img.shields.io/badge/-Ablation-orange) ![](https://img.shields.io/badge/-Cost_Quality-red)

1. **MemGUI-Bench: Benchmarking Memory of Mobile GUI Agents in Dynamic Environments**\
   Guangyi Liu, Pengxiang Zhao, Yaozhen Liang, et al. *arXiv 2026*. [[Paper](https://arxiv.org/abs/2602.06075)] [[Code](https://github.com/lgy0404/MemGUI-Bench)] [[Dataset](https://memgui-bench.github.io/)]\
   ![](https://img.shields.io/badge/-128_tasks-lightgrey) ![](https://img.shields.io/badge/-step_ratio-red) ![](https://img.shields.io/badge/-time_per_step-red) ![](https://img.shields.io/badge/-cost_per_step-red) ![](https://img.shields.io/badge/-mobile_GUI-purple)

1. **MemBench: Towards More Comprehensive Evaluation on the Memory of LLM-based Agents**\
   Haoran Tan, Zeyu Zhang, Chen Ma, et al. *ACL 2025 Findings*. [[Paper](https://arxiv.org/abs/2506.21605)] [[Code](https://github.com/import-myself/Membench)] [[Dataset](https://github.com/import-myself/Membench)]\
   ![](https://img.shields.io/badge/-53K_questions-lightgrey) ![](https://img.shields.io/badge/-65K_sessions-lightgrey) ![](https://img.shields.io/badge/-latency-red) ![](https://img.shields.io/badge/-capacity-orange) ![](https://img.shields.io/badge/-memory_overhead-yellowgreen)

[⬆️ top](#table-of-contents)

## 3. Surveys, Tutorials, and Position Papers

1. **🆕 Rethinking Memory Mechanisms of Foundation Agents in the Second Half: A Survey**\
   Wei-Chieh Huang, Weizhi Zhang, Yueqing Liang, et al. *arXiv 2026*. [[Paper](https://arxiv.org/abs/2602.06052)] [[Code](https://github.com/AgentMemoryWorld/Awesome-Agent-Memory)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Foundation_Agents-purple) ![](https://img.shields.io/badge/-Memory_Substrate-purple) ![](https://img.shields.io/badge/-Cognitive_Mechanism-yellowgreen)

1. **Memory in the Age of AI Agents**\
   Yuyang Hu, Shichun Liu, Yanwei Yue, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2512.13564)] [[Code](https://github.com/Shichun-Liu/Agent-Memory-Paper-List)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Agent_Memory-purple) ![](https://img.shields.io/badge/-Forms-blue) ![](https://img.shields.io/badge/-Functions-green) ![](https://img.shields.io/badge/-Dynamics-orange)

1. **🆕 Rethinking Memory in LLM based Agents: Representations, Operations, and Emerging Topics**\
   Yiming Du, Wenyu Huang, Danna Zheng, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2505.00675)] [[Code](https://github.com/Elvin-Yiming-Du/Survey_Memory_in_AI)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Representations-purple) ![](https://img.shields.io/badge/-Operations-orange) ![](https://img.shields.io/badge/-Taxonomy-yellowgreen) ![](https://img.shields.io/badge/-Agent_Memory-purple)

1. **🆕 From Human Memory to AI Memory: A Survey on Memory Mechanisms in the Era of LLMs**\
   Yaxiong Wu, Sheng Liang, Chen Zhang, et al. *arXiv 2025*. [[Paper](https://arxiv.org/abs/2504.15965)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Human_Memory-purple) ![](https://img.shields.io/badge/-LLM_Memory-purple) ![](https://img.shields.io/badge/-Cognitive_Inspiration-yellowgreen) ![](https://img.shields.io/badge/-Taxonomy-yellowgreen)

1. **Lifelong Learning of Large Language Model based Agents: A Roadmap**\
   Junhao Zheng, Chengming Shi, Xidi Cai, et al. *IEEE TPAMI 2025*. [[Paper](https://arxiv.org/abs/2501.07278)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Roadmap-yellowgreen) ![](https://img.shields.io/badge/-Lifelong_Learning-orange) ![](https://img.shields.io/badge/-Agent_Memory-purple) ![](https://img.shields.io/badge/-Continual_Learning-orange)

1. **A Survey on the Memory Mechanism of Large Language Model based Agents**\
   Zeyu Zhang, Xiaohe Bo, Chen Ma, et al. *ACM TOIS 2025*. [[Paper](https://arxiv.org/abs/2404.13501)] [[Code](https://github.com/nuster1128/LLM_Agent_Memory_Survey)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Agent_Memory-purple) ![](https://img.shields.io/badge/-Design-blue) ![](https://img.shields.io/badge/-Evaluation-lightgrey) ![](https://img.shields.io/badge/-Applications-purple)

1. **🆕 Human-inspired Perspectives: A Survey on AI Long-term Memory**\
   Zihong He, Weizhe Lin, Hao Zheng, et al. *arXiv 2024*. [[Paper](https://arxiv.org/abs/2411.00489)]\
   ![](https://img.shields.io/badge/-Survey-lightgrey) ![](https://img.shields.io/badge/-Long_Term_Memory-purple) ![](https://img.shields.io/badge/-Human_Memory-purple) ![](https://img.shields.io/badge/-Cognitive_Architecture-yellowgreen)

1. **🆕 Cognitive Architectures for Language Agents**\
   Theodore R. Sumers, Shunyu Yao, Karthik Narasimhan, Thomas L. Griffiths. *TMLR 2024*. [[Paper](https://arxiv.org/abs/2309.02427)] [[Code](https://github.com/ysymyth/awesome-language-agents)]\
   ![](https://img.shields.io/badge/-Position_Paper-lightgrey) ![](https://img.shields.io/badge/-Tutorial-lightgrey) ![](https://img.shields.io/badge/-Cognitive_Architecture-yellowgreen) ![](https://img.shields.io/badge/-Modular_Memory-purple)

[⬆️ top](#table-of-contents)

## 4. Frameworks, Products, and Resources

Paper-backed implementations are linked beside their papers above. The following broader platforms and curated collections were used as complementary sources and are useful for continued tracking.

1. **MemoryData**\
   OpenDataBox. [[GitHub](https://github.com/OpenDataBox/MemoryData)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Evaluation_Platform-purple) ![](https://img.shields.io/badge/-Memory_Systems-purple) ![](https://img.shields.io/badge/-Datasets-lightgrey)

1. **Agent Memory Paper List**\
   Shichun-Liu. [[GitHub](https://github.com/Shichun-Liu/Agent-Memory-Paper-List)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Agent_Memory-purple) ![](https://img.shields.io/badge/-Taxonomy-yellowgreen)

1. **Awesome AI Memory**\
   IAAR-Shanghai. [[GitHub](https://github.com/IAAR-Shanghai/Awesome-AI-Memory)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Systems-purple) ![](https://img.shields.io/badge/-Benchmarks-lightgrey)

1. **Awesome Memory for Agents**\
   TsinghuaC3I. [[GitHub](https://github.com/TsinghuaC3I/Awesome-Memory-for-Agents)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Applications-purple) ![](https://img.shields.io/badge/-Benchmarks-lightgrey)

1. **Awesome Agent Memory**\
   TeleAI-UAGI. [[GitHub](https://github.com/TeleAI-UAGI/Awesome-Agent-Memory)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Products-purple) ![](https://img.shields.io/badge/-Multimodal_Memory-purple)

1. **Awesome Graph-based Agent Memory**\
   DEEP-PolyU. [[GitHub](https://github.com/DEEP-PolyU/Awesome-GraphMemory)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Graph_Memory-purple) ![](https://img.shields.io/badge/-Benchmarks-lightgrey)

1. **Awesome Agent Memory Papers**\
   yyyujintang. [[GitHub](https://github.com/yyyujintang/Awesome-Agent-Memory-Papers)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Dashboard-purple) ![](https://img.shields.io/badge/-Multi_Tag-yellowgreen)

1. **Awesome Agent Memory (Foundation Agents)**\
   AgentMemoryWorld. [[GitHub](https://github.com/AgentMemoryWorld/Awesome-Agent-Memory)]\
   ![](https://img.shields.io/badge/-Resource-lightgrey) ![](https://img.shields.io/badge/-Paper_List-lightgrey) ![](https://img.shields.io/badge/-Foundation_Agents-purple) ![](https://img.shields.io/badge/-Taxonomy-yellowgreen)

[⬆️ top](#table-of-contents)

## Citation

```bibtex
@article{memoryasdata,
    title={Are We Ready For An Agent-Native Memory System?},
    author={Wei Zhou and Xuanhe Zhou and Shaokun Han and Hongming Xu and Guoliang Li and Zhiyu Li and Feiyu Xiong and Fan Wu},
    year={2026},
    journal={arXiv preprint arXiv:2606.24775},
    url={https://arxiv.org/abs/2606.24775}
}
```
