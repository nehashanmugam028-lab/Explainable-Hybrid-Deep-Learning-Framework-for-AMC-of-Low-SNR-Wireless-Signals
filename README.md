# Explainable Hybrid Deep Learning Framework for Automatic Modulation Classification of Low-SNR Wireless Signals

##  Project Overview

Wireless communication systems rely on modulation techniques to transmit information through radio signals. Identifying the modulation scheme of a received signal is an important task in modern wireless communication systems.

However, under low Signal-to-Noise Ratio (SNR) conditions, noise can significantly distort signal characteristics, making accurate modulation classification challenging.

This project proposes an **Explainable Hybrid Deep Learning Framework** that combines Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks to perform Automatic Modulation Classification (AMC) using In-phase (I) and Quadrature (Q) signal data.

The framework integrates **Explainable AI (XAI) using SHAP (SHapley Additive exPlanations)** to identify and interpret the signal features influencing the model's classification decisions.

##  Objectives

- Develop a hybrid CNN-LSTM architecture for automatic modulation classification.
- Process and normalize I/Q wireless signal samples.
- Classify different modulation schemes under varying noise conditions.
- Evaluate classification performance across different SNR levels.
- Improve the interpretability of deep learning predictions using SHAP.
- Analyze the features contributing to correct and incorrect classifications.

##  Proposed Methodology

The proposed framework consists of the following stages:

1. **Dataset Collection:** Synthetic wireless I/Q signal samples representing different modulation schemes and SNR levels.
2. **Signal Preprocessing:** Missing-value handling, reshaping, normalization, and label encoding.
3. **Dataset Splitting:** Dividing the dataset into training, validation, and testing sets using a 70:15:15 ratio.
4. **CNN Feature Extraction:** Extracting local patterns and relevant characteristics from I/Q signal samples.
5. **LSTM Sequential Learning:** Learning temporal dependencies and sequential patterns in the signal.
6. **Feature Fusion:** Combining the complementary features learned by the CNN and LSTM components.
7. **Modulation Classification:** Predicting the modulation scheme using the fused feature representation.
8. **Explainable AI:** Applying SHAP to understand the contribution of input features to classification predictions.
9. **Performance Evaluation:** Evaluating the framework using accuracy, precision, recall, F1-score, confusion matrices, and SNR-based analysis.

## Model Architecture

The framework uses a hybrid CNN-LSTM architecture:

- **CNN:** Extracts local signal patterns from I/Q data.
- **LSTM:** Captures temporal relationships within signal sequences.
- **Feature Fusion:** Combines CNN and LSTM representations.
- **Classification Layer:** Predicts the modulation class.
- **SHAP:** Provides feature attribution and interpretable explanations.

##  Explainable AI

SHAP is integrated to improve the transparency of the classification model.

It helps to:
- Identify influential I/Q signal features.
- Understand the factors contributing to individual predictions.
- Visualize feature contributions.
- Analyze model behavior under low-SNR conditions.
- Investigate incorrect classification decisions.

## Technologies Used

- Python
- Deep Learning
- Convolutional Neural Networks (CNN)
- Long Short-Term Memory (LSTM)
- Explainable AI (XAI)
- SHAP
- I/Q Signal Processing
- Data Visualization

##  Performance Evaluation

The framework is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Performance comparison across different SNR levels

## Future Scope

- Extend the framework to real-world wireless signals using Software-Defined Radio (SDR).
- Improve classification robustness under extremely low-SNR conditions.
- Support additional analog and digital modulation schemes.
- Explore lightweight architectures for real-time classification.
- Investigate open-set recognition for previously unseen modulation classes.
- Improve explainability for classification errors and signal characteristics.

## Conclusion

This project combines hybrid deep learning and Explainable AI to develop an interpretable approach for automatic modulation classification under noisy wireless communication conditions. By integrating CNN-LSTM feature learning with SHAP-based explanations, the framework aims to support more reliable and transparent wireless signal analysis.
