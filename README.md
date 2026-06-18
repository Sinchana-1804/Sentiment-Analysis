# Sentiment Analysis for Customer Reviews

## Overview

This project performs **Sentiment Analysis** on customer reviews using **Natural Language Processing (NLP)** and **Machine Learning** techniques. The model classifies reviews as **Positive** or **Negative** based on their textual content, helping businesses understand customer opinions and improve products or services.

The project includes data preprocessing, text cleaning, feature extraction, model training, evaluation, and visualization of sentiment trends.

---

## Objectives

* Analyze customer reviews and identify sentiment polarity.
* Build a machine learning model for sentiment classification.
* Visualize customer sentiment distribution and common review terms.
* Generate actionable insights from customer feedback.

---

## Dataset

The dataset consists of customer product reviews containing:

* **Text** – Review content
* **Score** – Rating provided by the customer

### Sentiment Mapping

| Score | Sentiment         |
| ----- | ----------------- |
| 1, 2  | Negative (0)      |
| 4, 5  | Positive (1)      |
| 3     | Removed (Neutral) |

To prevent model bias, the dataset was balanced by sampling an equal number of positive and negative reviews.

---

## Technologies Used

* Python
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* WordCloud
* Joblib
* Jupyter Notebook

---

## Project Workflow

### 1. Data Preprocessing

* Loaded and filtered review data.
* Removed neutral reviews.
* Converted ratings into sentiment labels.
* Balanced positive and negative classes.
* Performed text cleaning:

  * Lowercase conversion
  * Punctuation removal
  * Stopword removal

### 2. Feature Engineering

* Applied **Count Vectorization** to convert text into numerical features.
* Generated a document-term matrix for machine learning.

### 3. Model Training

Implemented the **Multinomial Naive Bayes** classifier:

* Split dataset into training and testing sets.
* Trained the model on processed review data.
* Generated sentiment predictions on unseen reviews.

### 4. Model Evaluation

Evaluation metrics used:

* Accuracy Score
* Confusion Matrix

**Model Accuracy:** **88%**

---

## Visualizations

The project generates:

### Sentiment Distribution

* Positive vs Negative review count comparison.

### Confusion Matrix

* Visualization of classification performance.

### Word Clouds

* Frequently occurring words in positive reviews.
* Frequently occurring words in negative reviews.

### Sample Predictions

* Displays customer reviews alongside their predicted sentiment labels.

---

## Key Features

* Automated text preprocessing pipeline.
* Balanced dataset handling.
* Count Vectorizer-based feature extraction.
* Multinomial Naive Bayes classification.
* Sentiment visualization using charts and word clouds.
* Sample review sentiment prediction display.

---

## Results

| Metric              | Value                               |
| ------------------- | ----------------------------------- |
| Model               | Multinomial Naive Bayes             |
| Accuracy            | 88%                                 |
| Classification Type | Binary Sentiment Classification     |
| Dataset Balance     | Equal Positive and Negative Samples |

---

## Project Structure

```text
Sentiment-Analysis/
│
├── Reviews.csv
├── sentiment_analysis.ipynb
├── README.md
│
├── outputs/
│   ├── confusion_matrix.png
│   ├── sentiment_distribution.png
│   ├── positive_wordcloud.png
│   └── negative_wordcloud.png
│
└── models/
    └── sentiment_model.pkl
```

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Sentiment-Analysis.git
```

### 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn nltk wordcloud scikit-learn joblib tabulate
```

### 3. Run the Notebook

Open Jupyter Notebook and execute all cells:

```bash
jupyter notebook
```

---

## Future Enhancements

* Experiment with TF-IDF vectorization.
* Implement advanced NLP models.
* Deploy as a Streamlit web application.
* Add multiclass sentiment classification.
* Compare multiple machine learning algorithms for improved performance.

---

## Conclusion

This project demonstrates the application of Natural Language Processing and Machine Learning to automatically classify customer reviews into positive and negative sentiments. The developed solution achieves strong performance while providing meaningful visual insights into customer feedback, making it useful for business intelligence and customer experience analysis.
