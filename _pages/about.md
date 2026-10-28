---
permalink: /
title: ""
excerpt: "Lingbo Wang - VLM, reinforcement learning, and agent memory"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

# About Me

I am **Lingbo Wang**, a master's student in the Natural Language Processing Lab at [Soochow University](https://www.suda.edu.cn/), advised by [Prof. Yu Hong](https://scst.suda.edu.cn/0c/f9/c30767a527609/page.htm). I received my B.Eng. in Intelligent Science and Technology from Qilu University of Technology.

My work focuses on **vision-language model (VLM) pre-training and post-training**, **reinforcement learning** (MPO, GSPO, ROPD, and Agentic RL), and **memory for long-horizon LLM agents**. I have experience building and training large-scale multimodal models with Megatron, DeepSpeed, VeRL, and vLLM.

[Download my résumé (PDF)](/王令博_2027应届生.pdf) · [GitHub](https://github.com/vllbc) · [Technical Blog](https://blog.vllbc.top)

# 🔥 News

- **2026:** *EffectMem: Effectiveness-Driven Memory Reuse for Long-Horizon LLM Agents* was accepted by **EMNLP 2026**.
- **2026:** *Anti-Exception Action Generation for Automatic Planning* was accepted by **ICASSP 2026**.
- **2025.09 - 2026.03:** Joined Baidu's Application Model Unit as a research intern, working on VLM pre-training, post-training, and reinforcement learning.

# 📝 Publications

1. **EffectMem: Effectiveness-Driven Memory Reuse for Long-Horizon LLM Agents**<br>
   **Lingbo Wang** (first author). *EMNLP 2026*, CCF-B.<br>
   We introduce an effectiveness-driven memory reuse framework that represents successful trajectories as executable contracts and validates their applicability before reuse. EffectMem outperforms ReAct, ExpeL, AutoGuide, and CFGM on ALFWorld, ScienceWorld, and WebShop.

2. **Anti-Exception Action Generation for Automatic Planning**<br>
   **Lingbo Wang** (first author). *ICASSP 2026*, CCF-B.

3. **RubricFlow-Mem: Rubric-Guided Self-Evolving Curriculum for Long-Term Memory Agents**<br>
   **Lingbo Wang** (first author). *Under review at ICLR 2027*.

# 💻 Experience

## Baidu · Application Model Unit (AMU), Multimodal Perception and Understanding

*Research Intern · 2025.09 - 2026.03*

**Wenxin-Lightning VLM foundation model**

- Contributed to data construction, architecture adaptation, and multi-stage pre-training/post-training of a multimodal MoE model for AI Search using Megatron.
- Built large-scale MapReduce data-cleaning and quality-evaluation pipelines; adapted InternViT/RiceViT and Lightning LLM/Qwen3 LLM; implemented bidirectional Megatron-Hugging Face checkpoint conversion.
- Helped establish an H200 thousand-GPU-scale training pipeline and an EvalScope evaluation workflow, then iterated SFT data mixtures and training strategies based on benchmark results.
- Constructed MPO preference data and conducted MPO post-training with DeepSpeed to improve mathematical reasoning.
- The resulting model reached **105.19%** of Qwen3-VL-30B-A3B's aggregate score on general VLM benchmarks and **124.11%** in STEM, while reducing average chain-of-thought length by **18.7%** and improving inference speed by **23.1%**.

**Wenxin Assistant photo-based K-12 problem solving**

- Built a data flywheel and MPO preference samples from real user queries; adapted the 30B-A3B MoE model in VeRL and established a hundred-GPU GSPO training pipeline.
- Developed offline evaluation to refine rewards and constraints and mitigate reward hacking; optimized LLM-as-a-Judge scheduling and vLLM image processing to reduce training bubbles, visual tokens, and inference cost.
- Improved offline accuracy from **79%** for the online baseline to **81%** with MPO and **85%** with GSPO, matching Seed1.6. After launch, page views increased by **1.37%** and search sessions by **1.12%**.

# 🧩 Selected Project

## World-Model-Driven Lookahead Planning for LLM Agents

*Agentic RL open-source project · 2025.06 - 2025.09*

- Identified and fixed an Agentic RL training bug in the VeRL main repository; the pull request was merged upstream.
- Extended `verl-agent` with a world-model-driven lookahead planner. At each rollout state, the planner samples candidate actions, predicts their next observations in batches, scores predicted states with rule-based or learned rewards, and executes the action with the highest expected return.
- On ALFWorld with Qwen2.5-1.5B Base, the success rate reached **50.78%** after 40 co-training steps and peaked at **93.84%** after convergence. World-model loss fell from **0.824** to **0.155**, while average task steps decreased by **70%**.

# 🎓 Education

- **Soochow University**, M.S. in Computer Science and Technology, Natural Language Processing Lab<br>
  *2024.09 - Present*
- **Qilu University of Technology**, B.Eng. in Intelligent Science and Technology, School of Mathematics and Statistics<br>
  *2020.09 - 2024.07*

# 🛠 Skills

- **Research:** VLM pre-training and post-training, MPO, GSPO, ROPD, Agentic RL, agent memory, automatic planning
- **Training and inference:** Megatron, DeepSpeed, VeRL, vLLM, EvalScope
- **Model architectures:** multimodal MoE, InternViT, RiceViT, Lightning LLM, Qwen3 LLM
- **Data and infrastructure:** MapReduce, large-scale distributed training, SFT and preference-data construction, LLM-as-a-Judge
