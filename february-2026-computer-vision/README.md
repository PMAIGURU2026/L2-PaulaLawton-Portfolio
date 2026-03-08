# February 2026 — Computer Vision

**Month:** February 2026  
**Program:** Pursuit AI Fellowship — Level 2  
**Author:** Paula Lawton

---

## Description

This project explores computer vision, covering image classification, object detection, and transfer learning. Using PyTorch and pre-trained convolutional neural networks (CNNs) from `torchvision`, models were fine-tuned on custom image datasets to solve real-world visual recognition problems.

## Topics Covered

- Image data preprocessing: resizing, normalization, data augmentation (`torchvision.transforms`)
- Convolutional Neural Networks (CNNs): architecture intuition (convolution, pooling, fully connected layers)
- Transfer learning: fine-tuning ResNet-18 and MobileNetV2 on custom datasets
- Model evaluation: top-1 accuracy, confusion matrices, Grad-CAM visualizations
- Introduction to object detection with YOLO (inference only)

## Project Highlights

- **Recycling Classifier:** Fine-tuned ResNet-18 to classify images into 6 recycling categories (cardboard, glass, metal, paper, plastic, trash). Achieved 91% top-1 accuracy on the held-out test set using a dataset of ~2,500 images.
- **Grad-CAM Visualizations:** Generated Grad-CAM heatmaps to visualize which image regions the model focused on, confirming the model learned meaningful visual features rather than spurious correlations.
- **Data Augmentation Study:** Compared model performance with and without augmentation (random horizontal flips, color jitter, random crops), demonstrating a ~7% accuracy improvement with augmentation on the training set.

## Skills Demonstrated

- Applying transfer learning to a new domain with limited data
- Building PyTorch `Dataset` and `DataLoader` classes for custom image data
- Model interpretability using Grad-CAM
- Training loop implementation with learning rate scheduling

## How to Run

```bash
pip install torch torchvision matplotlib pillow jupyter

jupyter notebook
```

> A GPU (CUDA) is recommended for training but not required — training on CPU will work for small datasets.

## Key Takeaways

Transfer learning makes computer vision accessible even without massive datasets or compute resources. Model interpretability (Grad-CAM) is essential for building trust in CV models, especially in real-world applications where false positives have consequences.
