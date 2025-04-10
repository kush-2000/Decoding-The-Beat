# Decoding the beat
Predicting Music Genres with Audio Features

[Medium Blog : Decoding the Beats ](https://medium.com/@ksimmonds92/decoding-the-beat-predicting-music-genres-with-audio-features-6ec2ee9dae52)


# Project Overview

The project applies machine learning and deep learning to classify music tracks into genres based on audio features extracted using Librosa. This project enhances music streaming services by improving genre identification accuracy, facilitating more personalized user experiences. By analyzing tempo, harmony, and other key audio signatures across ten diverse genres, our models demonstrate how AI can revolutionize music categorization and deepen our interaction with music.

## Dataset

The dataset consists of 1000 audio tracks each 30 seconds long. It covers ten musical genres and is sourced from the GTZAN genre collection. We augmented this with additional data from YouTube to enhance the model's accuracy and robustness.

## Features

We utilized Librosa to extract various audio features:
- **Chroma Features**: Chroma_stft, Chroma_cqt, Chroma_cens
- **Spectral Features**: Spectral centroid, spectral bandwidth, spectral rolloff
- **Temporal Features**: Zero-crossing rate, RMS
- **MFCCs**: Mel-frequency cepstral coefficients
- **Tempo**

## Models

We implemented several models to address the genre classification task:
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)
- Random Forest
- XGBoost
- Convolutional Neural Network (CNN)

Each model's performance is documented in the Results section, highlighting the effectiveness of ensemble methods and deep learning techniques.

## Results

Our models demonstrated varying levels of success:
- **Decision Tree**: Overfitting with high training accuracy but low test accuracy.
- **KNN**: Struggled with complex feature dimensions.
- **Random Forest and XGBoost**: Showed robust performance with high accuracy and AUC scores.
- **CNN**: Provided good results, especially in capturing spatial and temporal patterns in the spectrogram data.

## Future Work

- **Multi-label Classification**: To handle songs with blended genres, expanding the model's ability to classify more complex music categorizations.
- Additional efforts will focus on refining models and incorporating real-time data processing capabilities for live streaming applications.

