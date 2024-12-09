# DBANet
This project provides the code for 'Dual-Branch Attention Network for ORSI Salient Object Detection via Enhanced Feature Learning'

# Introduction

<div align="center">
    <img width="400" alt="image" src="images/Challenges.png?raw=true">
</div>


The top row shows typical ORSIs; the middle row displays the ground truth; and the bottom row presents the salient prediction map of the NSI-SOD method DPORT.


## Network Architecture
The overall architecture of DBANet, which mainly consists of Feature Enhancement Attention (FEA) module and an improved decoder. (a) Diagonal Enhanced Attention (DEA), (b) Multi-Scale Spatial Attention (MSA), and (c) Channel-Enhanced Attention Fusion (CEA).

<div align="center">
<img width="800" alt="image" src="images/DBANet.png?raw=true">
</div>

## Requirements

python 3.8 + pytorch 1.9.0

## Prepare Datasets

- Download datasets: ORSSD from this [link](https://challenge.isic-archive.com/data/#2017), EORSSD from this [link](https://challenge.isic-archive.com/data/#2018), and ORS-4199 from this [link](https://www.dropbox.com/scl/fi/epzcoqeyr1v9qlv/PH2Dataset.rar?rlkey=6mt2jlvwfkditkyg12xdei6ux&e=1).

## Train the DBANet

- Download [pvt_v2_b2.pth](https://pan.baidu.com/s/1U6Bsyhu0ynXckU6EnJM35w) (code: sxiq), and put it in './model/'. 
- Modify paths of datasets, then run train_DBANet.py.
- Note: Our main model is under './model/DBANet_models.py'

### 3. Test the DBANet
- Run test_DBANet.py.


## 🖼️ Visualization

<div align="center">
<img width="800" alt="image" src="images/Visualization.png?raw=true">
</div>



## 🎫 License

The content of this project itself is licensed under [LICENSE](LICENSE).

## 💡 Acknowledgement

- [UltraLight VM-UNet](https://github.com/eltociear/UltraLight-VM-UNet)
- [SHViT](https://github.com/ysj9909/SHViT)

