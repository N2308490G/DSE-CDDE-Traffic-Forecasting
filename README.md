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

## 📁 Project Structure

```
DSE-CDDE-Traffic-Forecasting/
├── README.md                    # This file
├── LICENSE                      # License information
├── requirements.txt            # Python dependencies
├── setup.py                    # Installation script
├── config/                     # Configuration files
│   ├── model_config.yaml      # Model hyperparameters
│   └── dataset_config.yaml    # Dataset configurations
├── data/                       # Data directory
│   ├── README.md              # Data preparation guide
│   ├── raw/                   # Raw datasets (to be added)
│   └── processed/             # Preprocessed data (to be added)
├── models/                     # Model implementations
│   ├── __init__.py
│   ├── dse.py                 # Dynamic Segment Extractor
│   ├── cdde.py                # Cross-Dimensional Dependency Encoder
│   ├── dse_cdde.py            # Complete DSE-CDDE model
│   └── baseline/              # Baseline model implementations
├── utils/                      # Utility functions
│   ├── __init__.py
│   ├── data_loader.py         # Data loading utilities
│   ├── metrics.py             # Evaluation metrics
│   └── visualization.py       # Visualization tools
├── experiments/                # Experiment scripts
│   ├── train.py               # Training script
│   ├── evaluate.py            # Evaluation script
│   └── run_experiments.sh     # Batch experiment runner
├── notebooks/                  # Jupyter notebooks
│   └── demo.ipynb             # Demonstration notebook
└── docs/                       # Additional documentation
    ├── architecture.md        # Model architecture details
    └── usage.md               # Usage instructions
```

---

## 🚀 Quick Start (Available After Publication)

### Installation

```bash
# Clone the repository
git clone https://github.com/N2308490G/DSE-CDDE-Traffic-Forecasting.git
cd DSE-CDDE-Traffic-Forecasting

# Install dependencies
pip install -r requirements.txt

# Or install as a package
pip install -e .
```

### Data Preparation

```bash
# Download datasets (scripts will be provided upon publication)
python scripts/download_data.py --dataset PEMS04

# Preprocess data
python scripts/preprocess.py --dataset PEMS04
```

### Training

```bash
# Train DSE-CDDE model
python experiments/train.py --config config/model_config.yaml --dataset PEMS04
```

### Evaluation

```bash
# Evaluate trained model
python experiments/evaluate.py --checkpoint checkpoints/best_model.pth --dataset PEMS04
```

---

## 📊 Datasets

Our experiments are conducted on the following public benchmark datasets:

- **PEMS03**: 358 sensors, 26,208 time steps
- **PEMS04**: 307 sensors, 16,992 time steps  
- **PEMS07**: 883 sensors, 28,224 time steps
- **PEMS08**: 170 sensors, 17,856 time steps

Dataset download links and preprocessing scripts will be provided upon paper acceptance.

---

## 🔬 Methodology

### Dynamic Segment Extractor (DSE)

The DSE module automatically learns optimal temporal boundaries for capturing multi-scale traffic patterns, moving beyond fixed-size time windows. Key components include:

- Learnable segmentation boundaries
- Multi-scale temporal convolutions
- Adaptive pooling mechanisms

### Cross-Dimensional Dependency Encoder (CDDE)

The CDDE integrates self-supervised denoising with cross-dimensional dependency modeling:

- Self-supervised denoising objectives
- Cross-dimensional attention mechanisms
- Robust spatio-temporal representation learning

---

## 📝 Citation

If you find our work useful, please consider citing our paper (citation information will be updated upon publication):

```bibtex
@article{yang2025dsecdde,
  title={DSE-CDDE: Dynamic Segment Extractor with Cross-Dimensional Dependency Encoder for Traffic Flow Forecasting},
  author={Yang, Wenbiao and Shang, Wenli and Wang, Lianhai and Liu, Zhiquan},
  journal={IEEE Transactions on Transportation Electrification},
  year={2025},
  note={Under Review}
}
```

---

## 👥 Authors

- **Wenbiao Yang** - Guangzhou University (yangwb@gzhu.edu.cn)
- **Wenli Shang** - Guangzhou University (shangwl@gzhu.edu.cn)
- **Lianhai Wang** - Shandong Computer Science Center, Qilu University of Technology
- **Zhiquan Liu** - Jinan University

---

## 📄 License

This project will be released under the MIT License upon paper acceptance. See [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

We welcome contributions! However, please note that active development and pull requests will be enabled after the paper is accepted and the complete code is released.

---

## 📮 Contact

For questions about the paper or implementation, please contact:
- Wenbiao Yang: yangwb@gzhu.edu.cn

---

## 🔔 Updates

- **2025-11-14**: Repository created with project structure
- **TBD**: Complete code release pending paper acceptance

---

## ⭐ Acknowledgments

This work was supported by:
- National Natural Science Foundation of China (Grant No. 62173101)
- Open Research Project of Key Laboratory of Computing Power Network and Information Security, Ministry of Education (Grant No. 2024ZD018)

---

**Note**: This is a placeholder repository. Complete implementation will be available upon paper acceptance. Thank you for your understanding and interest in our work!