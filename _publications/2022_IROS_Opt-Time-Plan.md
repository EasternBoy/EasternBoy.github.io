---
title: "Collision-free minimum-time trajectory planning for multiple vehicles based on ADMM"
collection: publications
category: conferences
permalink: /publication/2022_IROS_Opt-Time-Plan
excerpt: ''
date:  23-10-2022 
venue: '2022 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10156635'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

The paper presents a practical approach for planning trajectories for multiple vehicles where both collision avoidance and minimum travelling time are simultaneously considered. It is first proposed to exploit the mixed-integer programming (MIP) approach to formulate the collision avoidance paradigm, where the linear dynamic models are utilized to derive the linear constraints. Moreover, travelling time of each vehicle is compromised among them and set to be minimized so that all the vehicles can practically reach the expected destinations at the shortest time. Unfortunately, the formulated optimization problem is NP-hard. In order to effectively address it, we propose to employ the alternating direction method of multipliers (ADMM), which can share the computational burdens to distributive optimization solvers. Thus, the proposed method can enable each vehicle to obtain an expected trajectory in a practical time.