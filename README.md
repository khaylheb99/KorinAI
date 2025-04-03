# Audio Genre Classification and Melody Generation

## Overview
This project consists of two main components:
1. **Melody Generation** – A rule-based system using the `music21` library to generate melodies based on predefined musical templates for different genres (Afrobeat, Fuji, Jazz).
2. **Audio Genre Classification** – A machine learning model trained on the GTZAN dataset to classify audio files into different genres based on extracted features.

## Features
- **Generate Melodies**: Uses predefined scales, tempos, and rhythmic patterns.
- **Genre Classification**: Utilizes machine learning techniques to classify audio files.
- **Kaggle Integration**: Automatically downloads the GTZAN dataset for training and evaluation.

## Installation
To run this project, ensure you have Python installed and set up a virtual environment (optional but recommended):

```sh
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

Then, install the required dependencies:
```sh
pip install -r requirements.txt
```

## Running the Project

### 1. Melody Generation
To generate a melody for a specific genre, run:
```sh
python melody_generator.py --genre Fuji --duration 30 --output fuji.mid
```
Supported genres: `Afrobeat`, `Fuji`, `Jazz`

### 2. Audio Genre Classification
First, ensure the dataset is downloaded:
```sh
python download_dataset.py
```

Then, extract features and train the model:
```sh
python train_model.py
```

To classify a new audio file:
```sh
python classify_audio.py --file path/to/audio.wav
```

## Dataset
This project uses the GTZAN dataset from Kaggle. The script `download_dataset.py` fetches and extracts it automatically.

## Improvements & Future Work
- Integrate deep generative models for more complex melody generation.
- Enhance the classifier with CNN-based spectrogram analysis.
- Deploy the model as a web application for real-time predictions.
