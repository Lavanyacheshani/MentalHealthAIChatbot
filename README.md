# Chatbot for Mental Health 🤖🧠

A Python-based compilation of **rule-based**, **retrieval-based**, and **generative-based** chatbots trained on a mental health FAQ dataset. This project was developed as part of a university research collaboration to explore different chatbot design approaches for accessible mental health support.

> ⚠️ This repository uses a **sample dataset from Kaggle** as the original dataset used in the research is confidential.

---

## 🔧 Updates 
- ✅ Fixed outdated library and method issues
- ✅ Added `requirements.txt` for easier dependency installation
- ⚠️ Ensure you're using **Python 3.8** (or lower) for compatibility with libraries like TensorFlow

---

## 🧠 Motivation

Sri lanka's 2017 National Mental Health Survey reported that **1 in 7** people suffer from mental health disorders such as depression and anxiety. Nearly **150 million** people need mental health intervention — most without access due to affordability and stigma.

This project aims to make mental health more accessible by providing a foundation for conversational agents that can complement clinicians in therapeutic settings.

---

## 🧩 Chatbot Types Implemented

### 1. Rule-Based Chatbot
- Uses pattern matching with **TF-IDF** and **cosine similarity**
- Built with **NLTK** for preprocessing
- Simple but effective for closed-domain questions

### 2. Retrieval-Based Chatbot
- Trained on **manually converted JSON** data
- Models implemented:
  - Vanilla RNN
  - LSTM
  - Bi-LSTM
  - GRU
  - CNN (performed best)
- Best model: **CNN + Embedding + Dense Layer**
- Regularized with dropout and validated for loss/accuracy

### 3. Generative-Based Chatbot
- Trained using **seq2seq encoder-decoder** architecture (LSTM)
- Uses NLP techniques for conversational mimicry
- Learns to generate context-aware responses dynamically

---

## 📁 Dataset Used

- Sample: [Kaggle – Mental Health FAQ](https://www.kaggle.com/datasets) *(link to actual dataset if possible)*
- 98 Questions and Answers (only 20 used in this open-source version)
- Retrieval-based bot uses **JSON**, while generative bot uses **CSV**

---

## 🆚 JSON vs CSV (Why Both?)
| File Type | Use Case | Reason |
|-----------|----------|--------|
| JSON | Retrieval-Based Bot | Hierarchical format with tags and intents is ideal for mapping input to predefined responses |
| CSV  | Generative-Based Bot | Simpler structure with input-output pairs; easier to manipulate |

---

## 🛠️ Technologies Used

- **Python 3.8**
- **NLTK**, **Scikit-learn**, **TensorFlow/Keras**, **NumPy**, **Pandas**
- **TF-IDF**, **Cosine Similarity**
- **RNN**, **LSTM**, **Bi-LSTM**, **GRU**, **CNN**
- **Encoder-Decoder (seq2seq)**
- **Jupyter Notebooks**

---

## 🚀 How to Run

1. **Install Python 3.8**  
   (Use [pyenv](https://github.com/pyenv/pyenv) or a virtual environment manager)

2. **Clone the repository**  
   ```bash
   git clone https://github.com/YOUR_USERNAME/Chatbot-for-Mental-Health.git
   cd Chatbot-for-Mental-Health
