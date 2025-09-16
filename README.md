# 🎬 Movie Dataset NLP Preprocessing

This project demonstrates **Natural Language Processing (NLP) preprocessing** techniques on a Movies dataset (from The Movie Database API).  
The goal is to clean and prepare text data (movie overviews, genres, etc.) for further NLP tasks like classification, clustering, or sentiment analysis.  

---

## 📌 Steps Performed

### 1. Data Collection
- Used **TMDb API** to fetch top-rated movies.
- Extracted fields: `title`, `overview`, `genre_ids`.
- Mapped `genre_ids` → `genre names` using the TMDb genre API.

### 2. Data Cleaning
- Converted text to lowercase.  
- Removed HTML tags, URLs, and unnecessary characters.  
- Removed punctuation.  
- Normalized chat words & slang (e.g., *asap → as soon as possible*, *gn → good night*).  
- Corrected spelling mistakes using **pyspellchecker** (faster alternative to TextBlob).

### 3. Text Preprocessing
- Removed stopwords using **NLTK stopwords**.  
- Tokenized text using **NLTK word_tokenize**.  
- Applied **lemmatization** (WordNet Lemmatizer) to get root forms of words.  
- Final dataset includes cleaned tokens and lemmas.

---

## 🛠️ Tools & Libraries Used
- **Python 3**  
- **pandas** (data handling)  
- **requests** (API calls)  
- **nltk** (stopwords, tokenization, lemmatization)  
- **pyspellchecker** (spelling correction)  

---
