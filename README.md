## Machine Learning Analysis on Environmental Pollution Data

This project focuses on analyzing a global pollution dataset and building machine learning models to classify **pollution severity levels** based on environmental indicators.

The notebook walks through the entire machine learning pipeline including preprocessing, exploratory data analysis, model training, hyperparameter tuning, and model comparison.

---

## Project Workflow

### 1. Data Preprocessing

The dataset was cleaned and prepared using the following techniques:

- Handling missing values using **SimpleImputer**
  - Numerical columns → Median strategy
  - Categorical columns → Most frequent strategy

- Outlier detection and capping using the **Interquartile Range (IQR) method** for features such as:
  - Air Pollution Index
  - Water Pollution Index
  - Soil Pollution Index
  - Industrial Waste
  - CO₂ Emissions
  - Plastic Waste Produced

- Feature scaling using:
  - `StandardScaler`
  - `MinMaxScaler`

---

### 2. Exploratory Data Analysis

Visual analysis was performed using **Matplotlib** and **Seaborn**, including:

- Distribution plots of pollution indices
- Pollution severity distribution
- Feature relationships and trends

---

### 3. Machine Learning Models

Three classification algorithms were implemented and compared:

1. **Multinomial Naive Bayes**
2. **K-Nearest Neighbors (KNN)**
3. **Decision Tree Classifier**

---

### 4. Hyperparameter Tuning

To improve model performance, **GridSearchCV** with 5-fold cross-validation was used.

#### KNN Parameters
- `n_neighbors`
- `weights` (uniform / distance)
- `metric` (euclidean / manhattan)

#### Decision Tree Parameters
- `max_depth`
- `min_samples_split`
- `criterion` (gini / entropy)

---

### 5. Model Evaluation

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

Performance comparison was visualized using **accuracy and F1-score bar charts**.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Outcome

The project demonstrates how different machine learning algorithms perform on environmental pollution data and highlights the importance of preprocessing, hyperparameter tuning, and evaluation when building classification models.
