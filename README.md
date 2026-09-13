# AI Skin Cancer Classification

Bachelor thesis project investigating the use of deep learning for skin lesion classification using the HAM10000 dataset.

The project compares two convolutional neural network architectures:

- ResNet50
- EfficientNetB0

The main focus of the research was to understand how model architecture and class imbalance affect skin lesion classification, particularly melanoma detection.

## Project Overview

The original HAM10000 dataset contains seven skin lesion classes. During the experiments, severe class imbalance caused unstable performance for highly underrepresented classes.

The final comparison therefore focused on five classes:

- Actinic keratoses (`akiec`)
- Basal cell carcinoma (`bcc`)
- Benign keratosis-like lesions (`bkl`)
- Melanoma (`mel`)
- Melanocytic nevi (`nv`)

Both ResNet50 and EfficientNetB0 were trained using transfer learning and evaluated using different class-weight configurations.

## Evaluation

Because the dataset is highly imbalanced, the models were evaluated using more than overall accuracy.

Metrics included:

- Accuracy
- Balanced accuracy
- Macro F1-score
- Weighted F1-score
- Class-wise recall
- Melanoma sensitivity
- Melanoma specificity
- Confusion matrices

## Best Model

The strongest configuration was EfficientNetB0 with a capped class weight of 3.0.

Results:

- Test accuracy: 64.9%
- Balanced accuracy: 51.8%
- Macro F1-score: 48.3%
- Weighted F1-score: 68.3%
- Melanoma recall: 59.6%
- Melanoma specificity: 80.0%

## Technologies

- Python
- Deep Learning
- Convolutional Neural Networks
- Transfer Learning
- ResNet50
- EfficientNetB0
- Image Classification
- Machine Learning Evaluation

## Bachelor Thesis

**Using Artificial Intelligence for Skin Cancer Diagnosis: Accuracy, Challenges, and Opportunities**

Lucerne University of Applied Sciences and Arts  
Bachelor of Science in International IT Management  
2026

## Disclaimer

This project was developed for academic and educational purposes.

The models are experimental and are not intended for clinical diagnosis or use as a medical device.
