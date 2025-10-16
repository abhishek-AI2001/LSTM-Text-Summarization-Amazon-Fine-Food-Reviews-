# LSTM Text Summarization – Amazon Fine Food Reviews

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-Notebook-orange?logo=googlecolab&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?logo=github)

## Project Overview
Text summarization is the task of creating a short, accurate, and fluent summary of a longer text document. It is a **Natural Language Processing (NLP)** application that produces meaningful summaries from lengthy paragraphs, helping us understand the essence of the text efficiently. With the ever-growing volume of text data online, automatic text summarization is essential for **discovering and consuming relevant information quickly**.

This project focuses on generating concise summaries for **Amazon Fine Food reviews** using **abstractive text summarization** with **LSTM (Encoder-Decoder) architecture** and attention mechanisms.

---

## Dataset
The original dataset from Kaggle contains **~500,000 Amazon Fine Food reviews**. To reduce training time and improve efficiency, a **random sample of 50,000 reviews** was used for building and training the model.  

**Data Source:** [Kaggle – Amazon Fine Food Reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)

---

## Types of Text Summarization
- **Abstractive Summarization:** Generates new sentences that may not be present in the original text.  
- **Extractive Summarization:** Identifies and extracts the most important sentences or phrases from the original text to form a summary.

---

## Problem Statement
Customer reviews are often long and detailed, making manual analysis time-consuming. The goal of this project is to develop an **automatic summarization system** for Amazon Fine Food reviews to produce short, meaningful summaries efficiently.

---

## Project Pipeline
1. **Understanding Text Summarization** – Overview of abstractive and extractive methods.  
2. **Text Preprocessing** – Cleaning, tokenization, contraction mapping, stopword removal, and handling rare words.  
3. **Abstractive Summarization** – LSTM (Encoder-Decoder) model with **3-layer stacked encoder** and **custom attention mechanism**.  
4. **Web Scraping (Optional)** – Using BeautifulSoup to extract text from articles.  
5. **Model Training & Evaluation** – Training on the sampled 50,000 reviews and generating concise summaries.

---

## Sample Results

### Abstractive Summarization
- **Original text:** gluten free want crackers one also delicious second order  
  **Predicted summary:** great gluten free baking  

- **Original text:** coffee tastes like regular coffee good weak used little less water regular strength coffee taste great smell better whether works stomach needed sure  
  **Predicted summary:** good coffee  

- **Original text:** first time italy wife actually give gifts well good sucks seasonal definitely makes look forward holidays  
  **Predicted summary:** the best  

### Extractive Summarization
- **Original text:** Artificial intelligence AI is intelligence demonstrated by machines as opposed to the natural intelligence displayed by humans or animals …  
  **Predicted summary:** artificial intelligence (AI) is intelligence demonstrated by machines as opposed to the natural intelligence displayed by humans or animals. Leading AI textbooks define the field as the study of intelligent agents.

---

## Technologies Used
- Python, TensorFlow, Keras  
- LSTM (Encoder-Decoder) with Attention  
- NLP preprocessing (tokenization, text cleaning, rare word handling)  
- BeautifulSoup for web scraping (optional)  

---

## License
This project is licensed under the MIT License.
