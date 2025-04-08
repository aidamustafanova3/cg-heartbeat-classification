# ECG Heartbeat Classification (MIT-BIH)

This project classifies ECG signals into 5 heartbeat categories using a Multi-Layer Perceptron (MLP) built in PyTorch.

## Dataset: https://drive.google.com/drive/folders/1I_V3eevszHlFXQt2O2JavsNYoBXKOAMh?usp=sharing

- **MIT-BIH Arrhythmia**  
- 87,553 training samples, 21,891 test samples  
- Each sample contains 187 time-series points  
- Classes:  
  - 0: Normal  
  - 1: Atrial Premature  
  - 2: Ventricular Contraction  
  - 3: Fusion of Ventricular and Normal  
  - 4: Fusion of Paced and Normal  

## Model Architecture

- Input: 187 features  
- Hidden layers: 128 → 64 neurons (ReLU)  
- Dropout: 0.3  
- Output: 5 classes  
- Loss: CrossEntropyLoss  
- Optimizer: Adam (lr=0.001)  
- Epochs: 20, Batch size: 32

## 📈 Results

- Monitored training loss and accuracy  
- Evaluated using precision, recall, F1-score  
- Visualized training dynamics and sample ECG signals

## 📦 Requirements
torch
numpy
pandas
matplotlib
seaborn
plotly
scikit-learn



