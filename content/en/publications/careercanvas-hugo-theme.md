---
title: "The Invisible Spotlight: Reconstructing Fan Votes and Optimizing Scoring Mechanisms"
date: 2026-02-01
description: "2026 Mathematical Contest in Modeling (MCM/ICM) - Finalist"
featured_image: "/images/MCM2026/1.jpg"
tags: ["Mathematical Modeling", "Bayesian Inference", "ACO-LMM Framework", "Mechanism Design"]
---

## Problem Background
Reality television programs, such as *Dancing with the Stars* (DWTS), face a fundamental "binary paradox": the conflict between technical fairness and commercial value. Integrating professional evaluation (judges' scores) with public engagement (fan votes) has historically led to systemic controversies, as traditional scoring mechanisms often fail to balance technical merit with the "underdog" narratives favored by the audience.

## Methodology

### 1. Inverse Vote Reconstruction (Task 1: IBRM Model)
* **Challenge**: Fan voting data is proprietary and functions as a "black box."
* **Method**: Developed an **Inverse Bayesian Reconstruction Model (IBRM)**. By employing Monte Carlo Rejection Sampling to approximate the posterior distribution of fan votes based on observed elimination outcomes, we successfully decoded latent voting patterns.

### 2. Counterfactual Diagnostic Framework (Task 2: Simulation Engine)
* **Discovery**: Through a Counterfactual Simulation Engine, we identified the **"Variance Imbalance Principle."**
* **Insight**: The existing percentage-based system suffers from high fan-vote variance, enabling a form of "populism" that overshadows "meritocracy." Consequently, technically superior contestants (e.g., Tinashe) are frequently eliminated due to insufficient fan engagement.

### 3. Preference Decomposition Analysis (Task 3: Hybrid ACO-LMM Framework)
* **Innovation**: Developed a **Hybrid ACO-LMM framework**, integrating Ant Colony Optimization (ACO) for objective feature selection with Linear Mixed Models (LMM) to decompose hierarchical effects.
* **Results**: Quantitative analysis revealed a critical axiological misalignment: judges prioritize competitive sports logic, while fans favor "underdog" narratives. This divergence is identified as the sociological root of format failure.

### 4. Mechanism Design (Task 4: GPD System)
* **Design**: Proposed the **Grand Prix Dynamic (GPD) System**.
* **Core Logic**:
    * **F1 Scoring Structure**: Introduced non-linear point mapping to establish a "meritocracy firewall," mitigating the impact of short-term voting fluctuations on long-term outcomes.
    * **Sigmoid Dynamic Weights**: Implemented a temporal decay function to transition from entertainment-oriented weighting in early stages to competitiveness-oriented weighting in later stages.
    * **Dance-Off Protocol**: Integrated an immediate, high-pressure showdown as a final safeguard to ensure competitive integrity.

## Validation
* **Pareto Optimality**: Ablation studies confirmed that the GPD system achieves global Pareto optimality, maintaining high Fan Efficacy (0.76) while ensuring Professional Elitism (0.95).
* **Robustness**: The "Bobby Bones Stress Test" verified the system's resilience in balancing commercial success with competitive integrity.

## Resources

<div style="margin: 20px 0;">
  <a href="/files/mcmthesis-2026-2624237.pdf" target="_blank" style="padding: 12px 24px; background-color: #007BFF; color: white; text-decoration: none; border-radius: 5px; font-weight: bold; font-size: 16px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
    📄 View Full Paper (PDF)
  </a>
</div>
---