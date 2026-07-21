# 🐞 Log-Based Bug Pattern Mining

A machine learning project that analyzes software log data and predicts bug patterns using **Natural Language Processing (NLP)** and **Logistic Regression**. The project converts log messages into numerical features using **TF-IDF** and classifies them into different bug categories.

---

## 📌 Project Overview

Software systems generate thousands of log entries during execution. Manually identifying bug patterns from these logs is time-consuming and error-prone.

This project automates the process by:
- Cleaning and preprocessing log data
- Converting textual logs into numerical features using TF-IDF
- Training a machine learning model
- Predicting bug categories from unseen logs

---

## 🎯 Objectives

- Analyze software log files
- Preprocess textual log data
- Extract meaningful features using TF-IDF
- Train a classification model
- Evaluate prediction performance
- Automate bug pattern identification

---

## 📂 Dataset

The dataset contains software log records with information such as:

- Log Message
- Stack Trace
- Bug Type (Target Variable)
- Other log-related attributes

**Dataset Size**
- **12,500 records**
- **9 columns**

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TF-IDF Vectorizer
- Logistic Regression
- Jupyter Notebook

---

## 📚 Libraries Used

```python
numpy
pandas
scikit-learn
```

Main modules:

- TfidfVectorizer
- train_test_split
- LogisticRegression
- classification_report
- confusion_matrix
- Pipeline

---

## 🔄 Project Workflow

```text
Dataset
   │
   ▼
Load Data
   │
   ▼
Data Cleaning
   │
   ▼
Handle Missing Values
   │
   ▼
Text Preprocessing
   │
   ▼
TF-IDF Feature Extraction
   │
   ▼
Train-Test Split
   │
   ▼
Logistic Regression Model
   │
   ▼
Prediction
   │
   ▼
Performance Evaluation
```

---

## ⚙️ Methodology

### 1. Data Loading

- Import dataset using Pandas
- Explore dataset shape and information

### 2. Data Cleaning

- Identify missing values
- Replace null values in the **stack_trace** column
- Prepare clean textual data

### 3. Feature Engineering

The project uses **TF-IDF (Term Frequency–Inverse Document Frequency)** to convert log messages into numerical vectors.

Benefits:
- Removes common words
- Highlights important terms
- Reduces dimensionality using top features

Parameters used:

- max_features = 5000
- stop_words = "english"

---

### 4. Train-Test Split

Dataset is divided into:

- **70% Training**
- **30% Testing**

Using:

```python
train_test_split()
```

---

### 5. Model Training

Model Used:

**Logistic Regression**

Configuration:

- Balanced class weights
- Liblinear solver

---

### 6. Model Evaluation

Performance is measured using:

- Classification Report
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📊 Machine Learning Pipeline

```text
Raw Logs
     │
     ▼
Cleaning
     │
     ▼
TF-IDF Vectorization
     │
     ▼
Feature Matrix
     │
     ▼
Logistic Regression
     │
     ▼
Bug Prediction
```

---

## 📁 Project Structure

```
Log-Based-Bug-Pattern-Mining/
│
├── SE_CIPAT.ipynb
├── synthetic_log_dataset.xls
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/log-based-bug-pattern-mining.git
```

### 2. Navigate

```bash
cd log-based-bug-pattern-mining
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Notebook

```bash
jupyter notebook
```

Open:

```
SE_CIPAT.ipynb
```

Run all cells sequentially.

---

## 📈 Output

The notebook provides:

- Dataset analysis
- Missing value handling
- TF-IDF feature generation
- Logistic Regression model training
- Bug prediction
- Classification report
- Confusion matrix

---

## 🚀 Future Improvements

- Use advanced NLP techniques (Word2Vec, BERT)
- Try Random Forest, XGBoost, and SVM
- Hyperparameter tuning
- Deploy as a web application
- Real-time log monitoring
- Support multiple log formats

---

## 👨‍💻 Author

**Charmmy Lalwani**

Computer Engineering Student

---

## 📄 License

This project is intended for educational and research purposes.
