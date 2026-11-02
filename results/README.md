# Results and Performance

This directory contains the experimental results and performance evaluation of the CNN-based Musical Instrument Recognition system.

## 1. Single-Instrument Classification

The deep CNN model was evaluated on the held-out test dataset.

| Metric | Result |
|---|---:|
| Test Accuracy | 75.25% |
| Test Loss | 0.7513 |
| Test Samples | 1,006 |

The model predicts the predominant musical instrument present in an audio recording.

## 2. Multilabel Instrument Classification

The multilabel CNN model was evaluated on the official IRMAS test set.

| Metric | Result |
|---|---:|
| Micro-F1 Score | 0.6208 |
| Test Samples | 2,874 |

The multilabel model is designed to identify multiple instruments that may be present simultaneously in a musical recording.

## 3. Prediction Examples

The notebook includes examples of instrument predictions along with their confidence scores.

The results demonstrate the system's ability to recognize musical instruments from Mel-spectrogram representations of audio signals.

## 4. Evaluation

The single-instrument model is evaluated using classification accuracy and loss.

The multilabel model is evaluated using the micro-F1 score, which considers the overall precision and recall across instrument labels.

## 5. Reproducibility

The trained models are available in the [`models/`](../models/) directory.

The complete experimental workflow, including preprocessing, model training, evaluation, and prediction, is provided in the [`notebooks/`](../notebooks/) directory.
