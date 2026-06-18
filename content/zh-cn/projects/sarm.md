+++
title = "SARM 视觉增强框架"
description = "顶刊学术成果与省部级重点课题工程化：基于 Python/PyTorch 框架实现水下图像增强网络，打通物理先验与状态空间模型 (Mamba) 的深度整合。"
weight = 40
translationKey = "project-sarm"
featured_image = "/images/SARM/img.png"
tags = ["计算机视觉", "深度学习", "Mamba", "图像增强", "省部级课题"]
+++

### 项目概述
* 周期：2025.7 – 2026.5
* 项目类别：省部级重点课题支撑项目
* 担任角色：第一作者
* 研究依托：
  * 交通运输部长江航务管理局科技重点项目 (2025-020-6-Z-Y)
  * 湖北省交通运输厅科技项目 (2024BCB101)
  * 湖北省重点研发项目 (2024-81-3-3)

![SARM Model Architecture](/images/SARM/architecture.png)
![SARM Model Architecture](/images/SARM/IGAB.png)

### 核心技术与贡献
本项目旨在将前沿的水下图像增强 (UIE) 理论转化为解决真实水域探测痛点的工程应用。该核心研究成果我作为第一作者，于 2026 年 5 月被 JCR Q1 区期刊《Remote Sensing》正式录用。

* **面向真实需求的算法架构设计**：在多项省部级/厅局级重点科技项目的联合资助与依托下，聚焦于复杂退化水下场景的视觉增强难题，为实际的航务与交通水下探测任务提供底层视觉算法支撑。
* **物理先验与状态空间模型融合**：基于 Python 与 PyTorch 框架，在代码层面成功打通了传统水下成像物理先验知识与 State Space Models (Mamba 架构) 的深度整合，创新性地构建了 Scene-Aware Retinex Mamba (SARM) 网络模型。
* **高效的模型训练与反向调优**：针对极其复杂的真实水下退化数据，设计并实现了高效的特征提取模块与定制化损失函数。通过对网络进行精细化调优，大幅提升了模型在前向传播与反向梯度更新中的收敛效率及鲁棒性。