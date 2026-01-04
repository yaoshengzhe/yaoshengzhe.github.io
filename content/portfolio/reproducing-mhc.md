---
title: "Reproducing mHC"
tagline: "Manifold-Constrained Hyper-Connections for Stable Deep Networks"
weight: 1
featured: true
github: "https://github.com/yaoshengzhe/reproducing-mhc"
blog: "/posts/reproducing-mhc/"
status: "completed"
category: "research"
tech:
  - PyTorch
  - Sinkhorn-Knopp
  - Birkhoff Polytope
cover:
  image: "https://raw.githubusercontent.com/yaoshengzhe/reproducing-mhc/main/images/stability_detailed.png"
---

A PyTorch implementation that validates DeepSeek's mHC paper. The paper extends Hyper-Connections by constraining weight matrices to the Birkhoff polytope using Sinkhorn-Knopp normalization, achieving significantly more stable training dynamics.

**Reproduction results:**

- Confirmed the paper's stability claims with independent experiments
- mHC activation gain: 11.70 vs 61.33 for standard Hyper-Connections (5x reduction)
- Gradient stability: max norm of 4.46, enabling deeper networks without exploding gradients
- Convergence: achieved minimum loss of 1.787, outperforming all baselines
