# KorinAI

# Audio Genre Classification and Melody Generation

## Overview
This project consists of two main components:
1. Melody Generation – A rule-based system using the `music21` library to generate melodies based on predefined musical templates for different genres (Afrobeat, Fuji, Jazz).
2. Audio Genre Classification – A machine learning model trained on the GTZAN dataset to classify audio files into different genres based on extracted features.

## Features
- Generate Melodies: Uses predefined scales, tempos, and rhythmic patterns.
- Genre Classification: Utilizes machine learning techniques to classify audio files.
- Kaggle Integration: Automatically downloads the GTZAN dataset for training and evaluation.

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
First, ensure the dataset is downloaded
Then, extract features and train the model.

## Dataset
This project uses the GTZAN dataset from Kaggle. The script that fetches and extracts it automatically is written there.

