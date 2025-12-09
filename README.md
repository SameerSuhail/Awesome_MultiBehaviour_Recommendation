# Multi-Behavior Recommendation in the Deep Learning Era

**Models • Optimization • Open Challenges**

This repository contains the official resources for our survey "Multi-Behavior Recommendation in the Deep Learning Era: Models, Optimization, and Open Challenges."

The survey provides a complete, structured overview of how modern recommender systems model multiple user behaviors such as views, clicks, likes, add-to-cart, shares, and purchases.

## 🔍 Overview

Traditional single-behavior recommendation is no longer sufficient for real-world platforms. Multi-behavior recommendation (MBR) introduces richer signals but also new challenges such as behavior imbalance, semantic heterogeneity, temporal dependencies, and cross-task transfer.

Our work organizes the MBR landscape using a unified three-layer taxonomy:

- **Input Layer** – What signals enter the model?
- **Method Layer** – What architectures are used to model multi-behavior data?
- **Optimization Layer** – What objectives and training paradigms are used?

## 📋 Survey Overview

This survey analyzes all major directions in multi-behavior recommendation, including:

- Graph Neural Networks (GNNs)
- Multi-task learning
- Contrastive and self-supervised learning
- Knowledge-enhanced models
- Sequential models (RNNs, GNNs, Transformers)
- Generative models (autoregressive and diffusion-based)
- Reinforcement learning for multi-behavior feedback

We also provide detailed comparisons, identify common design patterns, and outline open research challenges.

## 🗂 Taxonomy Summary

### 1. Input Layer

Models may use the following input signals:

- Multi-behavior interactions
- User profile features
- Item metadata
- Knowledge graph information
- Social network signals
- Temporal sequence information

### 2. Method Layer

#### A. Models Using Only Multi-Behavior Data

- **Graph Neural Networks**: MBGCN, GNMR, MBRec, HEC-GCN, POGCN
- **Multi-task learning**: NMTR, EHCF, MB-GMN, HPMR
- **Contrastive learning frameworks**: HMG-CR, CML, RCL, MBRCC, MBSSL
- **Knowledge-enhanced methods**: KHGT, KMCLR, CLMRS, KEMCL

#### B. Models Combining Multi-Behavior + Sequential Signals

- **RNN-based models**: RLBL, BINN, IARS
- **Sequential GNNs**: MRIG, GPG4HSR, TGT, GHTDL, TAGCL
- **Generative models**: MBGen, GAMER, ICDD-T, M3BSSR, GRACE
- **Reinforcement learning**: MBKR, MB-GRL

### 3. Optimization Layer

- Supervised objectives
- Self-supervised contrastive objectives
- Reinforcement learning objectives
- Generative modeling losses

## 📈 Key Contributions

- A unified three-layer taxonomy for understanding multi-behavior recommendation
- Coverage of all major architectural families used in MBR
- A strict interpretation of how GNN-based models handle multi-behavior aggregation
- A deep dive into contrastive learning, generative modeling, and reinforcement learning in the MBR context
- A clear breakdown of strengths, limitations, and when each method should be used
- Identification of open research challenges, including behavior semantics, scalability, and unified modeling

## 📁 Repository Structure

```
├── README.md
├── survey.pdf
├── figures/
│   ├── taxonomy.png
│   ├── gnn_architecture.png
│   ├── mtl_framework.png
│   └── rl_flow.png
└── citations.bib
```

If you'd like, we can automatically extract all diagrams from the PDF and place them in the `figures/` folder.

## 🚀 How to Use This Repository

### For Researchers

- Use the taxonomy as a guide to categorize new and existing models
- Identify gaps in current MBR approaches for future research

### For Practitioners

- Select the right model family based on data characteristics (sparsity, sequence length, behavior diversity)
- Understand trade-offs such as scalability vs. modeling complexity

### For Students

- Get a structured introduction to multi-behavior recommendation
- Use the survey as a starting point for semester projects or thesis work

## 🧭 Roadmap

We plan to release:

- [ ] Implementations of key models
- [ ] Unified pseudo-code templates
- [ ] A benchmarking pipeline
- [ ] A Colab playground for experimentation
- [ ] A website version of the survey

## 📚 Papers Collection

