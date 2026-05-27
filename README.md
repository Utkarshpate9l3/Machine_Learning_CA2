# 🚀 RepoRadar — GitHub Repository Intelligence Engine

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge\&logo=jupyter)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-yellow?style=for-the-badge\&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge\&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-EDA-blueviolet?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)

> ### 📊 Machine Learning–based GitHub Repository Analytics & Prediction System

RepoRadar is a machine learning project focused on analyzing GitHub repository metadata and predicting repository health, growth trends, and popularity using multiple supervised learning models.

The project demonstrates complete ML workflows including:

* Data cleaning
* Exploratory Data Analysis (EDA)
* Feature engineering
* Model training
* Performance evaluation
* Feature importance analysis
* Comparative modeling

This repository is designed to showcase practical machine learning implementation skills using real-world repository metadata.

---

# 📖 Project Overview

Modern software repositories generate massive amounts of metadata such as stars, forks, watchers, pull requests, and commit activity. These signals can provide valuable insights into:

* Repository quality
* Community engagement
* Project sustainability
* Growth potential
* Popularity trends

RepoRadar leverages machine learning techniques to analyze repository metadata and build predictive models capable of classifying repositories into different operational and popularity categories.

The project contains **three independent ML notebooks**, each solving a different prediction problem:

| Notebook   | Objective                        | Model                    |
| ---------- | -------------------------------- | ------------------------ |
| Notebook 1 | Repository Health Prediction     | Decision Tree Classifier |
| Notebook 2 | Repository Growth Prediction     | Random Forest Classifier |
| Notebook 3 | Repository Popularity Prediction | Logistic Regression      |

---

# 🎯 Problem Statement

Open-source repositories vary significantly in terms of:

* Activity level
* Community engagement
* Maintenance quality
* Popularity
* Growth momentum

The challenge is to automatically identify and predict these characteristics using repository metadata.

This project aims to answer questions such as:

* Which repositories are healthy and actively maintained?
* Which repositories are growing rapidly?
* Which repositories are likely to become popular?
* Which repository metrics contribute most to growth and popularity?

---

# ✨ Core Features

✅ End-to-end ML workflows
✅ Data preprocessing and cleaning
✅ Missing value handling
✅ Feature engineering
✅ Exploratory Data Analysis (EDA)
✅ Multiple classification models
✅ Feature importance analysis
✅ Model evaluation using multiple metrics
✅ ROC curve analysis (Logistic Regression)
✅ Repository growth categorization
✅ Repository health scoring system
✅ Visual analytics using Seaborn & Matplotlib

---

# 🧠 Machine Learning Objectives

## 1️⃣ Repository Health Prediction

Predict whether a repository is:

* Healthy
* Moderate
* Poor

using repository engagement and maintenance metrics.

---

## 2️⃣ Repository Growth Prediction

Predict whether a repository is:

* Growing
* Stagnant
* Declining

based on repository age and popularity trends.

---

## 3️⃣ Repository Popularity Prediction

Predict whether a repository is:

* Popular
* Not Popular

using GitHub repository engagement metrics.

---

# 🗂 Dataset Information

| Attribute     | Details                        |
| ------------- | ------------------------------ |
| Dataset Type  | GitHub Repository Metadata     |
| File Used     | `repository_data.csv`          |
| Domain        | Open Source / GitHub Analytics |
| Format        | CSV                            |
| Learning Type | Supervised Classification      |

## 📌 Important Features Used

| Feature              | Description                        |
| -------------------- | ---------------------------------- |
| stars                | GitHub stars count                 |
| forks                | Fork count                         |
| watchers             | Repository watchers                |
| contributor_count    | Pull requests / contributors proxy |
| commit_frequency     | Commit activity                    |
| repository_age_days  | Age of repository                  |
| days_since_last_push | Repository inactivity measure      |
| stars_per_day        | Growth efficiency metric           |

---

# 🛠 Data Preprocessing Workflow

The notebooks implement multiple preprocessing techniques:

## ✅ Cleaning Steps

* Duplicate removal
* Column renaming for consistency
* Datetime conversion
* Missing value analysis
* Median-based null value imputation

