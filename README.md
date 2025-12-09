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
| ---- | Contrastive Meta Learning with Behavior Multiplicity for Recommendation | ---- | https://arxiv.org/abs/2202.08523 |
| ---- | A Self-Supervised Mixture-of-Experts Framework for Multi-behavior Recommendation | ---- | https://arxiv.org/abs/2508.19507 |
| ---- | Self-supervised Graph Neural Networks for Multi-behavior Recommendation | ---- | https://www.ijcai.org/proceedings/2022/285 |
| ---- | Knowledge-Enhanced Hierarchical Graph Transformer Network for Multi-Behavior Recommendation | ---- | https://arxiv.org/abs/2110.04000 |
| ---- | Multi-behavior Recommendation with Graph Convolutional Networks | ---- | https://dl.acm.org/doi/10.1145/3397271.3401072 |
| ---- | Multiplex Graph Neural Networks for Multi-behavior Recommendation | ---- | https://dl.acm.org/doi/pdf/10.1145/3340531.3412119 |

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
