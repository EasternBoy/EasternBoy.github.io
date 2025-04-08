---
title: "Connectivity-preserving distributed informative path planning for mobile robot networks"
collection: publications
category: manuscripts
permalink: /publication/2024_RAL_IPP
excerpt: ''
date: 2024-05-15
venue: 'IEEE Robotics and Automation Letters, vol. 9, no. 3, pp. 2949-2956, March'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10531062'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'H. Nguyen, B. Nguyen, H. -G. Lee and H. -S. Ahn, "Observer-Based Control for Linear Continuous-Time Systems With Fully Homomorphic Encryption," in IEEE Transactions on Control of Network Systems, vol. 12, no. 1, pp. 700-712, March 2025'
---
This letter addresses the distributed informative path planning (IPP) problem for a mobile robot network to optimally explore a spatial field. Each robot is able to gather noisy environmental measurements while navigating the environment and build its own model of a spatial phenomenon using the Gaussian process and local data. The IPP optimization problem is formulated in an informative way through a multi-step prediction scheme constrained by connectivity preservation and collision avoidance. The shared hyperparameters of the local Gaussian process models are also arranged to be optimally computed in the path planning optimization problem. By the use of the proximal alternating direction method of multiplier, the optimization problem can be effectively solved in a distributed manner. It theoretically proves that the connectivity in the network is maintained over time whilst the solution of the optimization problem converges to a stationary point. The effectiveness of the proposed approach is verified in synthetic experiments by utilizing a real-world dataset.