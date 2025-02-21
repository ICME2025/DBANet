<div align="center">
<h1>Dual-Branch Attention Network for Salient Object Detection in Optical Remote Sensing Images </h1>
</div>

## 📆 News
This project provides the code and results for DBANet.

## ⭐ Abstract
Salient object detection in optical remote sensing images (ORSI-SOD) presents significant challenges due to target diversity, scale variations, and spatial inconsistencies, often resulting in incomplete detections. To tackle these issues, we propose the Dual-Branch Attention Network (DBANet), which introduces a novel Feature Enhancement Attention (FEA) module and an improved decoder to enhance detection performance. The FEA module integrates Diagonal Enhanced Attention (DEA) for explicit feature enhancement and Multi-Scale Spatial Attention (MSA) for effectively capturing multi-scale context and preserving edge details, addressing the limitations in spatial consistency and generalization. Plus, the decoder’s feature fusion process employs channel shuffle and a large-kernel spatial attention mechanism to assign dynamic weights and preserve boundaries. Our approach improves feature learning and object localization, reducing spatial inconsistencies and incomplete detections. Extensive experiments on three benchmark datasets demonstrate that DBANet achieves state-of-the-art performance and robustness, highlighting its effectiveness in addressing key challenges in ORSI-SOD.

## 📻 Network Architecture
   <div align=center>
   <img src="https://github.com/Wyqmiao/RoCAFENet/blob/main/images/RoCAFENet.jpg">
   </div>
The overall architecture of DBANet, which mainly consists of Feature Enhancement Attention (FEA) module and an improved decoder. (a) Diagonal Enhanced Attention (DEA), (b) Multi-Scale Spatial Attention (MSA), and (c) Channel-Enhanced Attention Fusion (CEAF) module.
   
## 🎮 Requirements
   python 3.8 + pytorch 1.9.0
   
## 🎈 Training
   Download [pvt_v2_b2.pth] and put it in './model/'. 
   
   Modify paths of datasets, then run train.py.

Note: Our main model is under './model/DBANet.py'

## 🖼️ Quantitative comparison
   <div align=center>
   <img src="https://github.com/Wyqmiao/RoCAFENet/blob/main/images/table1.jpg">
   </div>
   
## 🎫 Visualization
   <div align=center>
   <img src="https://github.com/Wyqmiao/RoCAFENet/blob/main/images/Visualization comparison.jpg">
   </div>
