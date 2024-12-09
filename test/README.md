<div align="center">
<h1>Dual-Branch Attention Network for ORSI Salient Object Detection 
    via Enhanced Feature Learning </h1>
</div>


## 🎈 News

- [2024.11.10] Training and inference code released

## 🚀 Introduction

<div align="center">
    <img width="400" alt="image" src="asserts/Challenges.png?raw=true">
</div>


The top row shows typical ORSIs; the middle row displays the ground truth; and the bottom row presents the salient prediction map of the NSI-SOD method DPORT.


## 📻 Overview

<div align="center">
<img width="800" alt="image" src="asserts/DBANet.png?raw=true">
</div>


The overall architecture of DBANet, which mainly consists of Feature Enhancement Attention (FEA) module and an improved decoder. (a) Diagonal Enhanced Attention (DEA), (b) Multi-Scale Spatial Attention (MSA), and (c) Channel-Enhanced Attention Fusion (CEA).

## 📆 TODO

- [x] Release code

## 🎮 Getting Started

### 1. Install Environment

```
conda create -n DBANet python=3.8
conda activate DBANet
pip install torch==1.13.0 torchvision==0.14.0 torchaudio==0.13.0 --extra-index-url https://download.pytorch.org/whl/cu117
pip install packaging
pip install timm==0.4.12
pip install pytest chardet yacs termcolor
pip install submitit tensorboardX
pip install triton==2.0.0
pip install causal_conv1d==1.0.0  # causal_conv1d-1.0.0+cu118torch1.13cxx11abiFALSE-cp38-cp38-linux_x86_64.whl
pip install mamba_ssm==1.0.1  # mmamba_ssm-1.0.1+cu118torch1.13cxx11abiFALSE-cp38-cp38-linux_x86_64.whl
pip install scikit-learn matplotlib thop h5py SimpleITK scikit-image medpy yacs
```

### 2. Prepare Datasets

- Download datasets: ORSSD from this [link](https://challenge.isic-archive.com/data/#2017), EORSSD from this [link](https://challenge.isic-archive.com/data/#2018), and ORS-4199 from this [link](https://www.dropbox.com/scl/fi/epzcoqeyr1v9qlv/PH2Dataset.rar?rlkey=6mt2jlvwfkditkyg12xdei6ux&e=1).
- Folder organization: put ORSSD datasets into ./dataset/ORSSD folder, EORSSD datasets into ./dataset/EORSSD folder, and PH2 datasets into ./data/PH2 folder, Kvasir datasets into ./data/Kvasir folder, and BUSI datasets into ./data/BUSI folder.

### 3. Train the DBANet

- Download [pvt_v2_b2.pth](https://pan.baidu.com/s/1U6Bsyhu0ynXckU6EnJM35w) (code: sxiq), and put it in './model/'. 
- Modify paths of datasets, then run train_GeleNet.py.
- Note: Our main model is under './model/GeleNet_models.py' (PVT-v2-b2 backbone)

### 3. Test the DBANet
- Run test_GeleNet.py.


## 🖼️ Visualization

<div align="center">
<img width="800" alt="image" src="asserts/Visualization.png?raw=true">
</div>



## 🎫 License

The content of this project itself is licensed under [LICENSE](LICENSE).

## 💡 Acknowledgement

- [UltraLight VM-UNet](https://github.com/eltociear/UltraLight-VM-UNet)
- [SHViT](https://github.com/ysj9909/SHViT)

