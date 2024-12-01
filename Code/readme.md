# Code Folder

## Overview

This folder contains three Jupyter notebooks that serve as the core code for detecting AI-generated fake restaurant reviews. The notebooks explore different machine learning techniques, ranging from text-based models to deep learning models using images, as well as multimodal models combining both text and image features.

Each notebook is designed to train and evaluate a specific type of model:

1. **`text_model.ipynb`**: A text-based model for detecting fake reviews using Natural Language Processing (NLP) techniques.
2. **`visual_model.ipynb`**: An image-based model that uses a pre-trained ResNet50 model to analyze images of restaurant dishes for fake review detection.
3. **`multimodal_model.ipynb`**: A multimodal model that combines both textual and visual features for improved fake review detection.

These notebooks are meant to be run sequentially to explore the full scope of the fake review detection task, starting with text-based features, moving to image-based features, and finally combining both.

## Notebook Descriptions

### 1. **`text_model.ipynb`**
This notebook focuses on the text-based approach for detecting AI-generated reviews. The model uses the following techniques:
- TF-IDF vectorization for text representation.
- A Decision Tree classifier to detect fake reviews based on textual features.
- Evaluation using accuracy and classification reports on validation and test datasets.

### 2. **`visual_model.ipynb`**
In this notebook, the focus is on detecting fake reviews based on images. The following steps are involved:
- Preprocessing images using TensorFlow and ResNet50, a pre-trained Convolutional Neural Network (CNN).
- Training the model to distinguish between authentic and fake reviews based on dish images.
- Evaluation with accuracy and classification reports.

### 3. **`multimodal_model.ipynb`**
This notebook combines text and image features to improve detection accuracy:
- Combines the features extracted from both the text (using TF-IDF) and images (using ResNet50) for classification.
- Uses a deep learning approach with TensorFlow to fine-tune a multimodal model.
- Includes techniques like data augmentation and early stopping to improve generalization.
- Evaluation of the multimodal model's performance.

## Results and Evaluation

Each notebook includes detailed evaluation metrics such as:
- **Accuracy**: Performance on the validation and test sets.
- **Classification Report**: Precision, recall, and F1-score for each class (authentic vs machine-generated).
- **Training/Validation Curves**: Plots showing model performance during training.

## Additional Notes

- Ensure that the dataset files (`train_filtered.csv`, `test_filtered.csv`, `val_filtered.csv`) and images are properly set up in the appropriate directories.
- You can modify the notebooks to experiment with different models or hyperparameters.
- The notebooks are designed to be run in a Jupyter Notebook or Google Colab environment.

This code folder is meant to facilitate easy experimentation and evaluation of different machine learning models for detecting fake reviews.
