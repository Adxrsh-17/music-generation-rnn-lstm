Music Generation with LSTM
🎶 This project showcases a machine learning model that generates music using Long Short-Term Memory (LSTM) networks. Trained on a dataset of classical MIDI files, the model learns musical patterns and structures to compose original pieces.
🚀 Project Overview
The core objective is to develop an LSTM-based neural network capable of generating unique musical compositions. By learning temporal relationships within sequences of musical notes, the model produces melodies that reflect the stylistic patterns of the training data.
✨ Key Features

MIDI File Parsing: Utilizes the music21 library to efficiently parse MIDI files, extracting individual notes and chords.
LSTM-Based Model: Built with LSTM layers, ideal for complex sequence prediction tasks like music generation.
Dynamic Music Generation: Generates fresh melodies from an initial seed sequence of notes post-training.
Customizable Dataset: Allows training on user-provided MIDI files to create diverse musical styles.

⚙️ Installation
To set up the project, follow these steps:

Clone the repository:
git clone https://github.com/Adxrsh-17/music-generation-rnn-lstm.git


Install dependencies:
pip install -r requirements.txt



📖 Usage
Dataset Preparation
Organize your MIDI files in the designated directory. The project includes scripts to streamline dataset organization for seamless training.
Model Training
With the dataset ready, start the training process. The LSTM model learns note relationships by processing sequences, predicting subsequent notes over multiple epochs to minimize errors.
Music Generation
After training, provide a seed sequence (a few initial notes) to generate a new melody. The model predicts subsequent notes, creating a composition that can be saved as a MIDI file for playback.
🧠 Model Architecture
The model is built on an LSTM architecture, optimized for sequence prediction in music generation. Key components include:

LSTM Layers: Capture intricate temporal dependencies in music sequences.
Dropout Layers: Prevent overfitting by randomly deactivating input units during training.
Dense Layer: Uses softmax activation to output probabilities for each possible note.
Optimizer: Adamax, efficient for training deep learning models.

🗃️ Dataset
The model is trained on a dataset of classical music in MIDI format. Each file represents a unique musical piece, processed to extract notes and chords for training. Users can train the model on their own MIDI files to explore various musical styles.
📦 Dependencies
The project requires the following Python libraries:

music21: For parsing and manipulating MIDI files.
tensorflow: For building and training the LSTM model.
numpy: For numerical computing.

Install all dependencies with:
pip install -r requirements.txt

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.