| Year | Title | Venue | Link |
|------|-------|--------|------|
| 2015 | Multi-Behavioral Sequential Prediction with Recurrent Log-Bilinear Model | IEEE TKDE | [(https://dl.acm.org/doi/10.1109/TKDE.2017.2661760) |
| 2018 | Learning from History and Present: Next-item Recommendation via Discriminatively Exploiting User Behaviors  | SIGIR | https://dl.acm.org/doi/10.1145/3219819.3220014 |
| 2021 | Incorporating Link Prediction into Multi-Relational Item Graph Modeling for Session-Based Recommendation | TKDE | N/A |
| 2021 | Intent-Aware Recommender Systems | CIKM | N/A |
| 2022 | Global and Personalized Graphs for Heterogeneous SequentialRecommendation by Learning Behavior Transitions and UserIntentions | RecSys| https://dl.acm.org/doi/10.1145/3523227.3546761 |
| 2022 | Multi-Behavior Sequential Recommendation with Temporal Graph Transformer | TKDE| https://arxiv.org/abs/2206.02687 |
| 2024 | Global Heterogeneous Graph and Target Interest Denoising for Multi-behavior Sequential Recommendation | WSDM| https://dl.acm.org/doi/10.1145/3616855.3635857 |
| 2025 | TAGCL: A Time-Aware Recommendation Method via Graph Contrastive Learning | RAIIC| DOI: 10.1109/RAIIC65850.2025.11170190 |
| 2024 | Multi-Behavior Generative Recommendation | CIKM| https://arxiv.org/abs/2405.16871 |
| 2025 | Generative Sequential Recommendation via Hierarchical Behavior Modeling |  | [https://arxiv.org/abs/2405.16871](https://arxiv.org/abs/2511.03155) |
| 2025 | Target Item-oriented Conditional Diffusion Differential Transformer for Next-Item Prediction | CIKM | https://dl.acm.org/doi/10.1145/3746252.3761395 |
| 2025 | Multi-Modal Multi-Behavior Sequential Recommendation with Conditional Diffusion-Based Feature Denoising | SIGIR | https://dl.acm.org/doi/10.1145/3726302.3730044 |
| 2025 | GRACE: Generative Recommendation via Journey-Aware Sparse Attention on Chain-of-Thought Tokenization | RecSys | https://arxiv.org/html/2507.14758v1 |
| 2022 | Micro-behaviour with Reinforcement Knowledge-aware Reasoning for Explainable Recommendation | KBS | https://www.sciencedirect.com/science/article/abs/pii/S0950705122006529|
| 2024 | Multi-behavior Session-based Recommendation via Graph Reinforcement Learning | PMLR | https://proceedings.mlr.press/v222/qin24a.html|
| 2020 | Multi-behavior Recommendation with Graph Convolutional Networks | SIGIR |https://dl.acm.org/doi/10.1145/3397271.3401072|
| 2021 | Multi-Behavior Enhanced Recommendation with Cross-Interaction Collaborative Relation Modeling | ICDE |https://arxiv.org/abs/2201.02307|
| 2022 | Multi-Behavior Graph Neural Networks for Recommender System | IEEE Transactions on Nueral Networks and Learning Systems |https://arxiv.org/abs/2302.08678|
| 2024 | HEC-GCN: Hypergraph Enhanced Cascading Graph Convolution Network for Multi-Behavior Recommendation | |https://arxiv.org/abs/2412.14476|
| 2024 | Multi-Behavior Collaborative Filtering with Partial Order Graph Convolutional Networks | KDD |https://arxiv.org/abs/2402.07659|
| 2021 |Hyper Meta-Path Contrastive Learning for Multi-Behavior Recommendation | ICDM |https://arxiv.org/abs/2109.02859|
| 2022 |Contrastive Meta Learning with Behavior Multiplicity for Recommendation | WSDM |https://arxiv.org/abs/2202.08523|
| 2023 |Multi-behavior Self-supervised Learning for Recommendation | SIGIR |https://dl.acm.org/doi/abs/10.1145/3539618.3591734|
| 2023 |Multi-Relational Contrastive Learning for Recommendation | RecSyS |https://arxiv.org/abs/2309.01103|
| 2024 |Contrastive Clustering Learning for Multi-Behavior Recommendation | TOIS |https://dl.acm.org/doi/10.1145/3698192|
| 2019 |Neural Multi-task Recommendation from Multi-behavior Data | ICDE |https://ieeexplore.ieee.org/document/8731537|
| 2020 |Efficient Heterogeneous Collaborative Filtering without Negative Sampling for Recommendation| AAAI |https://yongfeng.me/attach/chen-aaai2020.pdf|
| 2021 |Graph Meta Network for Multi-Behavior Recommendationn| SIGIR |https://dl.acm.org/doi/abs/10.1145/3404835.3462972|
| 2023 |Hierarchical Projection Enhanced Multi-behavior Recommendation| KDD |https://dl.acm.org/doi/abs/10.1145/3580305.3599838|
| 2021 |Knowledge-Enhanced Hierarchical Graph Transformer Network for Multi-Behavior Recommendation| |https://arxiv.org/abs/2110.04000|
| 2023 |Knowledge Enhancement for Contrastive Multi-Behavior Recommendation| WSDM |https://arxiv.org/abs/2301.05403|
| 2023 |Contrastive Learning-based Multi-behavior Recommendation with Semantic Knowledge Enhancement| ICDM |https://ieeexplore.ieee.org/document/10415825|
| 2024 |Knowledge-Enhanced Multi-Behaviour Contrastive Learning for Effective Recommendation| RecSyS |https://dl.acm.org/doi/10.1145/3640457.3688186|




## 🤝 Contributing

We welcome contributions! You can help by:

- Implementing one of the reviewed models
- Adding new research papers to the taxonomy
- Improving diagrams or summaries
- Providing benchmarks or datasets
- Participating in discussions and giving feedback on open issues

## 📄 Citation

If you use this survey, please cite our work:

```bibtex
@article{multi_behavior_survey_2025,
  title={Multi-Behavior Recommendation in the Deep Learning Era: Models, Optimization, and Open Challenges},
  author={Anonymous},
  year={2025}
}
```

## 🙌 Acknowledgements

This README accompanies our full research survey. All diagrams and model summaries are adapted from the paper.
