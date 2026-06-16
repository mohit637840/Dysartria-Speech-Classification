# Dysarthria Speech Classification using Acoustic Signal Analysis and Machine Learning
<img width="1536" height="1024" height="686" alt="WhatsApp Image 2026-06-16 at 8 18 47 PM" src="https://github.com/user-attachments/assets/aac778d8-2b57-49e5-9f7a-6c273828112f" />

## Overview

Dysarthria is a motor speech disorder caused by neurological impairments that affect speech production and intelligibility. This project explores whether acoustic features extracted from speech recordings can be used to automatically distinguish dysarthric speech from non-dysarthric speech.

The project combines speech signal processing techniques with machine learning models to identify acoustic patterns associated with dysarthric speech.

---

## Project Goals

* Analyze acoustic differences between dysarthric and healthy speech.
* Extract informative speech features from audio recordings.
* Develop machine learning models for automated dysarthria detection.
* Identify the most important acoustic characteristics for classification.
* Build a foundation for future dysarthric speech recognition and assistive communication systems.

---

## Dataset

The dataset consists of speech recordings collected from dysarthric and non-dysarthric speakers.

Each sample contains:

* Audio recording (.wav)
* Speaker metadata
* Gender information
* Dysarthria label

---

## Methodology

### 1. Exploratory Audio Analysis

The following signal representations were explored:

* Waveform Analysis
* Spectrogram Analysis
* RMS Energy
* Zero Crossing Rate (ZCR)
* Spectral Centroid
* MFCC Visualization

### 2. Feature Extraction

Mel Frequency Cepstral Coefficients (MFCCs) were extracted from each speech recording.

For every MFCC coefficient, the following statistical features were computed:

* Mean
* Standard Deviation
* Minimum
* Maximum

This produced a feature set used for machine learning classification.

### 3. Machine Learning Models

The following models were evaluated:

* Logistic Regression
* Random Forest
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)

### 4. Model Evaluation

Performance was assessed using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* 5-Fold Stratified Cross-Validation

---

## Results

### Cross-Validation Performance

| Model               | Mean F1 Score |
| ------------------- | ------------: |
| SVM                 |        94.35% |
| Random Forest       |        94.29% |
| KNN                 |        94.16% |
| Logistic Regression |        85.81% |

### Key Findings

* MFCC-based acoustic features effectively distinguish dysarthric and non-dysarthric speech.
* Multiple machine learning models achieved F1 scores above 94%.
* Cross-validation confirmed the robustness and stability of the classification pipeline.
* Feature importance analysis identified several MFCC statistics as highly informative.

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

## Technologies Used

* Python
* NumPy
* Pandas
* Librosa
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Future Work

Future development will focus on:

* RMS-based features
* Pitch and prosodic features
* Chroma features
* Spectral Roll-off
* Spectral Bandwidth
* Speaker-level validation
* Feature selection techniques
* CNN-based models
* CNN-LSTM architectures
* Dysarthric Speech Recognition (ASR)

---
## Long-Term Vision

The ultimate goal of this project is to move beyond speech classification and develop an assistive communication system capable of automatically understanding and transcribing dysarthric speech, helping improve communication accessibility for individuals with speech impairments.

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Librosa](https://img.shields.io/badge/Librosa-Audio%20Processing-green)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
