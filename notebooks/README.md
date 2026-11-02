# Jupyter Notebook

This directory contains the Jupyter Notebook used for the **Musical Instrument Recognition Using DSP and Machine Learning** project.

## Notebook

`Musical_Instrument_Recognition.ipynb`

## Overview

The notebook implements the audio preprocessing, feature extraction, CNN-based classification, model evaluation, and prediction pipeline for musical instrument recognition using the IRMAS dataset.

## Workflow

The notebook covers the following stages:

### 1. Audio Preprocessing

- Loading audio recordings using Librosa.
- Converting audio to mono.
- Resampling audio to 22,050 Hz.
- Segmenting audio into 3-second windows.
- Extracting Mel-spectrogram features.

### 2. Single-Instrument Classification

- Preparing the processed dataset.
- Training a deep CNN model.
- Evaluating the model on the test data.
- Predicting the predominant instrument in an audio recording.

### 3. Multilabel Instrument Classification

- Preparing multilabel training data.
- Generating synthetic mixtures of musical instruments.
- Training CNN models for multilabel recognition.
- Evaluating model performance using precision, recall, and F1-score.
- Optimizing prediction thresholds.

### 4. Prediction on Audio Recordings

The notebook includes prediction implementations for audio recordings, including longer audio files using overlapping segments.

The models can identify the presence of multiple instruments in a recording and provide prediction confidence scores.

## Input Data

The notebook uses:

- Original IRMAS audio recordings.
- Processed NumPy feature and label arrays.
- Trained CNN models.

Refer to the [`data/README.md`](../data/README.md) for dataset download links and instructions.

## Trained Models

The trained models are available in the [`models/`](../models/) directory.

- `best_cnn_deep.keras`
- `best_cnn_multilabel_v2.keras`

## Requirements

The notebook uses Python and the following libraries:

- NumPy
- Pandas
- Librosa
- Matplotlib
- Scikit-learn
- TensorFlow / Keras

Install the required libraries using:

```bash
pip install -r ../requirements.txt
```

## Execution

1. Download the required original and processed datasets.
2. Download or use the trained models provided in the repository.
3. Update the dataset and model paths in the notebook according to your local directory.
4. Install the required Python libraries.
5. Open the notebook using Jupyter Notebook or JupyterLab.
6. Execute the cells in the appropriate order.

**Note:** The notebook contains local file paths from the development environment. These paths must be updated before running the notebook on another system.