## ✅ Feature Engineering

### Notebook 1

* `repo_health_score`
* `health_category`
* `days_since_last_push`

### Notebook 2

* `repository_age_days`
* `stars_per_day`
* `growth_label`

### Notebook 3

* `repository_age_days`
* Binary target variable: `popular`

---

# 📊 Exploratory Data Analysis (EDA)

The project performs extensive exploratory analysis using:

* Histograms
* Countplots
* Scatterplots
* Pairplots
* Correlation heatmaps
* Boxplots
* Distribution analysis
* Feature importance plots
* ROC Curve visualization

## 📈 Visualizations Used

| Visualization           | Purpose                             |
| ----------------------- | ----------------------------------- |
| Histograms              | Distribution analysis               |
| Correlation Heatmaps    | Feature relationships               |
| Pairplots               | Multi-feature relationships         |
| Countplots              | Target distribution                 |
| Scatterplots            | Feature interaction analysis        |
| Boxplots                | Outlier and spread analysis         |
| ROC Curve               | Classification threshold evaluation |
| Feature Importance Plot | Model interpretability              |

---

# 🧱 Tech Stack

## 👨‍💻 Programming Language

* Python

## 📚 Libraries & Frameworks

| Category             | Libraries           |
| -------------------- | ------------------- |
| Data Processing      | Pandas, NumPy       |
| Visualization        | Matplotlib, Seaborn |
| Machine Learning     | Scikit-learn        |
| Notebook Environment | Jupyter Notebook    |

---

# 🏗 Project Workflow Architecture

```text
Dataset Loading
       ↓
Data Cleaning
       ↓
Null Handling
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Feature Selection
       ↓
Train/Test Split
       ↓
Model Training
       ↓
Evaluation Metrics
       ↓
Visualization & Insights
```

---

# 📓 Notebook Descriptions

## 📘 Notebook 1 — Repo Health Prediction

### 🎯 Objective

Predict repository health category using a Decision Tree Classifier.

### 🤖 Model Used

* Decision Tree Classifier

### 🧩 Engineered Features

* `repo_health_score`
* `health_category`
* `days_since_last_push`

### 📊 EDA Highlights

* Missing value heatmap
* Stars distribution
* Forks distribution
* Correlation heatmap
* Contributor count boxplot

### 📈 Evaluation Metrics

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 0.9998 |
| Precision | 0.9998 |
| Recall    | 0.9998 |
| F1 Score  | 0.9998 |

### 🔍 Key Insight

Repositories with:

* Higher stars
* More forks
* Frequent commits

are more likely to be categorized as healthy.

---

## 📗 Notebook 2 — Repository Growth Prediction

### 🎯 Objective

Predict repository growth trend using Random Forest Classifier.

### 🤖 Model Used

* Random Forest Classifier

### 🧩 Engineered Features

* `repository_age_days`
* `stars_per_day`
* `growth_label`

### 📊 EDA Highlights

* Growth label countplot
* Pairplot of important features
* Correlation heatmap
* Distribution plots

### 📈 Evaluation Metrics

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 0.9797 |
| Precision | 0.9804 |
| Recall    | 0.9797 |
| F1 Score  | 0.9798 |

### 🔍 Key Insight

Repositories with:

* High stars per day
* Consistent commits
* Strong engagement

are more likely to be classified as growing repositories.

---

## 📙 Notebook 3 — Repository Popularity Prediction

### 🎯 Objective

Predict repository popularity using Logistic Regression.

### 🤖 Model Used

* Logistic Regression

### 🧩 Engineered Features

* `popular`
* `repository_age_days`

### 📊 EDA Highlights

* Stars histogram
* Forks histogram
* Popular vs non-popular distribution
* Correlation heatmap
* ROC curve

### 📈 Evaluation Metrics

| Metric    | Score                               |
| --------- | ----------------------------------- |
| Accuracy  | 0.7446                              |
| Precision | 0.8596                              |
| Recall    | 0.5502                              |
| F1 Score  | 0.6709                              |
| ROC-AUC   | Not explicitly provided in notebook |

