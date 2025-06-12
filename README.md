# DevelopersHub Data Science and Analytics Internship Tasks

This README file contains the four tasks I did at the internship.

## Task 1: Exploring and Visualizing the Iris Dataset

### Objective
Load, summarize, and visualize the Iris dataset to understand its structure and uncover patterns using pandas, matplotlib, and seaborn.

### Approach
- **Data Loading**: Imported the Iris dataset (150 samples, 4 features, 3 species) via seaborn's `load_dataset`.
- **Inspection**: Examined dataset structure (`.shape`, `.columns`, `.head`), checked for missing values, and computed summary statistics (`.describe`, species counts).
- **Visualizations**:
  - Correlation heatmap for feature relationships.
  - Scatter plot of sepal length vs. width by species.
  - Histograms for feature distributions with KDE.
  - Box plots for feature spread and outliers by species.
  - Pair plot for pairwise feature relationships.
- **Tools**: Used pandas for data handling, seaborn and matplotlib for visualizations with `Set2` palette and `whitegrid` style.

### Results and Insights
- **Data Quality**: No missing values; balanced species (50 samples each).
- **Correlations**: Strong correlation between petal length and width (r > 0.9).
- **Patterns**: Setosa is distinct; versicolor and virginica overlap in sepal measurements.
- **Outliers**: Minor outliers in sepal width for virginica.
- **Key Finding**: Petal measurements are more effective for species differentiation than sepal measurements.


## Task 2: Credit Risk Prediction

### Objective
Predict whether a loan applicant is likely to default on a loan.

### Approach
- **Data Loading**: Imported the Loan Prediction Dataset (614 samples, 13 columns) via a public URL.
- **Inspection**: Examined dataset structure (`.shape`, `.columns`, `.head`), handled missing values (median for `LoanAmount`, `Credit_History`, etc.; mode for `Gender`, etc.), and encoded categorical variables.
- **Visualizations**:
  - Histogram for `LoanAmount` distribution.
  - Count plot of `Education` vs. `Loan_Status`.
  - Histogram for `ApplicantIncome` distribution.
  - Scatter plot of `LoanAmount` vs. `ApplicantIncome` by `Loan_Status`.
- **Model Training**: Trained a Logistic Regression model for binary classification.
- **Evaluation**: Assessed model with accuracy and confusion matrix.
- **Tools**: Used pandas, seaborn, matplotlib, and scikit-learn with `Set2` palette and `whitegrid` style.

### Results and Insights
- **Data Quality**: Handled missing values; encoded categorical features like `Gender`, `Education`.
- **EDA**: `LoanAmount` and `ApplicantIncome` are right-skewed; graduates have higher approval rates.
- **Model Performance**: Logistic Regression achieved ~80% accuracy (varies by split).
- **Confusion Matrix**: Better prediction for approvals than non-approvals.
- **Key Finding**: `Credit_History` and `Education` strongly influence loan approval.
