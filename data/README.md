# Data Directory

This directory will contain traffic flow datasets and preprocessing scripts.

## Structure

```
data/
├── README.md              # This file
├── raw/                   # Raw datasets (PEMS03, PEMS04, PEMS07, PEMS08)
├── processed/             # Preprocessed data
└── scripts/               # Data preprocessing scripts
```

## Datasets

Our experiments use the following public benchmark datasets:

### PEMS03
- **Sensors**: 358
- **Time Steps**: 26,208
- **Time Range**: September to November 2018
- **Sampling Interval**: 5 minutes

### PEMS04
- **Sensors**: 307
- **Time Steps**: 16,992
- **Time Range**: January to February 2018
- **Sampling Interval**: 5 minutes

### PEMS07
- **Sensors**: 883
- **Time Steps**: 28,224
- **Time Range**: May to August 2017
- **Sampling Interval**: 5 minutes

### PEMS08
- **Sensors**: 170
- **Time Steps**: 17,856
- **Time Range**: July to August 2016
- **Sampling Interval**: 5 minutes

## Data Format

Each dataset includes:
- Traffic flow measurements (numpy arrays)
- Adjacency matrices for road network topology
- Sensor location metadata

## Data Preprocessing

Preprocessing steps include:
1. Missing value imputation
2. Data normalization (z-score)
3. Train/validation/test split (70%/10%/20%)
4. Sequence generation for temporal modeling

## Download Instructions

Dataset download links and preprocessing scripts will be provided upon paper acceptance.

### Data Sources

PEMS datasets are publicly available from:
- California Transportation Agencies (Caltrans) Performance Measurement System (PeMS)
- http://pems.dot.ca.gov/

---

**Note**: Complete datasets and preprocessing scripts will be provided upon paper acceptance.
