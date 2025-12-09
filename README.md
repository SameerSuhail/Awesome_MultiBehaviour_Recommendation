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
| 2015 | Recurrent Log-Bilinear Models for Next-Basket Recommendation | IEEE TKDE | N/A |
| 2018 | Behavioral Intent Neural Network for Recommendation (BINN) | SIGIR | N/A |
| 2021 | Intent-Aware Recommender Systems | CIKM | N/A |
| 2021 | Multi-Relational Interaction Graph for Recommendation | AAAI | N/A |
| 2022 | Graph Prompt Learning for Heterogeneous Sequential Recommendation | SIGIR | N/A |
| 2022 | Transformer-based Graph Transformer for Recommendation | KDD | N/A |
| 2024 | Graph Hierarchical Temporal Deep Learning for Recommendation | WWW | N/A |
| 2025 | Temporal-Aware Graph Contrastive Learning | AAAI | N/A |
| 2024 | Multi-Behavior Generative Recommendation | KDD | N/A |
| 2025 | Generative Adaptive Multi-Behavior Recommendation | WWW | N/A |
| 2025 | Intent-Conditioned Diffusion for Recommendation | AAAI | N/A |
| 2025 | Multi-Behavior Diffusion-based Sequential Recommendation | SIGIR | N/A |
| 2025 | Generative Recommendation via Journey-Aware Sparse Attention | WWW | N/A |
| 2022 | Multi-Behavior Knowledge-Aware Reinforcement Learning | AAAI | N/A |
| 2023 | Multi-Behavior Session-Based Recommendation via Graph Reinforcement Learning | CIKM | N/A |
| 2020 | Multi-Behavior Recommendation with Graph Convolutional Networks | AAAI | https://dl.acm.org/doi/10.1145/3397271.3401072 |
| 2021 | Multi-Behavior Enhanced Recommendation with Cross-Interaction Collaborative Relation Modeling | ICDE | N/A |
| 2024 | Multi-Behavior Graph Neural Networks for Recommender Systems | IEEE TNNLS | N/A |
| 2024 | HEC-GCN: Hypergraph Enhanced Cascading GCN | arXiv | https://arxiv.org/abs/2412.14476 |
| 2024 | Multi-Behavior Partial Order Graph Convolutional Network | arXiv | https://arxiv.org/abs/2402.07659 |
| 2021 | Hyper Meta-Path Contrastive Learning for Multi-Behavior Recommendation | ICDM | N/A |
| 2022 | Contrastive Meta Learning with Behavior Multiplicity | WSDM | https://arxiv.org/abs/2202.08523 |
| 2023 | Multi-Relational Contrastive Learning for Recommendation | arXiv | https://arxiv.org/abs/2309.01103 |
| 2024 | Contrastive Clustering Learning for Multi-Behavior Recommendation | TOIS | N/A |
| 2023 | Multi-Behavior Self-Supervised Learning for Recommendation | SIGIR | N/A |
| 2019 | Neural Multi-task Recommendation from Multi-behavior Data | ICDE | N/A |
| 2021 | Graph Meta Network for Multi-Behavior Recommendation | SIGIR | N/A |
| 2023 | Hierarchical Projection Enhanced Multi-Behavior Recommendation | KDD | N/A |
| 2020 | Efficient Heterogeneous Collaborative Filtering | SIGIR | N/A |
| 2021 | Knowledge-Enhanced Hierarchical Graph Transformer Network | arXiv | https://arxiv.org/abs/2110.04000 |
| 2023 | Knowledge-Enhanced Multi-Behavior Contrastive Learning | CIKM | N/A |
| 2023 | Contrastive Learning with Semantic Knowledge Enhancement | ICDM | https://doi.org/10.1109/ICDM58522.2023.00200 |
| 2024 | Knowledge-Enhanced Multi-Behavior Contrastive Learning | KDD | N/A |


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
