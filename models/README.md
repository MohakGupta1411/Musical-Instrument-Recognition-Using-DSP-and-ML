# Trained Models

This directory contains the trained CNN models developed for the Musical Instrument Recognition project using DSP and Machine Learning.

## Model Files

| Model | Description |
|---|---|
| `best_cnn_deep.keras` | Trained CNN model for predominant single-instrument classification. |
| `best_cnn_multilabel_v2.keras` | Trained CNN model for multilabel instrument recognition. |

## Model Details

### 1. Single-Instrument Classification

The deep CNN model identifies the predominant musical instrument in an audio recording.

### 2. Multilabel Classification

The multilabel CNN model identifies multiple instruments that may be present in a musical recording.

## Framework

The models were developed and trained using TensorFlow and Keras.

## Usage

Load the models using TensorFlow/Keras:

```python
from tensorflow.keras.models import load_model

# Load single-instrument model
model_single = load_model("models/best_cnn_deep.keras")

# Load multilabel model
model_multi = load_model("models/best_cnn_multilabel_v2.keras")
```

The models are trained on processed audio features. Refer to the project notebook for preprocessing details and prediction implementation.

