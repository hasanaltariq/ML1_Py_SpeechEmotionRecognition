# Speech Emotion Recognition



## The Challenge

Recognize a person’s emotion from his/her speech. 

## Assumption
Voice often reflects underlying emotion through tone and pitch. By converting audio signals to numerical values, we can extract features from the sound file and annotate as necessary. Using a supervised learning approach, we can train classifiers to learn and detect emotions.

## Data
For this project we will use a modified (reduced sample rate) version of Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS) dataset, which can be downloaded from [here](https://drive.google.com/file/d/1wWsrN2Ep7x6lWqOXfr4rpKGYrJhWc8z7/view ). This dataset has 7356 files rated by 247 individuals 10 times on emotional validity, intensity, and genuineness.

## Methodology
We will use [librosa 0.8.0](https://librosa.org/doc/latest/index.html), which is a Python library for analyzing audio and music as well as [pysoundfile -0.10.2](https://pysoundfile.readthedocs.io/en/latest/) library. 

Steps:
1. Load required libraries
2. Define a function for features extraction from audio files
3. Define a dictionary for emotions
4. Define a function to create a dataset by loading audio files and extracting features from those files.
5. Load, create and split dataset
6. Initialize feedforward ANN model: [Multi-layer Perceptron classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html)
7. Train and test the model
8. Measure performance
9. Future improvement: Parameter optimization, Different classifier (XGB)

## Measurement Criteria
    Accuracy

## Requirements
    Python 3.8, (Jupyter Notebook), pandas-1.1.1, numpy-1.19.1, scipy-1.5.2, scikit-learn-0.23.2, matplotlib-3.3.1, librosa 0.8.0, pysoundfile -0.10.2

## Disclaimer
We have reproduced the code for educational and learning purposes only. Original article can be found [here](https://data-flair.training/blogs/python-mini-project-speech-emotion-recognition/).



