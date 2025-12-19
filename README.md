# 📰 Fake News Detection using NLP & Machine Learning

A complete end-to-end project to classify **Fake vs True** news articles using **Natural Language Processing (NLP)**, **TF-IDF**, and **Multinomial Naive Bayes**.

---

## 📌 Project Overview

This project focuses on detecting fake news by analyzing text patterns from real and fabricated news articles. The workflow includes:

- Dataset merging  
- Text preprocessing  
- Feature engineering (TF-IDF)  
- Model training  
- Evaluation & error analysis  

The goal is to build a reliable ML model that can identify misleading or false news content.

---

## 📂 Dataset

The project uses two datasets:

- **True.csv** → Real news articles  
- **Fake.csv** → Fake or fabricated articles  

A new label is added:  
- `1` → True News  
- `0` → Fake News  

Both files are combined and shuffled for unbiased training.

---

## 🧹 Data Preprocessing

- Removed special characters & numbers  
- Lowercased all text  
- Tokenized text  
- Removed stopwords  
- Applied **lemmatization**  
- Combined `title + text`  
- Extracted features using **TF-IDF**  

---

## 🧠 Model Used

### **Multinomial Naive Bayes (MNB)**

Chosen because:

- Works extremely well for text classification  
- Efficient for large vocabularies  
- Fast training and prediction  

---

## 📊 Model Evaluation

The model is evaluated using:

- **Accuracy Score**  
- **Precision, Recall, F1-score**  
- **Confusion Matrix**  
- **ROC Curve / AUC Score**  

Results show strong performance and clear separation between Fake and True articles.

---

## 🔍 Key Insights

- TF-IDF captures clear differences in word usage between fake and real news.  
- Naive Bayes provides a strong and efficient baseline model.  
- Misclassifications occur when:
  - Fake news is structured like real journalism  
  - Real news uses emotional or sensational wording  

---

## ⚙️ Model Behaviour (Short)

- Learns fake vs real patterns from text.  
- Flags misleading or sensational writing as fake.  
- Handles large text data efficiently.  
- May misclassify when writing styles overlap.

---

## 📁 Project Structure
|── True.csv       
├── Fake.csv         
├── Fake News Detection.ipynb       
├── README.md       

---
## 🔮 Future Improvements
- Evaluate other ML models (LR, SVM, Random Forest)
- Add n-grams for richer context
- Try advanced models like BERT
- Build a Streamlit/Flask app for deployment
  
---
## 👨‍💻 Author

**Venkatesh Vijay Karnure**  
🔗 [LinkedIn](https://www.linkedin.com/in/venkateshk2003)  
💻 [GitHub](https://github.com/Venkatesh9372)
