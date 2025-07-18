Music Generation with LSTM
🎶 A machine learning model that generates music using Long Short-Term Memory (LSTM) networks. Trained on classical MIDI files, it learns musical patterns and structures to compose original pieces.
🚀 Project Overview
The goal is to develop an LSTM-based neural network to generate unique musical compositions. By learning temporal relationships within note sequences, the model produces melodies reflecting the training data's stylistic patterns.
✨ Key Features

MIDI File Parsing: Uses the music21 library to parse MIDI files and extract notes and chords.
LSTM-Based Model: Built with LSTM layers for complex sequence prediction tasks like music generation.
Dynamic Music Generation: Generates melodies from an initial seed sequence of notes post-training.
Customizable Dataset: Supports training on user-provided MIDI files for diverse musical styles.

⚙️ Installation

Clone the repository:
git clone https://github.com/Adxrsh-17/music-generation-rnn-lstm.git


Install dependencies:
pip install -r requirements.txt



📖 Usage
Dataset Preparation
Organize your MIDI files in the designated directory. Included scripts streamline dataset organization for seamless training.
Model Training
With the dataset ready, start training. The LSTM model learns note relationships by processing sequences and predicting subsequent notes over multiple epochs to minimize errors.
Music Generation
Post-training, provide a seed sequence (a few initial notes) to generate a new melody. The model predicts subsequent notes, creating a composition savable as a MIDI file.
🧠 Model Architecture

LSTM Layers: Capture temporal dependencies in music sequences.
Dropout Layers: Prevent overfitting by deactivating input units during training.
Dense Layer: Uses softmax activation for note probability output.
Optimizer: Adamax, efficient for deep learning model training.

🗃️ Dataset
Trained on classical music MIDI files, processed to extract notes and chords. Users can train on their own MIDI files for varied styles.
📦 Dependencies

music21: For MIDI file parsing and manipulation.
tensorflow: For building and training the LSTM model.
numpy: For numerical computing.

Install with:
pip install -r requirements.txt

📜 License
Licensed under the MIT License. See the LICENSE file for details.
