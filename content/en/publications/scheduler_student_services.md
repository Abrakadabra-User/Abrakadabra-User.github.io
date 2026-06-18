---
title: "SARM: Scene-Aware Retinex Mamba for Underwater Image Enhancement"
date: 2026-05-20
featured_image: "/images/SARM/img.png"
tags: ["Computer Vision", "Underwater Image Enhancement", "State Space Models", "Deep Learning"]
---

## Abstract
This paper addresses the degradation of underwater images under complex lighting conditions by proposing a self-supervised framework called **SARM**, which integrates Retinex theoretical priors with State Space Models (Mamba). By employing a scene-aware adapter for dynamic feature gating, the framework achieves high-fidelity underwater image enhancement while maintaining O(HW) linear inference complexity.

## Network Architecture
![SARM Model Architecture](/images/SARM/architecture.png)
![SARM Model Architecture](/images/SARM/IGAB.png)

## Key Achievements
* **Publication**: *Remote Sensing* (JCR Q1, IF: 4.1).
* **Main Advantages**: 
    * Utilizes a 2D selective scan mechanism to ensure global context modeling while enabling real-time inference.
    * Incorporates a Scene-Aware Adapter (SAA) to effectively suppress non-uniform scattering noise and color casts.

* **Performance**: Achieved state-of-the-art (SOTA) performance across multiple benchmark datasets, including UIEB and EUVP.
![SARM Model Architecture](/images/SARM/Table1.png)


## Project Timeline

<div class="timeline">
  <ul>
    <li><strong>July 2025</strong>: Defined research topic; completed literature review and domain survey.</li>
    <li><strong>Aug. 2025</strong>: Implemented baseline model modifications and designed the initial illumination estimator prototype.</li>
    <li><strong>Aug. 2025</strong>: Identified performance inconsistencies in varying degradation scenarios and proposed the core innovation: the Scene-Aware Adapter (SAA).</li>
    <li><strong>Oct. 2025</strong>: Integrated the State Space Model (Mamba) architecture to enhance long-sequence modeling and image restoration quality.</li>
    <li><strong>Nov. 2025</strong>: Designed and implemented a pseudo-label generation strategy to overcome the bottleneck of poor paired training data quality.</li>
    <li><strong>Feb. 2026</strong>: Conducted comprehensive ablation and comparative experiments; completed the initial manuscript.</li>
    <li><strong>Mar. 2026</strong>: Refined and polished the manuscript under the guidance of my supervisor and senior lab colleagues.</li>
    <li><strong>Mar. 13, 2026</strong>: Formally submitted the manuscript to <em>Remote Sensing</em>.</li>
    <li><strong>Apr. 27, 2026</strong>: Received initial review feedback (3 Minor, 1 Major); academic editor provided a "pre-acceptance" assessment.</li>
    <li><strong>May 14, 2026</strong>: Revised manuscript approved by all reviewers; academic editor requested minor final adjustments.</li>
    <li><strong>May 18, 2026</strong>: Manuscript officially accepted by <em>Remote Sensing</em> (JCR Q1).</li>
    <li><strong>May 20, 2026</strong>: Paper officially published online.</li>
  </ul>
</div>

## Resource Links
- 📄 [View Full PDF](https://doi.org/10.3390/rs18101652) (MDPI Official Link)
- 💻 [GitHub Repository](https://github.com/your-username/SARM)

## Visual Comparison(Click to view full size)

### 1. Benchmark Datasets 
<div style="display: flex; gap: 20px; align-items: flex-start;">
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/UIEB.jpg" target="_blank">
      <img src="/images/SARM/UIEB.jpg" width="200" class="hover-zoom" alt="UIEB">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">UIEB Dataset</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/EUVP.jpg" target="_blank">
      <img src="/images/SARM/EUVP.jpg" width="200" class="hover-zoom" alt="EUVP">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">EUVP Dataset</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/UCCS.jpg" target="_blank">
      <img src="/images/SARM/UCCS.jpg" width="200" class="hover-zoom" alt="UCCS">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">UCCS Dataset</figcaption>
  </figure>
</div>

### 2. Feature Analysis & Model Robustness
<div style="display: flex; flex-wrap: wrap; gap: 10px;">
  <div style="width: 48%; text-align: center;">
    <img src="/images/SARM/rgb.jpg" alt="RGB channel enhancement">
    <p style="font-size: 0.85em;">RGB Channel Consistency Analysis</p>
  </div>
  <div style="width: 48%; text-align: center;">
    <img src="/images/SARM/Ablation_Result_Transposed.jpg" alt="Ablation studies">
    <p style="font-size: 0.85em;">Ablation Study</p>
  </div>
</div>

### 3. Downstream Task Verification
<div style="display: flex; flex-wrap: wrap; gap: 10px;">
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Canny.jpg" alt="Edge detection">
    <p style="font-size: 0.85em;">Edge Detection Comparison</p>
  </div>
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Dots.png" alt="Feature point matching">
    <p style="font-size: 0.85em;">Key Feature Point Matching Visualization</p>
  </div>
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Segmentation.jpg" alt="Downstream segmentation">
    <p style="font-size: 0.85em;">Marine Semantic Segmentation</p>
  </div>
</div>
