# DSE-CDDE: Dynamic Segment Extractor with Cross-Dimensional Dependency Encoder for Traffic Flow Forecasting

[![Paper Status](https://img.shields.io/badge/Status-Under%20Review-yellow)](https://github.com/N2308490G/DSE-CDDE-Traffic-Forecasting)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 📢 Important Notice / 重要声明

**English:**
This repository contains the implementation code for our paper "DSE-CDDE: Dynamic Segment Extractor with Cross-Dimensional Dependency Encoder for Traffic Flow Forecasting," which is currently **under review** at IEEE Transactions on Transportation Electrification.

According to our university's research office regulations and academic integrity policies, we are **not permitted to publicly release the complete source code, datasets, or detailed implementation** until the paper has been **formally accepted for publication**.

This repository currently provides:
- Project structure and organization
- Code framework and module interfaces
- Documentation and usage guidelines
- Placeholder files for future code release

**The complete implementation code, trained models, and experimental data will be made publicly available immediately upon paper acceptance.**

---

**中文:**
本仓库包含我们论文《DSE-CDDE: 用于交通流预测的动态片段提取器与跨维度依赖编码器》的实现代码,该论文目前正在 **IEEE Transactions on Transportation Electrification 审稿中**。

根据我校科研院的规定和学术诚信政策,在论文**正式被接收发表之前**,我们**不允许公开发布完整的源代码、数据集或详细实现**。

本仓库当前提供:
- 项目结构和组织框架
- 代码框架和模块接口
- 文档和使用指南
- 未来代码发布的占位文件

**完整的实现代码、训练模型和实验数据将在论文被接收后立即公开发布。**

---

## 🎯 Overview

DSE-CDDE is a novel deep learning architecture specifically designed for robust traffic flow forecasting from noisy IoT sensor data. Our method introduces two core innovations:

1. **Dynamic Segment Extractor (DSE)**: Learns optimal temporal segmentation of traffic patterns through learnable boundaries, automatically adapting to different traffic regimes captured by IoT sensor networks.

2. **Cross-Dimensional Dependency Encoder (CDDE)**: Integrates self-supervised denoising mechanisms with cross-dimensional dependency modeling to extract robust spatio-temporal representations from corrupted IoT sensor inputs.

### Key Features

- ✅ Adaptive temporal segmentation for multi-scale pattern capture
- ✅ Robust to sensor failures, transmission errors, and missing values
- ✅ Self-supervised denoising integrated into the architecture
- ✅ State-of-the-art performance on multiple benchmark datasets
- ✅ Efficient for edge computing deployment

### Performance Highlights

- **12.3% reduction** in MAE compared to state-of-the-art baselines
- **15.7% reduction** in RMSE across benchmark datasets
- Tested on PEMS03, PEMS04, PEMS07, PEMS08 datasets
- Maintains accuracy under various noise conditions

---

**Note**: This is a placeholder repository. Complete implementation will be available upon paper acceptance. Thank you for your understanding and interest in our work!