+++
title = "Satellite Constellation Spatial Computing and Multi-Task Scheduling Engine"
description = "Achieved high-precision simulation of multi-satellite ground coverage and optimal scheduling of observation tasks based on spherical grid divide-and-conquer algorithms and dynamic programming."
weight = 50
translationKey = "project-satellite"
featured_image = "/images/project/5.png"
tags = ["Spatial Computing", "Algorithm Design", "Dynamic Programming", "Operations Optimization"]
+++

### Project Overview
* Duration: 2026.3 – 2026.5
* Project Category: Spatial Computing Engine
* Role: Algorithm R&D

### Core Technologies & Contributions
Addressing the complex spatio-temporal constraint problems in multi-satellite collaborative ground observation, I built a simulation engine from scratch encompassing high-precision spatial coverage calculation and optimal task scheduling.

* **Spherical Grid Divide-and-Conquer and Integral Solving**: Abandoned conventional planar approximation to accurately calculate coverage area using spherical integral formulas. Designed and implemented a divide-and-conquer algorithm for spatial grids to precisely determine the multiple coverage time windows of the satellites' conical service areas on the Earth's surface, strictly controlling the area calculation error to under 0.1%.
* **Dynamic Programming Scheduling under Multiple Constraints**: Targeting the multi-objective, multi-satellite resource allocation problem, designed and implemented dynamic programming and greedy scheduling algorithms under the dual constraints of strict visible time windows and minimum satellite transition times (e.g., 20s-35s), achieving the maximization of observation benefits (total weights) within a massive solution space.
* **Simulation System and Dynamic Visualization**: Independently completed the underlying data parsing and system architecture, and developed a visualization interface. Achieved the dynamic generation of satellite instantaneous coverage curves and the precise statistical display of target observation time gaps.