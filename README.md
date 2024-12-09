# DBANet
This project provides the code for 'Dual-Branch Attention Network for ORSI Salient Object Detection via Enhanced Feature Learning'

# Network Architecture
The overall architecture of DBANet, which mainly consists of Feature Enhancement Attention (FEA) module and an improved decoder. (a) Diagonal Enhanced Attention (DEA), (b) Multi-Scale Spatial Attention (MSA), and (c) Channel-Enhanced Attention Fusion (CEA).

<div align="center">
<img width="900" alt="image" src="images/DBANet.png?raw=true">
</div>

# Requirements

- python 3.8 + pytorch 1.9.0

# Train the DBANet
- We use data_aug.m for data augmentation.
- Modify paths of datasets, then run train_DBANet.py.
- Note: Our main model is under './model/DBANet_models.py'

# Test the DBANet
- Run test_DBANet.py.

# Quantitative comparison
Quantitative comparison with state-of-the-art methods on the ORSSD, EORSSD and ORS-4199 datasets.

<div align="center">
<img width="900" alt="image" src="images/table.png?raw=true">
</div>

# Visualization
Visualization comparing DBANet with eleven advanced methods on the ORS-4199 dataset.

<div align="center">
<img width="900" alt="image" src="images/Visualization.png?raw=true">
</div>


