# 🎵 Music Generation with LSTM

A machine learning model that generates original music compositions using Long Short-Term Memory (LSTM) neural networks. Trained on classical MIDI files, the model learns complex musical patterns and structures, enabling it to compose unique pieces that reflect the style of its training data.

## 🚀 Project Overview

The goal of this project is to develop an LSTM-based network capable of generating dynamic and stylistically faithful musical compositions. By modeling the temporal relationships in sequences of musical notes, the network produces melodies that carry the hallmarks of the training data's style while showcasing creative variation.

## ✨ Key Features

- **MIDI File Parsing**: Utilizes the music21 library to parse and extract notes and chords from MIDI files
- **LSTM-Based Model**: Employs LSTM layers, ideal for sequence prediction tasks such as music generation
- **Dynamic Music Generation**: Generates new melodies from a user-supplied seed sequence after the model is trained
- **Customizable Dataset**: Supports user-provided MIDI datasets, enabling training on diverse musical genres and styles

## ⚙️ Installation

### 1. Clone the repository:
```bash
git clone https://github.com/Adxrsh-17/music-generation-rnn-lstm.git
cd music-generation-rnn-lstm
```

### 2. Install dependencies:
```bash
pip install -r requirements.txt
```

## 📖 Usage

### Dataset Preparation
- Organize MIDI files within the specified dataset directory
- Included scripts help streamline the dataset organization process to ensure effective training

### Model Training
- Initiate training once the dataset is prepared
- The LSTM model processes sequences of notes, learning their temporal relationships and patterns through multiple training epochs to minimize prediction error

### Music Generation
- After training, provide the model with a seed sequence (a short series of notes)
- The model generates a new melody by predicting and chaining subsequent notes
- The generated composition can be saved as a MIDI file for playback or further processing

## 🧠 Model Architecture

- **LSTM Layers**: Capture and model temporal dependencies found in musical sequences
- **Dropout Layers**: Reduce overfitting by randomly deactivating input units during training
- **Dense Output Layer**: Softmax activation function outputs the probability distribution over possible notes
- **Optimizer**: Uses the Adamax optimizer, effective for deep learning tasks

## 🗃️ Dataset

- Model has been trained and validated on classical music MIDI files
- Easily extensible to user-supplied MIDI data to enable training on a wide variety of musical styles and genres

## 📦 Dependencies

- **music21**: MIDI parsing and musicological data processing
- **tensorflow**: Deep learning model construction and training
- **numpy**: Numerical operations

Install all dependencies with:
```bash
pip install -r requirements.txt
```

## 📜 License

Distributed under the MIT License. See the `LICENSE` file for details.

---

### 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### 📧 Contact

For questions or suggestions, please open an issue on this repository.

### ⭐ Show your support

Give a ⭐️ if this project helped you!
