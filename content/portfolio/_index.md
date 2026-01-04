---
title: "Portfolio"
description: "Open source projects and research reproductions"
---

A collection of projects I've built and research I've reproduced. Each project represents a deep dive into a technical domain, from AI/ML research to developer tooling.

---

## Reproducing mHC

**Manifold-Constrained Hyper-Connections**

A PyTorch implementation validating DeepSeek's mHC paper, which extends Hyper-Connections with manifold constraints for improved neural network training stability.

**Key results:**
- Validated the paper's core stability claims through reproduction
- mHC achieves lowest activation gain (11.70 vs 61.33 for unconstrained HC)
- Superior gradient stability with maximum gradient norm of 4.46

**Tech:** PyTorch, Sinkhorn-Knopp algorithm, Birkhoff polytope projections

[View on GitHub](https://github.com/yaoshengzhe/reproducing-mhc)

---

## Autoloop

**Autonomous Agent Iteration**

A plugin for agentic tools like Claude Code that enables AI agents to work independently until a task is completed.

**What it does:**
- Transforms back-and-forth AI interaction into autonomous execution
- Self-correcting iterations that build on previous progress
- Safety controls with maximum iteration limits
- Full transparency through version control

**Example usage:**
```bash
/autoloop Build a REST API with tests --max-iterations 15
```

**Tech:** Shell scripting, Claude Code hooks, Git integration

[View on GitHub](https://github.com/yaoshengzhe/autoloop)
