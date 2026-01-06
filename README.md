# Simple Audio Retrieval Project

This project implements a music information retrieval system using the **Free Music Archive (FMA)** dataset. It utilizes audio signal processing techniques (MFCC feature extraction) and machine learning (K-Nearest Neighbors) to identify and retrieve similar audio tracks based on their acoustic characteristics.

## 🚀 Overview
The project covers the full pipeline of an audio retrieval system:
- **Data Loading:** Efficiently parsing complex multi-indexed metadata from the FMA dataset.
- **Feature Engineering:** Extracting Mel-frequency cepstral coefficients (MFCCs) and calculating statistical moments (mean, std, skewness, etc.).
- **Visualization:** Reducing dimensionality with PCA to visualize genre clusters in a 2D space.
- **Retrieval Engine:** Implementing a K-Nearest Neighbors (KNN) model to find the most similar tracks to a query audio file.

## 📊 Dataset
The project uses the **fma_small** subset of the [FMA: A Dataset For Music Analysis](https://github.com/mdeff/fma), which contains 8,000 tracks of 30 seconds each, distributed across 8 balanced genres.

## 🛠️ Installation
To run this project locally, ensure you have Python 3.x installed along with the following libraries:

```bash
pip install numpy pandas scipy scikit-learn matplotlib librosa
```

Note: You may also need ffmpeg installed on your system for librosa to process MP3 files.
