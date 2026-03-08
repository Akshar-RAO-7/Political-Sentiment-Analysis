# Sentiment Analysis for Political Tweets (BJP vs Congress)

A Natural Language Processing (NLP) project that analyzes public sentiment toward major Indian political parties using Twitter data.
This project processes **79,930 tweets** related to election campaigns and applies multiple **machine learning models** to classify sentiment into **positive, negative, and neutral categories**.

The system uses **TF-IDF feature extraction** combined with traditional machine learning classifiers to evaluate public opinion trends during political campaigns.

---

# Project Overview

Social media platforms such as Twitter provide large-scale real-time public opinion data. This project leverages **NLP pipelines and machine learning models** to extract insights from political tweets.

Key objectives:

* Collect and analyze tweets related to **BJP and Congress**
* Preprocess noisy social media text
* Apply **machine learning algorithms for sentiment classification**
* Compare performance across multiple models
* Identify sentiment trends during political campaigns

---

# Dataset

The dataset contains **79,930 tweets** collected from Twitter related to Indian political parties.

## Files

| File                  | Description                                    |
| --------------------- | ---------------------------------------------- |
| `bjp_tweets.csv`      | Tweets related to Bharatiya Janata Party (BJP) |
| `congress_tweets.csv` | Tweets related to Indian National Congress     |

Each dataset contains tweet text along with preprocessing fields used for sentiment analysis.

---

# NLP Pipeline

The project follows a complete **text processing pipeline**:

### 1. Data Cleaning

* Remove URLs
* Remove mentions and hashtags
* Remove punctuation and numbers
* Convert text to lowercase

### 2. Text Normalization

* Tokenization
* Stopword removal
* Stemming / Lemmatization

### 3. Feature Extraction

* **TF-IDF Vectorization**

### 4. Model Training

Multiple machine learning algorithms were trained and evaluated.

---

# Machine Learning Models

The following classifiers were implemented and evaluated:

| Model               | Description                                    |
| ------------------- | ---------------------------------------------- |
| Decision Tree       | Tree-based classifier for sentiment prediction |
| Logistic Regression | Linear classification model                    |
| Linear SVC          | Support Vector Machine for text classification |
| Naive Bayes         | Probabilistic classifier widely used for NLP   |
| XGBoost             | Gradient boosting ensemble model               |

### Best Performing Model

| Model         | Accuracy  |
| ------------- | --------- |
| Decision Tree | **93.4%** |

---

# Project Structure

```text
Political-Sentiment-Analysis/
│
├── Data/
│   ├── bjp_tweets.csv
│   └── congress_tweets.csv
│
├── Notebooks/
│   ├── sentiment_analysis.ipynb
│   └── Project.ipynb
│
├── Documentation/
│   ├── FINAL_RESEARCHPAPER-SENTIMENT ANALYSIS.pdf
│   ├── report on Sentiment analysis.pdf
│   └── README.md
│
└── project.zip
```

---

# Installation

Clone the repository:

```
git clone https://github.com/Akshar-RAO-7/Political-Sentiment-Analysis.git
```

Navigate to the project folder:

```
cd Political-Sentiment-Analysis
```

Create a virtual environment:

```
python -m venv .venv
```

Activate the environment:

Windows

```
.venv\Scripts\activate
```

macOS / Linux

```
source .venv/bin/activate
```

Install required dependencies:

```
pip install pandas numpy scikit-learn nltk matplotlib seaborn
```

---

# Usage

1. Launch Jupyter Notebook or open the project in VS Code.
2. Open the notebook:

```
sentiment_analysis.ipynb
```

3. Run all cells sequentially to:

   * Load the datasets
   * Preprocess tweets
   * Train machine learning models
   * Evaluate sentiment classification performance

---

# Results and Insights

Key observations from the analysis:

* Decision Tree classifier achieved the **highest accuracy of 93.4%** using TF-IDF features.
* Sentiment distribution revealed varying public opinion patterns across political campaigns.
* Machine learning models effectively classified sentiment from short social media text.

---

# Applications

This system can be used for:

* Political campaign analysis
* Public opinion mining
* Social media monitoring
* Election trend prediction
* Policy feedback analysis

---

# Technologies Used

Python
Pandas
NumPy
Scikit-learn
NLTK
Matplotlib
Seaborn
Jupyter Notebook

---

# Future Improvements

* Deep learning models (LSTM / BERT)
* Real-time Twitter API streaming
* Topic modeling for issue-based sentiment
* Interactive dashboard for sentiment visualization

---

# Author

Akshar Rao
B.E. Computer Science (AI/ML)
Chandigarh University
UID: 22BAI71302

---

# License

This project is licensed under the MIT License.
