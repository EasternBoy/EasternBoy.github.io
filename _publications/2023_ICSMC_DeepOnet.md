---
title: "Causal Deep Operator Networks for Data-Driven Modeling of Dynamical Systems"
collection: publications
category: conferences
permalink: /publication/2023_ICSMC_DeepOnet
excerpt: ''
date: 2023-10-01
venue: '2023 IEEE International Conference on Systems, Man, and Cybernetics (SMC)'
# slidesurl: 'http://academicpages.github.io/files/slides3.pdf'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10394294'
# citation: 'Your Name, You. (2015). &quot;Paper Title Number 3.&quot; <i>Journal 1</i>. 1(3).'
---

The deep operator network (DeepONet) architecture is a promising approach for learning functional operators, that can represent dynamical systems described by ordinary or partial differential equations. However, it has two major limitations, namely its failures to account for initial conditions and to guarantee the temporal causality – a fundamental property of dynamical systems. This paper proposes a novel causal deep operator network (Causal-DeepONet) architecture for incorporating both the initial condition and the temporal causality into data-driven learning of dynamical systems, overcoming the limitations of the original DeepONet approach. This is achieved by adding an independent root network for the initial condition and independent branch networks conditioned, or switched on/off, by time-shifted step functions or sigmoid functions for expressing the temporal causality. The proposed architecture was evaluated and compared with two baseline deep neural network methods and the original DeepONet method on learning the thermal dynamics of a room in a building using real data. It was shown to not only achieve the best overall prediction accuracy but also enhance substantially the accuracy consistency in multistep predictions, which is crucial for predictive control.