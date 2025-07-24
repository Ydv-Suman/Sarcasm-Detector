# 🤖 Sarcasm Detection


---

## 📖 Overview

Sarcasm is a nuanced form of communication where the intended meaning often contradicts the literal wording. In this project, we build a deep‑learning pipeline to detect sarcasm in text. Starting from raw headlines and comments, we apply modern NLP techniques—tokenization, embeddings, and sequence modeling—to distinguish sarcastic from non‑sarcastic utterances with state‑of‑the‑art accuracy.

---

## 🏷 Problem Statement

> **Can we automatically identify sarcasm in short text (e.g., headlines or tweets) using deep learning?**

- **Input:** Raw text samples (headlines, comments).  
- **Output:** Binary label —  
  - `1` = sarcastic  
  - `0` = non‑sarcastic  

---

## 📊 Dataset

We use the public [“News Headlines Dataset For Sarcasm Detection”](https://www.kaggle.com/datasets/rmisra/news-headlines-dataset-for-sarcasm-detection) containing JSON lines with:

| Field              | Description                               |
|--------------------|-------------------------------------------|
| `headline`         | Text of the news headline                 |
| `is_sarcastic`     | 1 = sarcastic, 0 = not sarcastic          |
| `article_link`     | URL of the full article (unused)          |

_Raw JSON is split into a training set (23,000 samples) and a test set (remaining samples)._

---

## 🔍 Features

- **Text length** (number of words, characters)  
- **Punctuation counts** (!, ?, …)  
- **Word n‑grams** (via tokenization)  
- **Embedding vectors** (pre‑trained or learned)

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher  
- `pip` package manager  

### Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/sarcasm-detection.git
   cd sarcasm-detection
