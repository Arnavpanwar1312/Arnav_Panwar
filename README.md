# Exploratory Data Analysis (EDA) Course Project

## Student Information

* **Name:** Arnav Panwar
* **Registration Number:** 23BDS0192
* **Institution:** Vellore Institute of Technology (VIT)

---

# Project Overview

This repository contains the implementation of an **Exploratory Data Analysis (EDA)** project carried out using Python. The project focuses on analyzing the provided medical dataset through systematic preprocessing, statistical analysis, data cleaning, transformation, and visualization techniques.

The objective of this project is to understand the dataset, identify patterns, detect missing values and outliers, and generate meaningful insights using descriptive statistics and graphical representations.

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

* **pandas** – Data manipulation and analysis
* **numpy** – Numerical computations
* **matplotlib.pyplot** – Data visualization
* **seaborn** – Statistical data visualization

---

# Phase 1: Exploratory Data Analysis (EDA)

The objective of this phase is to prepare the raw dataset for analysis and discover important characteristics through statistical summaries and visualizations.

---

## Step 1: Import Required Libraries

Imported all required Python libraries for data manipulation, preprocessing, and visualization.

Libraries used:

* pandas
* numpy
* matplotlib
* seaborn

---

## Step 2: Dataset Loading

* Loaded the dataset (`data.csv`) into a Pandas DataFrame.
* Displayed:

  * First five records
  * Last five records
  * Dataset dimensions
  * Data types
  * Column names

---

## Step 3: Basic Statistical Analysis

Performed descriptive statistical analysis including:

* Summary statistics
* Mean
* Median
* Standard deviation
* Variance
* Correlation matrix for numerical variables

---

## Step 4: Missing Value Analysis

Performed missing value analysis by:

* Counting missing values
* Calculating missing value percentages
* Replacing missing numerical values using the column mean
* Verifying successful imputation

---

## Step 5: Data Cleaning

Performed data cleaning operations including:

* Removal of duplicate records
* Verification of duplicate entries
* Inspection of data types

---

## Step 6: Data Transformation

Applied Min-Max Normalization to all numerical attributes in order to scale values between 0 and 1.

A normalized dataset was created for further analysis.

---

## Step 7: Univariate Analysis

Analyzed individual variables using graphical techniques.

Visualizations include:

* Histogram of Age
* Box Plot of Age
* Density Plot of Age

These plots help understand:

* Distribution
* Central tendency
* Spread
* Presence of outliers

---

## Step 8: Bivariate Analysis

Explored relationships between two variables using:

* Scatter Plot (Age vs Risk)
* Box Plot (Gender vs Age)
* Correlation Heatmap

These visualizations highlight relationships between numerical and categorical variables.

---

## Step 9: Multivariate Analysis

Performed advanced visualization techniques including:

* Pair Plot
* Correlation Heatmap
* Bubble Plot (Age vs Risk with Bleed as bubble size)

These plots help identify multidimensional relationships within the dataset.

---

## Step 10: Conclusion

The Exploratory Data Analysis successfully identified:

* Dataset structure
* Statistical characteristics
* Missing values
* Duplicate records
* Feature distributions
* Relationships among variables
* Correlation between numerical attributes

The dataset was successfully prepared for further machine learning or predictive modeling tasks.

---

# Technologies Used

* Python 3.x
* Jupyter Notebook / Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn

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
11. Generate Insights

---

# Repository Contents

```text
├── data.csv
├── Phase-1_EDA.ipynb
├── README.md
```
