# b2ai-voice-biomarker
This repository contains the implementation focusing on the automatic improvement of data collection tasks, with a particular emphasis on voice data quality and task compliance.

## Project Overview

The project aims to enhance the data collection process by automating the assessment of voice data quality and task compliance. The project involves custom annotation of voice data, training machine learning models, and employing advanced techniques to improve prediction accuracy.

## Tasks and Implementation

### Data Annotation

- **Objective:** Annotate a subset of the audio data for quality and adherence using a custom Likert scale (1 to 5).
- **Implementation:**
  - Annotated 13% of the audio data (800 out of 6000+ files) for quality and adherence.
  - Developed a custom Likert scale for annotation.

### Model Training

- **Objective:** Train machine learning models to predict quality labels and adherence.
- **Implementation:**
  - Developed and trained a CNN model using MFCC features to predict quality labels, achieving an accuracy of 80.85%.
  - Generated Mel-frequency spectrograms and utilized pre-trained models (ResNet50 and EfficientNet B0) to predict adherence.
  - Applied cross-validation and data augmentation techniques, enhancing model accuracy from 75.23% and 65.06% to 91.50%.

### Preprocessing

- **Objective:** Apply advanced preprocessing techniques to prepare the data for modeling.
- **Implementation:**
  - Utilized noise reduction, normalization, and conversion to spectrograms for audio data preprocessing.

## Technologies Used

- Python
- Jupyter Notebook
- Librosa
- PyTorch
- Scikit-learn
- Pre-trained models (ResNet50, EfficientNet B0)
