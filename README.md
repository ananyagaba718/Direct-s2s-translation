# 🎙️ Speech-to-Speech Translation (German ➝ English)

An end-to-end neural network-based system that directly translates spoken German audio into English speech — without using intermediate text representation.

## 🚀 Features
- 🎤 Accepts spoken German input via microphone or audio file
- 🎧 Outputs translated English speech using waveform reconstruction
- 🔁 No intermediate text layer — direct audio-to-audio mapping
- 🎯 Built using MFCC feature extraction, RNN-based sequence modeling, and Griffin-Lim algorithm

## 🧠 Model Architecture
- **Input Processing**: Extracts MFCCs from input audio
- **Model**: Sequence-to-sequence **RNN encoder-decoder** trained on paired audio embeddings
- **Output**: English MFCC sequence reconstructed into speech

## 🛠 Tech Stack
- Python, NumPy, Librosa, TensorFlow/Keras
- MFCC, RNN, Seq2Seq, Griffin-Lim
- Speech Recognition and Audio Playback

## 📊 Accuracy & Testing
- Trained on a subset of German-English audio pairs
- Focused on short sentence translation
- Evaluated on translation clarity and output waveform quality

## 📁 Project Structure
```bash
├── data/              # Preprocessed audio data
├── model/             # Training scripts and saved models
├── utils/             # Feature extraction, reconstruction tools
├── app.py             # Main app interface
├── requirements.txt   # Required libraries
└── README.md
