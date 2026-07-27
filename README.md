<p align="center">
  <img src="man.png" alt="Alzheimer's Disease" width="600">
</p>

# EEG-Based Alzheimer's Disease Classification

## Group Information

Group 02
  
Md. Al Ehtesum korim(ID: 2025-2-96-016)

Sadika Parvin Mumu(ID: 2026-2-74-010)

Department of Computer Science and Engineering

---
##Project Track
- **Track:** Graph Neural Network (GNN) + Attention
- **Objective:** Classify Alzheimer's Disease (AD) and Healthy Control (HC) EEG recordings.

---

## Project Description

This project analyzes resting-state, eyes-closed EEG signals to distinguish Alzheimer's Disease (AD) patients from Healthy Control (HC) participants.

The workflow includes:

- Exploratory Data Analysis (EDA)
- Spectral Analysis
- EEG Feature Extraction
- Statistical Analysis
- Functional Connectivity Analysis
- Graph Neural Network (GNN) with Attention Mechanism for Classification

---

# Datasets

## Dataset 1

**Description**

- **Classes:** Alzheimer's Disease (AD) and Healthy Control (HC)
- **Condition:** Eyes Closed
- **File Format:** `.txt`

### Folder Structure

```text
EEG_data/
├── AD/
│   └── Eyes_closed/
│       └── Subject/
│           ├── Channel_1.txt
│           ├── Channel_2.txt
│           └── ...
└── Healthy/
    └── Eyes_closed/
        └── Subject/
            ├── Channel_1.txt
            ├── Channel_2.txt
            └── ...
```

---

## Dataset 2

**Description**

- **Classes:** Healthy Control (SETB) and Alzheimer's Disease (SETD)
- **Condition:** Eyes Closed
- **Sampling Frequency:** 128 Hz
- **Recording Duration:** Approximately 8 seconds
- **Channels:** 19 EEG channels (International 10–20 System)
- **File Format:** `.out`

> **Note:** Eyes-open recordings are excluded because the same participants were recorded under both eyes-open and eyes-closed conditions.

### Folder Structure

```text
DataBase/
├── SETB/
│   ├── ec0101.out
│   └── ...
└── SETD/
    ├── ec0303.out
    └── ...
```

---

## EEG Channels

- Fp1
- Fp2
- F7
- F3
- Fz
- F4
- F8
- T3
- C3
- Cz
- C4
- T4
- T5
- P3
- Pz
- P4
- T6
- O1
- O2

---

# Analysis Pipeline

The project includes the following analyses:

- Dataset statistics
- Missing-value analysis
- EEG amplitude distribution analysis
- Power Spectral Density (PSD)
- Fast Fourier Transform (FFT)
- Relative Delta, Theta, Alpha, Beta, and Gamma band power
- Theta/Alpha ratio
- Delta/Alpha ratio
- Alpha peak frequency
- Spectral entropy
- Hjorth Activity
- Hjorth Mobility
- Hjorth Complexity
- EEG channel correlation analysis
- t-SNE visualization
- Welch's t-test
- Hedges' g effect size
- False Discovery Rate (FDR) correction

---

# GNN + Attention Framework

The EEG signals are modeled as a graph.

| Component | Description |
|-----------|-------------|
| **Nodes** | EEG Channels |
| **Node Features** | Spectral, statistical, and complexity features |
| **Edges** | Functional connectivity between EEG channels |
| **Attention Mechanism** | Learns the most informative EEG channels and channel connections |

---

# Repository Structure

```text
.
├── Code/
│   ├── EDA.ipynb
│   ├── Feature_Extraction.ipynb
│   ├── GNN_Model.ipynb
│   └── ...
├── Papers/
├── Report/
└── README.md
```

