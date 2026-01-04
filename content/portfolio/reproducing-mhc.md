---
title: "Reproducing mHC"
tagline: "Manifold-Constrained Hyper-Connections for Stable Deep Networks"
weight: 1
github: "https://github.com/yaoshengzhe/reproducing-mhc"
blog: "/posts/reproducing-mhc/"
tech:
  - PyTorch
  - Sinkhorn-Knopp
  - Birkhoff Polytope
cover:
  image: "https://raw.githubusercontent.com/yaoshengzhe/reproducing-mhc/main/images/stability_detailed.png"
---

A PyTorch implementation validating DeepSeek's mHC paper, which extends Hyper-Connections with manifold constraints for improved neural network training stability.

**Key results from reproduction:**

- Validated the paper's core stability claims
- mHC achieves lowest activation gain (11.70 vs 61.33 for HC)
- Superior gradient stability with max gradient norm of 4.46
- Best convergence with minimum loss of 1.787
