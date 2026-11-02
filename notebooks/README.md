# Jupyter Notebooks

This directory contains the Jupyter Notebooks used for the **Musical Instrument Recognition Using DSP and Machine Learning** project. The notebooks cover the complete experimental workflow as well as a demonstration of the trained models on audio recordings.

## Notebooks

### 1. Complete Project Workflow

`Musical_Instrument_Recognition.ipynb`

Implements the audio preprocessing, feature extraction, CNN-based classification, model evaluation, and prediction pipeline using the IRMAS dataset.

### 2. Final Project Demonstration

`Final_Project_Demonstration.ipynb`

A short demonstration notebook showing the trained models in action on an audio recording. It includes predominant instrument prediction, multilabel instrument predictions, confidence scores, comparison with ground-truth labels, and window-wise predictions for longer audio.

## Workflow — Complete Project Notebook

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

The notebooks use:

- Original IRMAS audio recordings.
- Processed NumPy feature and label arrays.
- Trained CNN models.
- Audio recordings for demonstration and prediction.

Refer to [`data/README.md`](../data/README.md) for dataset download links and instructions.

## Trained Models

The trained models are available in the [`models/`](../models/) directory.

- `best_cnn_deep.keras`
- `best_cnn_multilabel_v2.keras`

## Requirements

The notebooks use Python and the following libraries:

- NumPy
- Pandas
- Librosa
- Matplotlib
- Scikit-learn
- TensorFlow / Keras

Install the required libraries from the repository root:

```bash
pip install -r requirements.txt
```

## Execution

1. Clone or download the repository.
2. Download the required original and processed datasets.
3. Use the trained models provided in the `models/` directory.
4. Install the required Python libraries.
5. Open the notebook using Jupyter Notebook or JupyterLab.
6. Update dataset, audio, and model paths according to your local directory.
7. Execute the cells in the appropriate order.

**Note:** The notebooks may contain local file paths from the development environment. These paths must be updated before running the notebooks on another system.
