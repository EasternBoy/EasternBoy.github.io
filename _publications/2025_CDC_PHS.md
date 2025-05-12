---
title: "Structure- and stability-preserving learning-based model order reduction for port-Hamiltonian systems  "
collection: publications
category: conferences
permalink: /publication/2025_CDC_PHS
excerpt: ''
date:  09 Dec 2025 - 12 Dec 2025 
venue: '2025 Conference on Decision and Control (CDC)'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
# paperurl: 'https://arxiv.org/abs/2403.16489'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

This paper addresses the problem of data-driven
model order reduction for port-Hamiltonian systems while
preserving their intrinsic Hamiltonian structure and
stability. We propose a novel approach that, unlike
existing methods, does not require the availability of
samples of the Hamiltonian and its gradient within the
training data. Our method employs a Petrov–Galerkin
projection approach and introduces a neural network-based
approximation technique designed to learn the Hamiltonian
while explicitly preserving equilibrium conditions
characterized by the vanishing gradient of the Hamiltonian.
Conventional neural network-based Hamiltonian
approximations often impose convexity constraints, which
can limit the expressiveness and generalization of the
learned models. In contrast, our approach relaxes this
convexity requirement, enabling the adoption of more
general non-convex models to enhance flexibility and
performance. A numerical experiment is
presented to validate the effectiveness of the proposed
method, demonstrating its capability to achieve accurate
structure- and stability-preserving order reduction for
port-Hamiltonian systems. 