---
title: "Physics-Informed Data-Driven Modeling of HVAC Systems: A Systematic Analysis"
collection: publications
category: manuscripts
permalink: /publication/2026_ACCESS_PIML-HVAC
excerpt: ''
date: 2026-01-12
venue: EEE Access, vol. 14, pp. 6481-6500
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
# paperurl: 'https://ieeexplore.ieee.org/abstract/document/10531062'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'H. Nguyen, B. Nguyen, H. -G. Lee and H. -S. Ahn, "Observer-Based Control for Linear Continuous-Time Systems With Fully Homomorphic Encryption," in IEEE Transactions on Control of Network Systems, vol. 12, no. 1, pp. 700-712, March 2025'
---
Heating, ventilation, and air conditioning (HVAC) systems account for a significant portion of energy consumption in developed countries. Accurately identifying their dynamics is crucial for developing effective controllers. However, it is challenging due to the system’s nonlinearities and variations across building types. Data-driven approaches have shown great promise in modeling the dynamics of HVAC systems, replacing traditional ordinary differential equations. However, relying solely on data can lead to poor generalization, particularly when the training data is limited or when unknown disturbances, such as weather conditions and occupant behavior, are present. Physics-informed machine learning (PIML) techniques have been developed for integrating physical principles into machine learning methods to improve the accuracy and data efficiency of modeling of dynamical systems. This paper investigates PIML techniques that incorporate three different physical properties: monotonicity, boundedness, and system structure. These models are benchmarked against physics-agnostic machine learning (PAML) approaches and the gray-box modeling technique to further highlight the performance of PIML models in terms of accuracy, robustness, and data efficiency for modeling HVAC systems from real data. Experimental data collected from a real-world HVAC system are used for systematically studying and analyzing thirteen gray-box, PAML, and PIML modeling techniques in different scenarios. Our results demonstrate that PIML models outperform PAML models in predicting the temperature dynamics of HVAC systems, especially when the training data is limited, unreliable, or noisy, with accurate and robust performance. Furthermore, we identify which physical properties are the most beneficial for enhancing machine learning performance for HVAC system identification.