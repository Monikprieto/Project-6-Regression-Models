# Project-6-Regression-Models
Detecting Fake Banknotes Using Regression Models.

Introduction
This project explores the detection of counterfeit banknotes using Exploratory Data Analysis (EDA), Linear Regression, and Logistic Regression techniques. The goal is to analyze features extracted from images of banknotes and build predictive models that distinguish between genuine and fake bills.

Dataset Description
- **Dataset Name:** `Fake_Bills.csv`
- **Source:** [Kaggle Dataset - Fake Bills](https://www.kaggle.com/datasets/alexandrepetit881234/fake-bills)
- **Attributes:**
  - `diagonal`, `height_left`, `height_right`, `margin_low`, `margin_up`, `length`
  - `is_genuine` (Target: True = genuine, False = fake)
The dataset includes geometrical measurements extracted from banknote images and a binary classification label.

Tools Used
- **Programming Language:** Python
- **Libraries:**
  - `pandas`, `numpy`: data manipulation and numerical operations
  - `matplotlib`, `seaborn`: data visualization
  - `scikit-learn`: model training, preprocessing, and evaluation
  - `statsmodels`: additional regression analysis

Development (Code)
1. Data Loading and Initial Exploration
- Loaded the dataset using `pandas`
- Explored basic statistics and structure with `df.info()` and `df.describe()`
- Checked for missing and duplicate values
 2. Data Visualization (EDA)
- Histograms to understand feature distributions
- Count plot for the target variable
- Correlation matrix and heatmap to identify relationships
3. Preprocessing
- Handled missing values (none detected)
- Converted categorical labels if needed
- Standardized features using `StandardScaler`
 4. Modeling
- **Linear Regression** for educational comparison (used for continuous predictions)
- **Logistic Regression** to classify fake vs. genuine bills
- Split data into training and testing sets
- Evaluated models using:
  - Accuracy
  - Confusion Matrix
  - Classification Report
  - R² and RMSE (for regression insight)

Results and Conclusions
- The **logistic regression model** provided a reliable method for detecting fake banknotes, achieving a good balance between precision and recall.
- **EDA** revealed clear differences in the distribution of features between genuine and fake bills.
- Visualizations enhanced the interpretability of model performance and feature relevance.

Author
Monica Prieto — Data Engineer
