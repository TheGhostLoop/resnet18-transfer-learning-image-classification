## Experiments

### 1. Cats vs Dogs (Binary Classification)
- Feature extraction + fine-tuning
- Achieved ~100% validation accuracy
- Very fast convergence due to ImageNet features

### 2. Flowers Dataset (14-Class Classification)
- Fine-tuned last ResNet block
- Best validation accuracy ~98%
- Early stopping due to overfitting risk

## Overview
Applied transfer learning using a pretrained ResNet18 model for binary image classification.

## Approach
- Used ImageNet-pretrained ResNet18
- Feature extraction (frozen backbone)
- Fine-tuned last residual block (layer4) with lower learning rate
- Monitored training vs validation accuracy to avoid overfitting

## Results
- Feature extraction accuracy: ~98%
- Fine-tuned accuracy: 100% (on validation set)

## Training Curves
[accuracy_plot.png]

## Key Learnings
- Importance of freezing/unfreezing layers
- Effect of learning rate during fine-tuning
- Early stopping based on validation metrics
