# 🚀 NLP and LLM Practice Exercises

This repository contains my solutions for NLP and LLM practical exercises covering:

✅ Topic Modeling (LDA & NMF)  
✅ Sentiment Analysis (VADER & Transformers)  
✅ Spam Classification (zero-shot classification)  
✅ Chatbot with Streamlit & Transformers

---

## 📁 Folder Structure


---

## 📝 Exercise Summaries

### 1. Topic Modeling

**Objective:** Extract topics from the *newsgroups* dataset using LDA and NMF.

**Steps:**

- Load data using pickle
- Text cleaning (lowercase, remove punctuation, stopwords, lemmatization)
- Vectorize using CountVectorizer & TfidfVectorizer
- Apply **LDA** and **NMF** to extract 10 topics each
- Plot top 10 words per topic
- Generate WordClouds of significant words

✔️ **Libraries used:** pandas, sklearn, gensim, matplotlib, seaborn, wordcloud

---

### 2. Sentiment Analysis

**Objective:** Perform sentiment analysis on tweets dataset using:

✅ **VADER (lexicon-based)**  
✅ **Transformers pipeline (pre-trained neural model)**

**Steps:**

- Load `tweets-data.csv`
- Sample 500 rows
- Clean text (lowercase, remove URLs, mentions, hashtags, punctuation, stopwords)
- Apply **VADER** to get sentiment label and score
- Apply **Transformers** sentiment pipeline (DistilBERT) to get sentiment label and score
- Save final results to `tweets_sentiment_analysis_results.csv`

✔️ **Libraries used:** pandas, nltk, transformers

---

### 3. Spam Email Classification (Zero-shot)

**Objective:** Classify emails as spam or ham using **zero-shot classification**.

**Steps:**

- Load `spam.csv`
- Use Hugging Face **facebook/bart-large-mnli** zero-shot pipeline
- Define candidate labels: spam, ham
- Apply classification function to sample data for testing
- Save final results to `spam_email_classification_results.csv`

✔️ **Libraries used:** pandas, transformers

---

### 4. Chatbot using Streamlit & Transformers

**Objective:** Build a minimal chatbot web app using Streamlit and an LLM (GPT2 demo).

**Steps:**

- Create `app.py` with Streamlit UI and Transformers pipeline
- Install dependencies via `pip`
- Run app locally with:

```bash
streamlit run app.py
