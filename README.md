# Playing Card Image Classifier (ML)

This project implements an image classification model to recognize playing cards
using Convolutional Neural Networks and transfer learning.

## Overview
- Task: Image classification
- Classes: 13 (Spades suit)
- Model: MobileNetV2 (pretrained on ImageNet)
- Framework: TensorFlow / Keras

## Repository Structure
```
playing-card-classifier-ml/
├── dataset/
│ ├── train/
│ ├── validation/
│ └── test/
├── playing_card_classifier.ipynb
├── card_classifier_spades.h5
├── requirements.txt
└── README.md 
```

## Methodology
- Directory-based dataset labeling
- Data augmentation to handle limited data
- Transfer learning with frozen base layers
- Softmax classification head

## Results
- High accuracy achieved on a controlled test set
- Performance degradation observed when scaling to multiple suits,
  highlighting the importance of sufficient data per class

## Scope Limitation
This project focuses on a single suit as a proof of concept. The same pipeline
can be extended to all 52 cards with additional data.

## Future Work
- Expand dataset with multiple images per card
- Extend classification to all suits
- Apply similar techniques to scientific datasets
