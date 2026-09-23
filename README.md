# Exploratory Data Analysis (EDA) Course Project

## Student Information

* **Name:** Arnav Panwar
* **Registration Number:** 23BDS0192
* **Institution:** Vellore Institute of Technology (VIT)

---

# Project Overview

This repository contains the implementation of an Exploratory Data Analysis (EDA) project carried out using Python.

The project focuses on analyzing a medical dataset through data preprocessing, cleaning, statistical analysis, transformation, visualization, and clustering techniques.

The main objective is to understand the dataset, identify patterns, handle missing values, study relationships between variables, detect possible outliers, and group similar observations using clustering methods.

---

# Dataset

**Dataset Name:** `data.csv`

The dataset contains patient-related medical information, including demographic details, clinical observations, treatment information, and outcome variables.

Some important attributes include:

* Age
* Gender
* Risk
* Outcome
* SOD
* PEP
* Bleed
* Treatment Status
* Procedure Type
* Surgery Information

---

# Libraries Used

The following Python libraries were used throughout the project:

* **pandas** for data manipulation and analysis
* **numpy** for numerical computations
* **matplotlib** for data visualization
* **seaborn** for statistical visualization
* **scipy** for statistical analysis and clustering
* **scikit-learn** for preprocessing and clustering

---

# Phase 1: Exploratory Data Analysis

The first phase focuses on understanding and preparing the dataset for further analysis.

## Step 1: Import Required Libraries

The required Python libraries were imported for data manipulation, numerical calculations, statistical analysis, and visualization.

The main libraries used are pandas, numpy, matplotlib, and seaborn.

---

## Step 2: Dataset Loading

The dataset `data.csv` was loaded into a Pandas DataFrame.

The following information was examined:

* First five records
* Last five records
* Dataset dimensions
* Data types
* Column names

This provided an initial understanding of the structure and contents of the dataset.

---

## Step 3: Basic Statistical Analysis

Basic descriptive statistics were performed to understand the numerical variables in the dataset.

The analysis included:

* Summary statistics
* Mean
* Median
* Standard deviation
* Variance
* Correlation between numerical variables

---

## Step 4: Missing Value Analysis

Missing values were examined throughout the dataset.

The analysis included:

* Counting missing values
* Calculating missing value percentages
* Replacing missing numerical values using the column mean
* Verifying the results after imputation

This helped prepare the dataset for further analysis.

---

## Step 5: Data Cleaning

Data cleaning was performed to improve the quality of the dataset.

The following operations were carried out:

* Identification and removal of duplicate records
* Verification of duplicate entries
* Inspection of data types

---

## Step 6: Data Transformation

Min-Max Normalization was applied to numerical attributes.

The values were scaled between 0 and 1 to make the numerical features comparable for further analysis.

A normalized dataset was created for subsequent analysis.

---

## Step 7: Univariate Analysis

Individual variables were analyzed using graphical techniques.

The visualizations included:

* Histogram of Age
* Box Plot of Age
* Density Plot of Age

These visualizations were used to understand the distribution, central tendency, spread, and possible outliers in the data.

---

## Step 8: Bivariate Analysis

Relationships between two variables were analyzed using different visualization techniques.

The analysis included:

* Scatter Plot of Age vs Risk
* Box Plot of Gender vs Age
* Correlation Heatmap

These visualizations helped identify relationships between numerical and categorical variables.

---

## Step 9: Multivariate Analysis

Multiple variables were analyzed together using:

* Pair Plot
* Correlation Heatmap
* Bubble Plot of Age vs Risk with Bleed as bubble size

These visualizations helped examine relationships between multiple attributes at the same time.

---

## Step 10: Phase 1 Conclusion

The first phase provided an overall understanding of the dataset.

The analysis covered:

* Dataset structure
* Statistical characteristics
* Missing values
* Duplicate records
* Feature distributions
* Relationships between variables
* Correlations between numerical attributes

The cleaned and transformed dataset was then used for further statistical analysis and clustering.

---

# Phase 2: Statistical Analysis and Clustering

The second phase focuses on detailed statistical analysis, multivariate analysis, and clustering.

The main numerical variables used in this phase are:

* Age
* SOD
* PEP

The main categorical variables considered are:

* Risk
* Outcome

---

## 9. 1D Statistical Analysis

One-dimensional statistical analysis was performed on the numerical variables.

Summary statistics were calculated for Age, SOD, and PEP.

The analysis included:

* Count
* Mean
* Standard deviation
* Minimum
* Quartiles
* Maximum

The Outcome variable was also analyzed using frequency counts.

