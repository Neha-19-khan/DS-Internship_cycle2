#  Task 2: Text Summarization – Data Science Internship

##  Objective

Create a text summarization system that can generate concise summaries from long articles using both extractive and abstractive NLP techniques.

---

##  Dataset

- **Name**: CNN/DailyMail Dataset
- **Source**: Hugging Face `ccdv/cnn_dailymail`
- **Version**: 3.0.0 (non-anonymized)
- **Fields**: `article` (full news) and `highlights` (summary)
 Due to size, we used:
```python
dataset = load_dataset("ccdv/cnn_dailymail", "3.0.0", split="test[:10]", trust_remote_code=True)

---

##  Techniques Used

###  Extractive Summarization
- Used `spaCy` to extract top 3 important sentences
- Based on word frequency and sentence scoring

###  Abstractive Summarization
- Used `facebook/bart-large-cnn` via Hugging Face `transformers`
- Generates fluent, paraphrased summaries

---

## 🔍 Sample Output

**Original:** Long news article (500+ words)  
**Extractive Summary:** Top 3 ranked sentences from original  
**Abstractive Summary:** Short rephrased version using BART  
**Reference Summary:** Human-written highlights from dataset

---

## Insights

- Extractive summary gives quick factual information.
- Abstractive summary feels more natural and human-like.
- BART model performs well without fine-tuning.
- Reference summary quality is close to BART output.

---

##  Libraries Used

- `datasets`, `transformers`, `spaCy`, `nltk`, `rouge-score`
- Python 3.12
- Jupyter Notebook

---
