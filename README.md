# Fetal-Health-Classification
CTG-Based Predictive Modeling Using Machine Learning

This project uses Cardiotocography (CTG) data to predict fetal health conditions using supervised learning models. CTG is a widely used prenatal test that measures the fetal heart rate and uterine contractions. The goal is to detect risks early and reduce fetal or maternal complications by automating the classification of fetal health status into Normal, Suspect, or Pathological categories.

# data and codes
fetal-health-classification.ipynb    # Main analysis and model notebook
fetal_health.csv                     # Dataset (if included locally)
# How run
Load and preprocess fetal CTG data

Explore and visualize the data

Train multiple classification models

Evaluate model performance using precision, recall, F1-score

Recommend the best-performing model for real-world application



# Tools & Libraries Used
| Tool                                    | Role                          |
| --------------------------------------- | ----------------------------- |
| `NumPy`, `Pandas`                       | Data handling                 |
| `Matplotlib`, `Seaborn`                 | Visualization                 |
| `Scikit-learn`                          | ML model training and metrics |
| `XGBoost`, `RandomForest`, `KNN`, `SVM` | Classifiers tested            |

# Dataset Description
Source: UCI Machine Learning Repository
Records: 2,126 CTG exam results
Classes:

1 = Normal

2 = Suspect

3 = Pathological

Features: 21 physiological measurements, including:

FHR baseline, accelerations, decelerations

Uterine contractions

Histogram-based indicators (mean, median, variance)

Short and long-term variability patterns

Target: fetal_health (1–3 class label)


# Workflow Overview
Import Libraries

Load Dataset

EDA & Preprocessing

Check for missing values

Encode categorical values (if needed)

Normalize/scale features

Model Building

Train/test split

Train different models (e.g., Random Forest, KNN)

Evaluation

Classification report

Confusion matrix

Accuracy/F1-score comparison
# Sample Results

| Model         | Accuracy | F1 Score |
| ------------- | -------- | -------- |
| Random Forest | 94.2%    | 0.94     |
| KNN           | 90.1%    | 0.90     |
| XGBoost       | 95.1%    | 0.95     |

# Key Insights
Most fetal conditions in the dataset are normal; hence class imbalance handling is important.

Ensemble models like Random Forest and XGBoost outperform linear models due to non-linear relationships in physiological features.

Histogram-based features contributed significantly to classification accuracy.

Acknowledgments
Dataset courtesy of the UCI ML Repository

Visuals and styling inspired by the medical domain