Pie charts and bar charts were used to visualize the distribution of different outcome categories.

Age was divided into different groups:

* 0–20
* 21–40
* 41–60
* 61–80
* 81–100

A histogram was used to understand the distribution of Age, while a box plot was used to examine its spread and identify possible outliers.

---

## 10. 2D Statistical Analysis

Two-dimensional analysis was performed to study relationships between different variables.

A contingency table was created between Risk and Outcome to examine their relationship.

Age was grouped according to Outcome and descriptive statistics were calculated, including:

* Mean
* Median
* Standard deviation
* Minimum
* Maximum

Box plots and violin plots were used to compare Age distributions across different Outcome categories.

Pearson and Spearman correlation were calculated between Age and SOD.

Pearson correlation was used to study the linear relationship, while Spearman correlation was used to examine the monotonic relationship.

Simple linear regression was also performed between Age and SOD.

The regression analysis provided:

* Slope
* Intercept
* R-squared
* P-value

---

## 11. 3D Statistical Analysis

Three numerical variables were analyzed together:

* Age
* SOD
* PEP

A 3D scatter plot was created to visualize the relationship between these variables.

The plot uses:

* X-axis: Age
* Y-axis: SOD
* Z-axis: PEP

This provides a three-dimensional view of the numerical features.

---

## 12. ND and Multivariate Analysis

Multivariate analysis was performed by considering multiple variables together.

Age was grouped according to Risk and Outcome.

The following group statistics were calculated:

* Mean
* Median
* Standard deviation
* Count

Box plots were used to compare Age across different Risk and Outcome combinations.

A grouped bar chart was also created to compare the average Age across different groups.

The correlation between Age and SOD was calculated separately for each Outcome category.

A correlation heatmap was created for:

* Age
* SOD
* PEP

A pair plot was also generated to visualize pairwise relationships between the numerical variables.

---

## 13. Clustering Preparation

Before applying clustering algorithms, the numerical variables required for clustering were selected.

The variables used were:

* Age
* SOD
* PEP

Rows containing missing values were removed before clustering.

The selected variables were then standardized using StandardScaler.

Standardization puts the variables on a comparable scale and prevents features with larger numerical ranges from dominating the clustering process.

---

## 14. K-Means Clustering

K-Means clustering was applied to group similar observations based on their numerical characteristics.

An initial K-Means model was created using two clusters.

The Elbow Method was then used to study different values of K.

Within-Cluster Sum of Squares was calculated for K values ranging from 1 to 10.

An elbow plot was created to help identify a suitable number of clusters.

A final K-Means model was created using three clusters.

The resulting cluster labels were stored in the `cluster` column of `cluster_data`.

A scatter plot using Age and SOD was created to visualize the resulting clusters.

---

## 15. Hierarchical Clustering

Hierarchical clustering was performed to study the grouping structure of the dataset.

The following linkage methods were analyzed:

* Single linkage
* Complete linkage
* Ward linkage

Dendrograms were generated for each linkage method to visualize how observations were progressively grouped together.

Agglomerative clustering was then performed using:

* Number of clusters: 3
* Linkage method: Ward

The resulting cluster labels were stored in the `hierarchical_cluster` column of `cluster_data`.

---

# Phase 2 Conclusion

The second phase extended the exploratory analysis by applying statistical methods and clustering techniques.

The analysis included:

* 1D statistical analysis
* 2D statistical analysis
* 3D analysis
* Multivariate analysis
* Correlation analysis
* Linear regression
* Data standardization
* K-Means clustering
* Elbow Method
* Hierarchical clustering
* Dendrogram analysis

These techniques helped identify relationships within the dataset and group observations based on their numerical characteristics.

---

# Technologies Used

* Python 3.x
* Jupyter Notebook
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Scikit-learn

---

# Project Workflow

1. Import Libraries
2. Load Dataset
3. Explore Dataset
4. Perform Statistical Analysis
5. Handle Missing Values
6. Clean Data
7. Transform Data
8. Perform Univariate Analysis
9. Perform Bivariate Analysis
10. Perform Multivariate Analysis
11. Perform 1D Statistical Analysis
12. Perform 2D Statistical Analysis
13. Perform 3D Analysis
14. Perform Correlation and Regression Analysis
15. Prepare Data for Clustering
16. Apply K-Means Clustering
17. Apply Hierarchical Clustering
18. Generate Insights

---

# Repository Contents

```text
├── data.csv
├── Phase-1_EDA.ipynb
├── Phase-2_Statistical_Analysis_and_Clustering.ipynb
├── README.md
