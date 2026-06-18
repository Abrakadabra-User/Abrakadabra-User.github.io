---
title: "SARM: 场景感知水下图像增强框架"
date: 2026-05-20
featured_image: "/images/SARM/img.png"
tags: ["计算机视觉", "水下图像增强", "状态空间模型", "深度学习"]
---

## 摘要
本文针对水下图像在复杂光照下的退化问题，提出了一种融合 Retinex 理论先验与状态空间模型 (Mamba) 的自监督框架——**SARM**。该方法通过场景感知适配器实现动态特征门控，在保持 O(HW) 线性推理复杂度的同时，实现了水下图像的高保真增强。

## 网络架构 
![SARM 模型架构](/images/SARM/architecture.png)
![SARM 模型架构](/images/SARM/IGAB.png)

## 核心成果
* **学术发表**: *Remote Sensing* (JCR Q1, 影响因子: 4.1).
* **主要优势**: 
    * 采用 2D 选择性扫描机制，在保证全局上下文建模的同时实现实时推理。
    * 引入场景感知适配器 (SAA)，有效抑制了不均匀散射噪声与复杂色偏。
* **实验表现**: 在 UIEB, EUVP 等多个基准数据集上达到 SOTA 水平。
![SARM 性能指标](/images/SARM/Table1.png)

## 项目时间线

<div class="timeline">
  <ul>
    <li><strong>2025年07月</strong>: 确定研究课题，完成领域内核心文献的综述与调研。</li>
    <li><strong>2025年08月</strong>: 在基准模型（Baseline）基础上进行创新尝试，完成照度估计器的初步原型设计。</li>
    <li><strong>2025年08月</strong>: 针对现有模型在不同退化程度场景下的不平衡表现，提出核心创新点——场景感知适配器 (SAA)。</li>
    <li><strong>2025年10月</strong>: 引入状态空间模型 (Mamba) 架构，通过优化长序列建模能力，显著提升了图像增强效果。</li>
    <li><strong>2025年11月</strong>: 为克服训练数据配对质量不佳带来的瓶颈，设计并实现伪标签生成策略以优化训练过程。</li>
    <li><strong>2026年02月</strong>: 完成消融实验与对比实验等，整理实验结果并完成初稿撰写。</li>
    <li><strong>2026年03月</strong>: 联系导师，在师兄指导下，对论文初稿进行深度润色。</li>
    <li><strong>2026年03月13日</strong>: 正式向 <em>Remote Sensing</em> 投递学术论文。</li>
    <li><strong>2026年04月27日</strong>: 收到一审反馈（3 Minor, 1 Major），学术编辑给出“审稿后录用”预判。</li>
    <li><strong>2026年05月14日</strong>: 修订稿获所有审稿人认可，学术编辑建议作最后细微调整。</li>
    <li><strong>2026年05月18日</strong>: 论文被 JCR Q1 期刊 <em>Remote Sensing</em> 正式录用。</li>
    <li><strong>2026年05月20日</strong>: 论文于期刊官网在线发表。</li>
  </ul>
</div>

## 资源传送门
- 📄 [点击查看 PDF 全文](https://doi.org/10.3390/rs18101652) (MDPI 官方链接)
- 💻 [GitHub 代码仓库](https://github.com/your-username/SARM) 

## 可视化对比 (点击图片可查看大图)

### 1. 基准数据集对比
<div style="display: flex; gap: 20px; align-items: flex-start;">
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/UIEB.jpg" target="_blank">
      <img src="/images/SARM/UIEB.jpg" width="200" class="hover-zoom" alt="UIEB">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">UIEB 数据集增强效果</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/EUVP.jpg" target="_blank">
      <img src="/images/SARM/EUVP.jpg" width="200" class="hover-zoom" alt="EUVP">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">EUVP 数据集质量提升</figcaption>
  </figure>
  <figure style="margin: 0; text-align: center;">
    <a href="/images/SARM/UCCS.jpg" target="_blank">
      <img src="/images/SARM/UCCS.jpg" width="200" class="hover-zoom" alt="UCCS">
    </a>
    <figcaption style="font-size: 0.8em; margin-top: 5px;">UCCS 真实水下场景</figcaption>
  </figure>
</div>

### 2. 特征分析与模型鲁棒性
<div style="display: flex; flex-wrap: wrap; gap: 10px;">
  <div style="width: 48%; text-align: center;">
    <img src="/images/SARM/rgb.jpg" alt="RGB channel enhancement">
    <p style="font-size: 0.85em;">RGB 通道一致性分析</p>
  </div>
  <div style="width: 48%; text-align: center;">
    <img src="/images/SARM/Ablation_Result_Transposed.jpg" alt="Ablation studies">
    <p style="font-size: 0.85em;">消融实验</p>
  </div>
</div>

### 3. 下游任务验证
<div style="display: flex; flex-wrap: wrap; gap: 10px;">
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Canny.jpg" alt="Edge detection">
    <p style="font-size: 0.85em;">边缘检测</p>
  </div>
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Dots.png" alt="Feature point matching">
    <p style="font-size: 0.85em;">关键特征点匹配可视化</p>
  </div>
  <div style="width: 32%; text-align: center;">
    <img src="/images/SARM/Segmentation.jpg" alt="Downstream segmentation">
    <p style="font-size: 0.85em;">水下语义分割任务验证</p>
  </div>
</div>