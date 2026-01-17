# Reproducing Quantum State Designs from Chaotic Dynamics 

## Overview
This repository contains a computational study aimed at reproducing Figure 3b from the paper: ["Exact emergent quantum state designs from quantum chaotic dynamics" Wen Wei Ho & Soonwon Choi (2022)](https:/https://arxiv.org/pdf/2109.07491)
  

## The Physics: What is Figure 3b?
Figure 3b shows the Trace Distance of the k-th moment of the projected ensemble to a Haar random ensemble versus the projected subsystem size, $N_B$. 
Skeleton: 
-  We start with a system of N qubits and divide it into two parts - A & B. The state of B is projectively measured in the local computational basis.
-  The projective measurement results in a bit-string outcome, and we are interested in its associated pure quantum state on subsystem A.
-  The state of subsystem A and the possibility of that state form the projected ensemble.
-  The chain of qubits undergoes Floquet dynamics with no global conservation laws.
-  The comparison between the Haar random ensemble and the projected ensemble is captured by the trace distance between them.
-  As the projected subsystem size increases, the projected ensemble becomes more similar to a random Haar ensemble. 
## Implementation Journey 
I worked on this project during the summer before my junior year. At the time, with a background in introductory Quantum Mechanics, much of the many-body machinery was black-boxed and reverse-engineered. Since this project was a significant learning milestone, I also included my working notes to document my thought process and progress. 
## Current Status 
The current simulation is qualitatively consistent with the paper's result, capturing the characteristic decay towards the Haar-random ensemble. However, the quantitative values do not yet match the theoretical predictions. For example, the spike at N_b = 7 suggests that a thorough investigation is needed. To conduct this investigation, I am currently taking a course on Quantum Many-Body Physics. 
https://github.com/UguumuRR/Quantum-state-design-WIP/issues/1
*My current reproduced result*
![Figure 3b from the paper](jb-image:img_1768644191945_365d00239f78a8)
*Figure 3b from the paper*
## How to Run 
1. Ensure you have Numpy and QuTip installed.
2. Run the main reproduction script: https://github.com/UguumuRR/Quantum-state-design-WIP/blob/main/Fig3b_Final_Model.ipynb
