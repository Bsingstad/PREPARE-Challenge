# PREPARE: Pioneering Research for Early Prediction of Alzheimer's and Related Dementias EUREKA Challenge

This repository contains solutions for the **PREPARE EUREKA Challenge**, aimed at advancing early prediction of Alzheimer's disease and related dementias (ADRD). The challenge is divided into two main subtasks, each focusing on a unique aspect of prediction and leveraging distinct datasets.

## Challenge Tracks

### 1. Social Determinants Track
This track involves developing algorithms and analytic approaches for early prediction of ADRD based on **social determinants of health**. The emphasis is placed on the **explainability** of predictions, ensuring that models provide interpretable results to support clinical decision-making.

- **Notebook**: `driven data alzheimer social tabnet.ipynb`
- **Model**: TabNet, a neural network architecture that inherently supports interpretability.
- **Features**: Social and demographic features, including health, lifestyle, and socioeconomic indicators.
- **Key Components**:
  - **Data Preprocessing**: Handling missing data and encoding categorical variables.
  - **Model Training**: Using TabNet to predict a composite score reflecting cognitive function across [seven different domains](https://www.drivendata.org/competitions/300/competition-nih-alzheimers-sdoh-2/page/930/#cognitive-domains).
  - **Explainability**: Generating feature importance to understand model decisions.
- **Outcome**: Explainable ADRD risk predictions driven by social determinants.

### 2. Acoustic Track
This track focuses on advancing algorithms for early prediction of ADRD based on **voice recordings**. The goal is to use audio data to uncover patterns associated with cognitive decline, with an emphasis on **model explainability**.

- **Notebook**: `melspectrogram_classification.ipynb`
- **Model**: Deep learning model trained on Mel-spectrogram representations of audio.
- **Features**: Acoustic features extracted from voice recordings, transformed into spectrograms for analysis.
- **Key Components**:
  - **Audio Processing**: Conversion of raw audio into Mel-spectrograms.
  - **Model Training**: CNN-based architecture for classification of ADRD risk.
  - **Explainability**: Techniques like Grad-CAM for interpreting spectrogram regions contributing to predictions.
- **Outcome**: Accurate and interpretable ADRD risk predictions from voice data.

## Repository Structure
```plaintext
.
├── driven-data-alzheimer-social-tabnet.ipynb  # Social Determinants Track solution
├── melspectrogram_classification.ipynb        # Acoustic Track solution
├── README.md                                  # Project documentation
