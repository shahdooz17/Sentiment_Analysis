# 🎯 Sentiment Analysis using IMDB Dataset  

This project performs **Sentiment Analysis** on the **IMDB dataset** using a deep learning model built with **TensorFlow** and **Keras**. The model leverages **LSTM (Long Short-Term Memory)** layers and pre-trained **GloVe (Global Vectors for Word Representation)** embeddings to improve accuracy.

---

## 🚀 Project Overview  
The goal of this project is to classify movie reviews from the IMDB dataset as either **positive** or **negative** based on their sentiment. The dataset contains **50,000 reviews**, with an equal split of positive and negative sentiments.

---

## 📂 Dataset  
- **IMDB Dataset:** The IMDB dataset can be downloaded from [here](https://ai.stanford.edu/~amaas/data/sentiment/).  
- **GloVe Embeddings:** Pre-trained GloVe embeddings can be downloaded from the official Stanford NLP page [here](https://nlp.stanford.edu/projects/glove/).  

---

## 🛠️ Technologies Used  
- **Python**  
- **TensorFlow**  
- **Keras**  
- **LSTM**  
- **GloVe Embeddings**  

---

## 📥 Setup Instructions  
### 1. Clone the repository:  
```bash
git clone https://github.com/your-repo/sentiment-analysis.git
cd sentiment-analysis
```
### 2. Create a virtual environment and install dependencies:
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```
### 3. Download the IMDB dataset and extract it:
```bash
curl -L -o imdb-dataset.zip https://ai.stanford.edu/~amaas/data/sentiment/aclImdb_v1.tar.gz
tar -xvzf imdb-dataset.zip
```
### 4. Download GloVe embeddings and extract them:
```bash
curl -L -o glove.6B.zip http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip
```
## 🧠 Model Architecture  
- **Embedding Layer** – Pre-trained GloVe embeddings (100 dimensions)  
- **LSTM Layer** – Captures long-term dependencies  
- **Dense Layers** – Fully connected layers for classification  

---

## 📊 Training  
- **Training data:** 40,000 reviews  
- **Validation data:** 10,000 reviews  
- **Optimizer:** Adam  
- **Loss Function:** Binary Crossentropy  

---

## 🚀 Usage  
### Train the model:  
```bash
python train.py
```
## 🎯 Results  
- **Training Accuracy:** ~90%  
- **Test Accuracy:** ~88%  

---

## 📚 References  
- **IMDB Dataset:** [https://ai.stanford.edu/~amaas/data/sentiment/](https://ai.stanford.edu/~amaas/data/sentiment/)  
- **GloVe Embeddings:** [https://nlp.stanford.edu/projects/glove/](https://nlp.stanford.edu/projects/glove/)  
- **TensorFlow:** [https://www.tensorflow.org/](https://www.tensorflow.org/)  

---
## ✅ Future Improvements  
- Try different embedding sizes (e.g., `50d`, `200d`)  
- Fine-tune the LSTM model  
- Experiment with bidirectional LSTM  
