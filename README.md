# Mental Rotation EEG Emotion Classification

A PyTorch-based deep learning framework for classifying emotional states from multimodal physiological data (EEG, eye-tracking, GSR) during mental rotation tasks using RNN-HMM hybrid models.

##Dataset

Uses the Multisensor Mental Rotation Dataset with EEG, IVT, TIVA, EYE, GSR, and PSY modalities.

## Features

- **Multimodal Synchronization**: Aligns EEG, eye-tracking, GSR, and facial data using trial windows
- **RNN-HMM Hybrid**: Combines LSTM/GRU temporal modeling with Hidden Markov Models
- **Data Augmentation**: Temporal warping, noise addition for small datasets
- **5Hz Downsampling**: Consistent sampling rate across all modalities

##Model Architecture

· Input: Synchronized multimodal time-series data
· RNN: Bidirectional LSTM/GRU with attention
· HMM: Gaussian HMM for hidden state modeling
· Output: Binary classification (correct/incorrect trials)

##Results

· Cross-validated performance on limited datasets
· Data augmentation for small sample sizes
· Comprehensive visualization and analysis tools
