# music-generation-rnn-lstm

Music Generation Using LSTM
This repository contains a machine learning project for generating music using Long Short-Term Memory (LSTM) networks. The model is trained on a dataset of classical MIDI files, and it is capable of generating new musical compositions by learning patterns and structures from the dataset.

Project Overview
The goal of this project is to build a neural network model using LSTM (Long Short-Term Memory) networks that can generate original music compositions after being trained on a collection of MIDI files. The LSTM model is designed to learn temporal relationships in sequences of musical notes and generate new compositions that mimic the patterns in the dataset.

Key Features
MIDI File Parsing: The project uses the music21 library to parse MIDI files and extract musical notes and chords.

LSTM-Based Model: The model is built using LSTM layers, ideal for sequence prediction tasks such as music generation.

Music Generation: After training, the model can generate new melodies based on an initial sequence of notes.

Customizable Dataset: Users can train the model on their own MIDI files to generate different styles of music.

Installation
To get started with this project, you’ll need to install the required dependencies. You can do so by cloning the repository and installing the necessary packages using pip:

Clone the repository:

bash
Copy
Edit
git clone https://github.com/Adxrsh-17/music-generation-rnn-lstm.git
Install the dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Usage
Dataset Preparation
Before training the model, you need to prepare the dataset. The MIDI files must be placed in the designated directory. The script handles the movement and organization of the dataset files for easy access during training.

Model Training
Once the dataset is prepared, the next step is to train the model. The training process involves feeding sequences of musical notes into the LSTM model, which learns the relationships between the notes to predict subsequent notes. The model is trained over several epochs to minimize prediction errors.

Music Generation
Once the model is trained, it can generate new music. You can input a seed sequence (a few initial notes), and the model will predict the next notes, creating a melody that follows the patterns it learned during training. The generated music can be saved as a MIDI file for playback.

Model Architecture
The model is based on an LSTM architecture, which is well-suited for sequence prediction tasks such as time-series analysis and music generation. Key components of the architecture include:

LSTM Layers: The core of the model, designed to capture the temporal dependencies in music sequences.

Dropout Layers: Used to reduce overfitting during training by randomly setting a fraction of the input units to 0.

Dense Layer: The final output layer with a softmax activation function that produces the probabilities for each possible note in the sequence.

The architecture is optimized using the Adamax optimizer, which is known for its efficiency in training deep learning models.

Dataset
This model is trained on a dataset of classical music in MIDI format. The dataset consists of individual MIDI files, each representing a musical piece. These files are processed to extract notes and chords, which are then used to train the LSTM model. You can train the model on your own MIDI files to create music in different styles.

Dependencies
The project requires the following Python libraries:

music21: A Python toolkit for computer-assisted musicology that is used to parse and manipulate MIDI files.

tensorflow: An open-source machine learning library for building and training the LSTM model.

numpy: A fundamental package for numerical computing in Python.

To install the dependencies, run the following command:

bash
Copy
Edit
pip install -r requirements.txt
License
This project is licensed under the MIT License - see the LICENSE file for details.
