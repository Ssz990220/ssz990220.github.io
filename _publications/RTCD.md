---
title: "Hardware-Accelerated Ray Tracing for Discrete and Continuous Collision Detection on GPUs"
collection: publications
permalink: /publication/RTCD
excerpt: 'GPU ray tracing accelerates mesh-to-mesh collision checks for discrete robot poses and swept-sphere checks along continuous robot trajectories.'
github: 'https://github.com/Ssz990220/RTCollisionDetection'
date: 2025-09-02
venue: 'IEEE International Conference on Robotics and Automation (ICRA)'
paperurl: 'https://doi.org/10.1109/ICRA55743.2025.11128528'
citation: 'S. Sui, L. Sentis, and A. Bylard, “Hardware-Accelerated Ray Tracing for Discrete and Continuous Collision Detection on GPUs,” 2025 IEEE International Conference on Robotics and Automation (ICRA), 2025.'
---
We use hardware-accelerated GPU ray tracing to check robot collisions at discrete poses and along continuous trajectories. The discrete method tests robot link meshes directly against obstacle meshes. The continuous method approximates the robot with spheres and checks the volumes they sweep along piecewise-linear or quadratic B-spline paths.

[IEEE Xplore](https://doi.org/10.1109/ICRA55743.2025.11128528) · [arXiv preprint](https://arxiv.org/abs/2409.09918) · [Code on GitHub](https://github.com/Ssz990220/RTCollisionDetection)

## Algorithms
![](../images/RTCD/RTCD.png)
Demonstration of our collision detection methods: discrete-pose collision detection by ray-tracing (a) along obstacle meshes  and (b) along robot meshes, and continuous collision detection by ray-tracing against swept sphere-approximated robot volumes (c) along piecewise-linear paths or (d) along quadratic B-spline paths.

## Method
<img src="../images/RTCD/RT2.gif" alt="drawing" width="400"/>

## Result
![](../images/RTCD/DCDResult.png)
![](../images/RTCD/CCDResult.png)

The arXiv preprint reports speedups of up to 3× for batched discrete-pose queries and up to 9× for continuous queries. The ICRA paper reports up to 2.8× for batched discrete-pose queries and up to 7× for continuous queries in its reported test conditions.
