# 📰 News Classification using BERT

## 📌 Project Overview

This project focuses on **multi-class text classification** using the **BERT Transformer** model. The objective is to classify news articles into one of four categories:

- 🌍 World  
- 💼 Business  
- 🧪 Technology / Science  
- 🏅 Sports

This task was assigned as part of a real-world internship at **Developer Hub Corporation** during June–July 2025, with an emphasis on deploying state-of-the-art NLP models using practical data.

---

## 🧠 Model: BERT (Bidirectional Encoder Representations from Transformers)

- Used `bert-base-uncased` from Hugging Face Transformers
- Fine-tuned on the **AG News** dataset
- Handled variable-length text using attention masks and padding
- Tokenized using `BertTokenizerFast`

---

## 🛠️ Workflow

1. **Data Preparation**
   - Loaded and preprocessed AG News dataset
   - Encoded target labels into numerical format
2. **Text Tokenization**
   - Used BERT tokenizer with truncation and padding
   - Created attention masks for proper transformer input
3. **Model Fine-Tuning**
   - Used `BertForSequenceClassification`
   - Optimized with `AdamW` and a scheduler for learning rate decay
   - Used PyTorch & Hugging Face `Trainer` API
4. **Evaluation**
   - Accuracy
   - F1-score
   - Confusion Matrix

---

---

## 💡 Key Takeaways

- Transfer learning significantly boosts performance on small datasets
- BERT embeddings capture contextual meaning effectively
- Using `Trainer` class simplifies training and evaluation workflows

---

## 🗂️ Files

- `news_classifier.ipynb`: Full Jupyter notebook for training & evaluation
- `model/`: Saved fine-tuned BERT model
---

## ✅ Future Work

- Add GUI/web interface for real-time news classification

