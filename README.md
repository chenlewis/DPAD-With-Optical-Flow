# DPAD-With-Optical-Flow

## Overview

This is the implementation of the method proposed in "A Document Presentation Attack Detection Scheme with Optical Flow under a Flashlight" with pytorch(1.12.1, gpu version). The associated datasets are available upon request.

## Introduction

In this work, we improve the generalization performance of the existing DPAD backbones by introducing a new data modality, the optical fow. First, through a comparative analysis of physical properties, the fundamental differences in light reflection characteristics between genuine and recaptured documents are revealed. Leveraging video temporal data and optical flow estimation algorithms, the significant 
distinctions in their dynamic optical flow features are characterized. Second, a dual-stream network architecture is designed, incorporating a cross-modal focal loss for dynamic weight allocation, which effectively fuses optical flow features with low-level features. Finally, we construct a student card video dataset under flashlight, containing over 18,000 frames of genuine documents and various types of recaptured data.
<div align="center">
  <img src="https://github.com/chenlewis/DPAD-With-Optical-Flow/blob/main/Figure/Physical%20Model.png" width="500" height="500"/>
</div>

## Environment Request

python == 3.9.12   
matplotlib == 3.7.1  
numpy == 1.22.3  
Pillow== 9.0.1  
scikit_learn == 1.2.2  
torch == 1.12.1  
torchnet == 0.0.4  
torchvision == 0.13.1  
tqdm == 4.65.0  

## Files Description

```F-AutheNet.py```  
Train\Valid\Test\Calculate AUC and EER metrics

## Citation

If you use our code please cite: Changsheng Chen, Wenyu Chen, Ximin Chen, and Haodong Li, A Document Presentation Attack Detection Scheme with Optical Flow under a Flashlight, in _Apsipa ASC_, 2024.
