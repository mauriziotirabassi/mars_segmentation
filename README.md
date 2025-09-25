# Mars Terrain Semantic Segmentation with U-Net

This project implements semantic segmentation of Mars surface images using U-Net architectures. It focuses on handling class imbalance, analyzing texture variability, and optimizing model performance through data augmentation, custom loss functions, and architectural improvements.

## Overview

- Dataset: 2,615 grayscale images (64×128) with 5 segmentation classes  
- Challenges: severe class imbalance, high texture variability  
- Solutions: outlier removal, tiling, oversampling, data augmentation, focal loss, and architectural tuning  

## Model

- U-Net with skip connections and dual-path design (standard + dilated convolutions)  
- SE attention in bottleneck and spatial dropout for regularization  
- Background class excluded from loss for better minority class learning

## Results

- Oversampling improved Mean IoU from 41.76% → 43.51%  
- Best augmentation (G + N): Mean IoU 44.55%, Score 45.70%  
- Final model: Mean IoU 60.51%, Score 69.06%

## Authors

- M. Alipoor  
- G. Annaloro  
- M. Tirabassi
