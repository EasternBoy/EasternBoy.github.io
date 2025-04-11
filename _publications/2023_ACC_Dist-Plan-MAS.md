---
title: "Distributed formation trajectory planning for multi-vehicle systems"
collection: publications
category: conferences
permalink: /publication/2023_ACC_Dist-Plan-MAS
excerpt: ''
date:  31 May 2023 - 02 June 2023 
venue: '2023 American Control Conference (ACC)'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10156635'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

This paper addresses the problem of distributed formation trajectory planning for multi-vehicle systems with collision avoidance among vehicles. Unlike some previous distributed formation trajectory planning methods, our proposed approach offers great flexibility in handling computational tasks for each vehicle when the global formation of all the vehicles changes. It affords the system the ability to adapt to the computational capabilities of the vehicles. Furthermore, global formation constraints can be handled at any selected vehicles. Thus, any formation change can be effectively updated without recomputing all local formations at all the vehicles. To guarantee the above features, we first formulate a dynamic consensus-based optimization problem to achieve desired formations while guaranteeing collision avoidance among vehicles. Then, the optimization problem is effectively solved by ADMM-based or alternating projection-based algorithms, which are also presented. Theoretical analysis is provided not only to ensure the convergence of our method but also to show that the proposed algorithm can surely be implemented in a fully distributed manner. The effectiveness of the proposed method is illustrated by a numerical example of a 9-vehicle system.