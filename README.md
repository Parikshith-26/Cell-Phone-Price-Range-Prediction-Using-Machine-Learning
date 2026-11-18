# 📱 Mobile Price Range Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on predicting the price range of mobile phones based on their technical specifications using Machine Learning classification algorithms.

The objective is to help a mobile phone company understand the relationship between mobile specifications and price categories and make data-driven decisions regarding product development, pricing strategy and market segmentation.

The project uses mobile specifications such as RAM, battery power, internal memory, camera resolution, screen dimensions and connectivity features to classify mobile phones into four price categories.

## 🎯 Problem Statement

A new mobile phone company wants to compete with established brands such as Apple and Samsung. However, estimating the appropriate price category for its products is challenging.

This project analyzes mobile phone specifications and builds classification models to predict the price range of a mobile phone.

The target variable, `price_range`, contains four categories:

| Price Range | Category |
|---|---|
| 0 | Low Cost |
| 1 | Medium Cost |
| 2 | High Cost |
| 3 | Very High Cost |

## 📂 Dataset Information

- **Dataset:** Mobile Price Classification
- **Source:** Provided project dataset
- **File:** `datasets_11167_15520_train.csv`
- **Total Records:** 2,000
- **Total Columns:** 21
- **Target Variable:** `price_range`

### Features

| Feature | Description |
|---|---|
| battery_power | Battery capacity in mAh |
| blue | Bluetooth availability |
| clock_speed | Processor clock speed |
| dual_sim | Dual SIM support |
| fc | Front camera megapixels |
| four_g | 4G availability |
| int_memory | Internal memory |
| m_dep | Mobile depth |
| mobile_wt | Mobile weight |
| n_cores | Number of processor cores |
| pc | Primary camera megapixels |
| px_height | Pixel resolution height |
| px_width | Pixel resolution width |
| ram | Random Access Memory |
| sc_h | Screen height |
| sc_w | Screen width |
| talk_time | Battery talk time |
| three_g | 3G availability |
| touch_screen | Touchscreen availability |
| wifi | Wi-Fi availability |
| price_range | Target price category |

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## 🔍 Project Workflow

### 1. Data Loading and Understanding
- Loaded the dataset using Pandas.
- Examined dataset dimensions and data types.
- Generated descriptive statistical summaries.

### 2. Data Quality Assessment
- Checked for missing values.
- Checked for duplicate records.
- Validated binary categorical features.
- Examined target variable distribution.

### 3. Exploratory Data Analysis (EDA)
- Univariate analysis using histograms and boxplots.
- Bivariate analysis using boxplots.
- Multivariate analysis using scatterplots and pairplots.
- Correlation analysis using a heatmap.

### 4. Data Preprocessing
- Separated independent and dependent variables.
- Performed train-test splitting.
- Applied StandardScaler for Logistic Regression and SVM.

### 5. Machine Learning Models

The following classification algorithms were implemented:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. Support Vector Machine (SVM)

### 6. Model Evaluation

Models were evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix
- 5-Fold Cross-Validation

### 7. Feature Importance Analysis

Feature importance was analyzed using:

- Logistic Regression coefficients.
- Random Forest feature importance scores.

This analysis helps identify mobile specifications that contribute to predicting price categories.

## 📊 Model Performance Comparison

### Test Accuracy

| Model | Accuracy |
|---|---:|
| Logistic Regression | 96.5% |
| Decision Tree | 83% |
| Random Forest | 100% |
| SVM | 89.5% |

### 5-Fold Cross-Validation Accuracy

| Model | Average Accuracy |
|---|---:|
| Logistic Regression | 94.63% |
| Decision Tree | 82.88% |
| Random Forest | 86.88% |
| SVM | 85.94% |

**Best Model: Logistic Regression**

Logistic Regression achieved the highest average cross-validation accuracy of 94.63% and a test accuracy of 96.5%.

Although Random Forest achieved 100% test accuracy, its cross-validation performance was lower. Therefore, Logistic Regression was selected as the preferred model based on more consistent evaluation results.

## 💡 Business Applications

This project can help a mobile phone company in the following ways:

1. **Product Development:** Identify specifications associated with different price categories.
2. **Pricing Strategy:** Estimate the likely price category of a planned mobile phone.
3. **Market Segmentation:** Develop products for budget, mid-range, premium and high-end customers.
4. **Competitive Advantage:** Make informed decisions about product specifications and market positioning.
5. **Resource Allocation:** Prioritize important specifications during product planning.

## ⚠️ Challenges Faced

- Understanding relationships between mobile specifications and price categories.
- Evaluating data quality and feature distributions.
- Handling different feature scales.
- Performing multiclass classification.
- Comparing multiple machine learning algorithms.
- Evaluating model generalization using cross-validation.
- Identifying important features influencing predictions.

These challenges were addressed using Exploratory Data Analysis, StandardScaler, multiple classification algorithms, model evaluation metrics and cross-validation.

## 📁 Project Structure

```text
Mobile-Price-Range-Prediction/
│
├── datasets_11167_15520_train.csv
├── Mobile_Price_Range_Prediction.ipynb
└── README.md
```

## 🚀 How to Run the Project

**Step 1: Clone the repository**

```bash
git clone <your-github-repository-url>
```

**Step 2: Navigate to the project folder**

```bash
cd Mobile-Price-Range-Prediction
```

**Step 3: Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5:** Open `Mobile_Price_Range_Prediction.ipynb` and run the notebook cells.

## 📌 Conclusion

This project demonstrates how Machine Learning can be used to predict mobile phone price categories based on technical specifications.

Four classification algorithms were implemented and evaluated. Logistic Regression achieved the best average cross-validation accuracy of 94.63%, making it the preferred model among the evaluated algorithms.

The project highlights how data analysis, predictive modelling and feature importance can support product planning, pricing decisions and business growth.

---

**Project Domain:** Machine Learning | Data Science | Classification

**Developed using:** Python and Scikit-learn
