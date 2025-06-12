DevelopersHub Data Science and Analytics Intership Tasks
This README file contains the four tasks i did at the internship. 
Task 1: Exploring and Visualizing the Iris Dataset
Objective
Load, summarize, and visualize the Iris dataset to understand its structure and uncover patterns using pandas, matplotlib, and seaborn.
Approach

Data Loading: Imported the Iris dataset (150 samples, 4 features, 3 species) via seaborn's load_dataset.
Inspection: Examined dataset structure (.shape, .columns, .head), checked for missing values, and computed summary statistics (.describe, species counts).
Visualizations:
Correlation heatmap for feature relationships.
Scatter plot of sepal length vs. width by species.
Histograms for feature distributions with KDE.
Box plots for feature spread and outliers by species.
Pair plot for pairwise feature relationships.


Tools: Used pandas for data handling, seaborn and matplotlib for visualizations with Set2 palette and whitegrid style.

Results and Insights

Data Quality: No missing values; balanced species (50 samples each).
Correlations: Strong correlation between petal length and width (r > 0.9).
Patterns: Setosa is distinct; versicolor and virginica overlap in sepal measurements.
Outliers: Minor outliers in sepal width for virginica.
Key Finding: Petal measurements are more effective for species differentiation than sepal measurements.
