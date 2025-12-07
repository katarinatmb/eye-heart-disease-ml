# Cardiovascular Disease Prediction from Retinal Fundus Images

## 🔗 Related Projects

This project is part of a multi-modal cardiovascular disease detection research series:

- **👁️ Eye-Based Detection** (This Repository) - Retinal fundus image analysis using CNN and logistic regression
- **👅 [Tongue-Based Detection](https://github.com/katarinatmb/Tongue-Based-Detection)** - Tongue image classification using deep learning CNNs (AUC: 0.605)

## Overview

This project investigates whether subtle patterns in retinal fundus images can help predict heart disease. Inspired by emerging research connecting microvascular eye features with cardiovascular risk, the goal was to build machine learning models capable of identifying heart disease indicators directly from retinal photographs. To explore this connection, I developed two core models: a Convolutional Neural Network (CNN) that learns visual patterns from images, and a logistic regression model that acts as a baseline for comparison. Together, these models create a cohesive framework for understanding how predictive the eye really is when it comes to cardiovascular health.

## Methodology

The workflow for this project began with importing and structuring a dataset of retinal images labeled according to the presence or absence of heart disease. The images were not standardized: lighting varied across photos, and some subjects were wearing glasses or had their eyes closed. These inconsistent or unusable images were manually removed to ensure dataset quality. The remaining images were resized, normalized, and transformed to prepare them for model training. A CNN was built using TensorFlow/Keras, with layers designed to extract meaningful spatial features and reduce overfitting through dropout regularization. After training the model and evaluating its predictions, a confusion matrix and classification report were generated to examine accuracy, precision, recall, and overall model behavior. Although the dataset was relatively small, the CNN still demonstrated promise in detecting patterns associated with heart disease.

To complement the CNN, I constructed a second approach using logistic regression. The images were flattened using grayscale histogram features, creating a structured numerical representation that allowed logistic regression to learn broader statistical relationships rather than visual ones. This helped benchmark how much value the CNN's image-based feature extraction was adding beyond a simpler model. Comparing these results gave insight into model limitations, dataset needs, and future potential.

## Results & Impact

This work highlights the potential for retinal imaging to assist in early cardiovascular screening. With more data, optimized architectures, and hyperparameter tuning, future iterations could better capture subtle retinal signs linked to heart disease. The project also demonstrates how deep learning and traditional statistical models can complement each other when exploring complex biomedical relationships.

**Key Findings:**
- CNN achieved AUC of 0.732 for cardiovascular disease detection
- Manual quality control was essential for handling non-standardized medical images
- Comparison with tongue-based approach (AUC 0.605) suggests eye images contain stronger cardiovascular signals

## Technologies Used

- **Deep Learning:** TensorFlow, Keras
- **Machine Learning:** scikit-learn, Logistic Regression
- **Data Processing:** NumPy, pandas, OpenCV
- **Visualization:** Matplotlib, seaborn


