---
title: "Real-time distributed trajectory planning for mobile robots"
collection: publications
category: conferences
permalink: /publication/2023_IFAC_RT-Dist-Plan
excerpt: ''
date:  02 July 2023 
venue: 'IFAC-PapersOnLine'
# slidesurl: 'http://academicpages.github.io/files/slides2.pdf'
paperurl: 'https://www.sciencedirect.com/science/article/pii/S2405896323015239'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Efficiently planning trajectories for nonholonomic mobile robots in formation tracking is a fundamental yet challenging problem. Nonholonomic constraints, complexity in collision avoidance, and limited computing resources prevent the robots from being practically deployed in realistic applications. This paper addresses these difficulties by modeling each mobile platform as a nonholonomic motion and formulating trajectory planning as an optimization problem using model predictive control (MPC). That is, the optimization problem is subject to both nonholonomic motions and collision avoidance. To reduce computing costs in real time, the nonholonomic constraints are convexified by finding the closest nominal points to the nonholonomic motion, which are then incorporated into a convex optimization problem. Additionally, the predicted values from the previous MPC step are utilized to form linear avoidance conditions for the next step, preventing collisions among robots. The formulated optimization problem is solved by the alternating direction method of multiplier (ADMM) in a distributed manner, which makes the proposed trajectory planning method scalable. More importantly, the convergence of the proposed planning algorithm is theoretically proved while its effectiveness is validated in a synthetic environment.