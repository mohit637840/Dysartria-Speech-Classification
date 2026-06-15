<img width="1536" height="1024" alt="ac612f08-2e26-487b-8542-0df3ace16d79" src="https://github.com/user-attachments/assets/184ed312-9e72-423e-be9d-ff7be4b1e004" />

# Dysarthria Speech Classification using Acoustic Features and Machine Learning

## Overview

Dysarthria is a motor speech disorder caused by neurological impairments that affect speech production and intelligibility. This project investigates whether acoustic features extracted from speech recordings can be used to automatically distinguish dysarthric speech from non-dysarthric speech.

The study combines speech signal processing techniques with machine learning models to identify acoustic patterns associated with dysarthric speech.

---

## Objectives

- Analyze speech recordings from dysarthric and healthy speakers.
- Explore acoustic differences using signal visualization techniques.
- Extract informative speech features from audio recordings.
- Develop machine learning models for dysarthria detection.
- Identify the most important acoustic characteristics for classification.

---

## Dataset

The dataset consists of speech recordings collected from dysarthric and non-dysarthric speakers.

Each sample contains:

- Audio recording (.wav)
- Speaker metadata
- Gender information
- Dysarthria label

---

## Project Workflow

Speech Recording
↓
Signal Analysis
↓
Feature Extraction
↓
Feature Engineering
↓
Machine Learning Classification
↓
Performance Evaluation

---

## Acoustic Analysis

The following speech representations were explored:

- Waveform Analysis
- Spectrogram Analysis
- RMS Energy
- Zero Crossing Rate (ZCR)
- Spectral Centroid
- Mel Frequency Cepstral Coefficients (MFCCs)

---

## Feature Engineering

For each recording, MFCC coefficients were extracted and summarized using:

- Mean
- Standard Deviation
- Minimum
- Maximum

This produced a feature set used for machine learning classification.

---

## Machine Learning Models

The following models were evaluated:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

---

## Results

Key findings:

- MFCC-based acoustic features effectively distinguish dysarthric and non-dysarthric speech.
- Random Forest and Support Vector Machine achieved approximately **94% classification accuracy**.
- Feature importance analysis identified several MFCC statistics as highly discriminative.

---

## Future Work

Future development will focus on:

- RMS-based features
- Spectral centroid features
- Pitch and prosodic features
- Chroma features
- Deep learning models (CNN, CNN-LSTM)
- Dysarthric Speech Recognition (ASR)
- Speech-to-Text Assistive Systems

---

## Long-Term Vision

The ultimate goal of this project is to develop an assistive communication system capable of automatically understanding and transcribing dysarthric speech, helping improve communication accessibility for individuals with speech impairments.

---

## Technologies Used

- Python
- NumPy
- Pandas
- Librosa
- Matplotlib
- Seaborn
- Scikit-Learn
