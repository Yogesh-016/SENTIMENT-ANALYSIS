# 📊 Sentiment Analysis using Python & NLP

![Python](https://img.shields.io/badge/Language-Python-blue?style=flat&logo=python)
![NLP](https://img.shields.io/badge/Technique-NLP-purple?style=flat)
![Library](https://img.shields.io/badge/Library-TextBlob-teal?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

---

## 🏢 Internship Details

| Field | Details |
|---|---|
| **Company** | CODTECH IT SOLUTIONS |
| **Name** | Yogesh S |
| **Intern ID** | CTIS3967 |
| **Domain** | Data Analysis |
| **Duration** | 4 Weeks |
| **Mentor** | Neela Santosh |
| **Task** | Task-3 – Sentiment Analysis using Python |

---

## 📖 Project Overview

This project focuses on performing **Sentiment Analysis** on textual data using **Natural Language Processing (NLP)** techniques. The goal is to analyze text content and classify it into **Positive**, **Negative**, or **Neutral** sentiments to understand public opinion and emotional trends.

The dataset contains text data along with demographic and country-level information, making it suitable for real-world sentiment analysis applications.

---

## 🎯 Objectives

- Analyze textual data using NLP techniques
- Classify sentiments as **Positive**, **Negative**, or **Neutral**
- Generate insights from unstructured text data
- Visualize sentiment distribution using charts
- Support decision-making using sentiment patterns

---

## 🛠️ Tools & Technologies Used

| Library | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data loading, manipulation & analysis |
| TextBlob | Sentiment polarity analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualizations |

---

## ⚙️ Methodology

```
1. Load & Inspect Dataset
        ↓
2. Clean & Preprocess Text Data
        ↓
3. Apply TextBlob Sentiment Analysis
        ↓
4. Calculate Polarity Score per Text Entry
        ↓
5. Classify Sentiment Based on Polarity
        ↓
6. Store Results → Predicted_Sentiment Column
        ↓
7. Visualize Sentiment Distribution
```

---

## 🧪 Sentiment Classification Logic

Sentiment is determined based on the **TextBlob polarity score** (ranging from `-1.0` to `+1.0`):

| Polarity Score | Sentiment Label |
|---|---|
| Polarity > 0 | ✅ Positive |
| Polarity < 0 | ❌ Negative |
| Polarity = 0 | ➖ Neutral |

```python
# Sentiment classification logic
def classify_sentiment(polarity):
    if polarity > 0:
        return "Positive"
    elif polarity < 0:
        return "Negative"
    else:
        return "Neutral"

df["Predicted_Sentiment"] = df["text_column"].apply(
    lambda x: classify_sentiment(TextBlob(str(x)).sentiment.polarity)
)
```

---

## 📊 Visualization

A **bar chart** displays the count distribution across all sentiment categories:

- ✅ Positive sentiments
- ❌ Negative sentiments
- ➖ Neutral sentiments

This helps in understanding overall **public opinion trends** at a glance.

### Output Preview

![Sentiment Analysis Output](https://github.com/user-attachments/assets/5a4d55f2-df49-4d53-a053-6b12a97908ea)

---

## 📂 Project Structure

```
Sentiment-Analysis/
│
├── dataset.csv                  # Input text dataset
├── sentiment_analysis.ipynb     # Main Jupyter Notebook
└── README.md                    # Project documentation
```

---

## ✅ Results

- Each text entry is labeled with a **predicted sentiment**
- Sentiment distribution is clearly **visualized** via bar chart
- Dataset is enhanced with actionable **sentiment insights**

---

## 📌 Conclusion

This project demonstrates how **NLP techniques** can be used to extract meaningful insights from unstructured text data. Sentiment analysis plays a crucial role in understanding:

- 🛒 Customer feedback & product reviews
- 📱 Social media opinions & trends
- 📈 Market sentiment & brand perception

---

## 👤 Author

**Yogesh S**  
Aspiring Data Analyst | NLP & Machine Learning Enthusiast

---

> 📝 *This project was completed as part of a Data Analysis internship at CODTECH IT SOLUTIONS.*
