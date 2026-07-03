---
title: "AD-MPCC: Adaptive Differentiable Model Predictive Contouring Control for Autonomous Racing"
excerpt: '<br/><img src="/images/paper_abstract/AD-MPCC-architecture.png" width="420"> <img src="/images/paper_abstract/AD-MPCC-single.gif" width="320">'
collection: portfolio
paperurl: "https://arxiv.org/abs/2607.00141"
---

<p align="center">
  <img src="/images/paper_abstract/AD-MPCC-architecture.png" width="760" alt="AD-MPCC architecture">
</p>

**AD-MPCC** integrates differentiable Model Predictive Contouring Control (MPCC)
with online Pacejka tire-parameter estimation for autonomous racing under
changing road-surface conditions. The controller adapts both the tire model and
the MPCC objective weights online, enabling stable high-speed racing when the
friction profile changes across the track.

**Sources:** [arXiv paper](https://arxiv.org/abs/2607.00141) |
[source code](https://github.com/nxt-lab/AD-MPCC) |
[IROS 2026](https://2026.ieee-iros.org/) |
[F1TENTH Gym](https://github.com/f1tenth/f1tenth_gym)

## Paper

**AD-MPCC: Adaptive Differentiable Model Predictive Contouring Control for
Autonomous Racing**

Nam T. Nguyen, Binh Nguyen, Ahmad Amine, Thanh Vo-Duy, Rahul Mangharam, and
Truong X. Nghiem.

## Method Overview

AD-MPCC combines three components at each control step:

- **Online parameter estimation:** a prior-regularized moving-horizon estimator
  with exponentially decaying weights updates Pacejka tire parameters to track
  surface transitions in real time.
- **Differentiable MPCC:** implicit-function-theorem sensitivities of the MPCC
  solution with respect to objective weights identify high-performing MPCC
  weight choices.
- **PaIML adaptation:** a Pacejka-informed machine learning model maps the
  estimated tire/surface state to MPCC weights for real-time control.

## Simulation Figures

### Single-Surface Scenario

All controllers are evaluated on a uniform surface with `mu_max = 1.2` for 10
laps. Diff-MPCC and AD-MPCC reduce lap time by about 11 seconds compared with
the fixed-weight baseline, while AD-MPCC gives the smallest mean lateral offset.

<p align="center">
  <img src="/images/paper_abstract/AD-MPCC-single.gif" width="760" alt="AD-MPCC single-surface simulation">
</p>

| Controller | Avg. Lap Time (s) | Avg. vx (m/s) | Avg. Lateral Offset (m) | Avg. Comp. Time (ms) |
|:---:|---:|---:|---:|---:|
| MPCC | 75.57 | 11.38 | 1.953 | 20.45 |
| A-MPCC | 75.62 | 11.41 | 1.815 | 21.21 |
| Diff-MPCC | **64.08** | **13.59** | 1.040 | 23.56 |
| AD-MPCC | 64.89 | 13.50 | **0.926** | 24.18 |

### Multi-Surface Scenario

The multi-surface race varies from `mu_max = 0.7` to `mu_max = 1.2` across
different track sections. In the reported experiments, AD-MPCC is the only
controller that completes the lap; MPCC, A-MPCC, and Diff-MPCC crash at the
first low-friction segment.

<p align="center">
  <img src="/images/paper_abstract/AD-MPCC-multiple.gif" width="760" alt="AD-MPCC multi-surface simulation">
</p>

| Controller | Avg. Lap Time (s) | Avg. vx (m/s) | Avg. Lateral Offset (m) |
|:---:|---:|---:|---:|
| MPCC | crashed | - | - |
| A-MPCC | crashed | - | - |
| Diff-MPCC | crashed | - | - |
| **AD-MPCC** | **74.9** | **11.65** | **1.069** |

## Citation

```bibtex
@misc{nguyen2026admpccadaptivedifferentiablemodel,
      title={AD-MPCC: Adaptive Differentiable Model Predictive Contouring Control for Autonomous Racing},
      author={Nam T. Nguyen and Binh Nguyen and Ahmad Amine and Thanh Vo-Duy and Rahul Mangharam and Truong X. Nghiem},
      year={2026},
      eprint={2607.00141},
      archivePrefix={arXiv},
      primaryClass={cs.RO},
      url={https://arxiv.org/abs/2607.00141},
}
```
