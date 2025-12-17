# Mini Case Study: CNN Feature Fusion for Image Classification

## Overview
This repository presents a mini case study on **image classification using feature-level fusion**. The project demonstrates how combining early and late features from a pretrained convolutional neural network can improve classification performance while keeping the model lightweight and efficient.

## Task
- **Computer Vision Task**: Image Classification  
- **Approach**: Feature fusion using a pretrained MobileNetV2 backbone

## Dataset
- Public, non-Kaggle image dataset  
- Images resized to 128×128 and normalized  
- Simple data augmentation applied  

## Methodology
- **Backbone**: Pretrained MobileNetV2  
- **Fusion Strategy**:
  - Extract features from early and late layers
  - Apply global pooling
  - Concatenate features before classification
- **Training**:
  - Cross-Entropy Loss
  - Adam optimizer
  - 2 training epochs (lightweight setup)

## Results

| Epoch | Loss  | Accuracy |
|------:|------:|---------:|
| 1 | 1.1648 | 62.78% |
| 2 | 0.6978 | 77.58% |

Training curves and sample predictions are shown in the notebook.

## Conclusion
Feature-level fusion of early and late CNN representations improves classification accuracy while maintaining fast training and low computational cost. The results show effective convergence even with minimal training.

