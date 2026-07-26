# EEG-Based Alzheimer’s Disease Classification

**Group:** Group 02  
**Track:** Graph Neural Network (GNN) with Attention  
**Task:** Classify Alzheimer’s Disease (AD) and Healthy Control EEG recordings.

## Project Overview

This project investigates EEG-based identification of Alzheimer’s disease using statistical analysis, spectral features, functional connectivity, and a Graph Neural Network with an attention mechanism.

Each EEG channel is treated as a graph node. Connectivity measures between channels are used as graph edges, while EEG features such as relative band power, spectral entropy, Hjorth parameters, and theta/alpha ratios are used as node features.

## Datasets

### Dataset 1

- **Classes:** Healthy Control and Alzheimer’s Disease
- **Condition:** Eyes closed
- **File format:** `.txt`
- **Structure:** Each subject has separate EEG channel files.
- **Analysis unit:** Subject-level features aggregated across EEG channels.

```text
EEG_data/
├── AD/
│   └── Eyes_closed/
│       └── Subject/
│           ├── Fp1.txt
│           ├── Fp2.txt
│           └── ...
└── Healthy/
    └── Eyes_closed/
        └── Subject/
            ├── Fp1.txt
            ├── Fp2.txt
            └── ...
