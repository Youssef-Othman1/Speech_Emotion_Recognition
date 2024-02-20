# Speech Emotion Recognition
Speech Emotion Recognition: A CNN-based model for predicting human emotions from audio signals using TensorFlow and Keras. Utilizes CREMA dataset and implements preprocessing, feature extraction, data augmentation, and model training.

## Introduction
### Problem Statement
The objective is to develop a model capable of discerning embedded emotions within an audio signal. This report proposes a speech emotion recognition model utilizing Convolutional Neural Network (CNN) architecture to predict human emotions by learning segmented audio samples of specific emotional states.

## Dataset Description
### Overview
The dataset utilized is CREMA, comprising 7442 audio files, with each file corresponding to a distinct emotion. The dataset encompasses six emotions: Sadness, Fear, Happiness, Anger, Disgust, and Neutral.

## Audio Preprocessing
Several preprocessing techniques were explored for the audio data:
- Noise Reduction
- Silence Removal
- Pre-emphasis
- Normalization
- Truncation and Padding

## Feature Spaces
Two feature spaces were created from the audio:
1. Time Domain and Frequency Domain for 1D convolution
2. Spectrograms for 2D convolution

### Features for 1D Convolution
- Energy
- Entropy of Energy
- Zero Crossing Rate
- Root Mean Square
- Spectral Centroid
- Spectral Centroid Roll Off

### Spectrogram (2D Convolution)
A spectrogram visualizes the frequency content of a signal over time, allowing analysis of spectral components' changes.

## Data Augmentation
Augmentation techniques applied:
- Noise addition
- Shifting
- Pitch shifting

## Model Training
The CNN model architecture:
- Utilizes libraries such as TensorFlow and Keras
- The model achieved 52.75% accuracy on the test set for the 1D model and 55.40% for the 2D model, which are considered considerably acceptable and high on the given dataset.