### 🔍 Key Insight

Features such as:

* Forks
* Watchers
* Contributor count

show strong linear relationships with repository popularity.

---

# ⚖️ Model Comparison

| Notebook   | Model               | Prediction Type            | Accuracy | Strengths                                   |
| ---------- | ------------------- | -------------------------- | -------- | ------------------------------------------- |
| Notebook 1 | Decision Tree       | Multi-class Classification | 0.9998   | High interpretability                       |
| Notebook 2 | Random Forest       | Multi-class Classification | 0.9797   | Reduced overfitting & better generalization |
| Notebook 3 | Logistic Regression | Binary Classification      | 0.7446   | Fast and interpretable baseline             |

---

# 🏆 Best Performing Model

## 🥇 Decision Tree Classifier (Notebook 1)

### Why it performed best:

* Strong feature separability
* Engineered repository health score
* Structured classification boundaries
* Highly correlated metadata features

### Important Note

Although the Decision Tree achieved extremely high accuracy, Random Forest generally offers:

* Better robustness
* Lower overfitting risk
* Improved generalization

for production-grade systems.

---

# 📐 Evaluation Metrics Used

| Metric                | Purpose                                  |
| --------------------- | ---------------------------------------- |
| Accuracy              | Overall prediction correctness           |
| Precision             | Correct positive predictions             |
| Recall                | Ability to identify true positives       |
| F1 Score              | Precision-recall balance                 |
| Confusion Matrix      | Prediction distribution analysis         |
| Classification Report | Comprehensive performance summary        |
| ROC Curve             | Binary classification threshold analysis |

---

# 📊 Key Findings & Insights

## 🔹 Repository Health

* Stars and forks are strong indicators of repository quality.
* Frequent commits strongly correlate with healthy repositories.
* Long inactivity negatively impacts health classification.

## 🔹 Repository Growth

* Stars per day is an effective growth indicator.
* Older repositories with low engagement often become stagnant.
* Growth classification benefits significantly from engineered features.

## 🔹 Repository Popularity

* Forks and watchers are highly correlated with popularity.
* Logistic Regression works as a strong baseline model.
* Popular repositories typically attract stronger contributor activity.

---

# 🌍 Real-World Applications

This project can be applied in:

* GitHub analytics platforms
* Open-source recommendation systems
* Repository ranking systems
* Developer productivity tools
* Engineering management dashboards
* OSS investment analysis
* Repository health monitoring systems
* Developer portfolio analysis tools

---


# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/RepoRadar-GitHub-Repository-Intelligence-Engine.git
```

## 2️⃣ Navigate to Project Folder

```bash
cd RepoRadar-GitHub-Repository-Intelligence-Engine
```

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 📦 Requirements

```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

# ▶️ Usage Instructions

## Launch Jupyter Notebook

```bash
jupyter notebook
```

Open any notebook and run cells sequentially.

Recommended order:

1. Repository Health Prediction
2. Repository Growth Prediction
3. Repository Popularity Prediction

---

# 📸 Suggested Screenshots / Graphs for README

Add screenshots of:

✅ Correlation heatmaps
✅ Feature importance charts
✅ ROC curve visualization
✅ Pairplot visualization
✅ Stars distribution histogram
✅ Growth label countplot
✅ Confusion matrix results

---


# 🧾 Conclusion

RepoRadar demonstrates a complete machine learning workflow using GitHub repository metadata.

The project successfully:

* Cleans and preprocesses repository data
* Engineers meaningful analytical features
* Trains multiple ML classification models
* Evaluates performance using industry-standard metrics
* Extracts actionable insights from repository behavior

The notebooks collectively showcase:

* Practical ML engineering skills
* Strong EDA capability
* Feature engineering knowledge
* Classification model implementation
* Visualization and analytical thinking

This makes the project highly suitable for:

* ML/Data Science portfolios
* Academic submissions
* Open-source showcases
* Recruiter demonstrations
* GitHub portfolio enhancement

---

# 📜 License

```txt
MIT License
```

---

# 🙌 Acknowledgment

This project uses GitHub repository metadata for educational and machine learning experimentation purposes.
