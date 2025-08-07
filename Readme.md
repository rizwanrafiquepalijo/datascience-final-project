Documentation for Peer-Graded Assignment on Boston Housing Dataset Analysis

 Overview
This Jupyter notebook analyzes the Boston Housing Dataset, which contains information about housing values in suburbs of Boston. The analysis includes data exploration, visualization, and statistical tests to understand relationships between various housing features.

## Dataset Description
The Boston Housing Dataset contains the following variables:
- CRIM: Per capita crime rate by town
- ZN: Proportion of residential land zoned for lots over 25,000 sq.ft.
- INDUS: Proportion of non-retail business acres per town
- CHAS: Charles River dummy variable (1 if tract bounds river; 0 otherwise)
- NOX: Nitric oxides concentration (parts per 10 million)
- RM: Average number of rooms per dwelling
- AGE: Proportion of owner-occupied units built prior to 1940
- DIS: Weighted distances to five Boston employment centers
- RAD: Index of accessibility to radial highways
- TAX: Full-value property-tax rate per $10,000
- PTRATIO: Pupil-teacher ratio by town
- LSTAT: % lower status of the population
- MEDV: Median value of owner-occupied homes in $1000's

Analysis Tasks Performed

1. Data Loading and Initial Exploration
- Imported necessary libraries (pandas, seaborn, matplotlib, scipy.stats, statsmodels)
- Loaded the Boston Housing dataset from a CSV file
- Displayed the first few rows of the dataset to understand its structure

2. Visualization Tasks

a. Boxplot of MEDV (Median Home Value)
- Created a boxplot to visualize the distribution of median home values
- The plot shows median, quartiles, and potential outliers in the housing prices

b. Bar Plot of CHAS (Charles River) vs. MEDV
- Visualized the relationship between proximity to the Charles River and median home values
- The plot compares average home values for properties near vs. not near the river

c. Boxplot of MEDV vs. AGE Groups
- Discretized the AGE variable into three categories:
  - 35 years and younger
  - Between 35 and 70 years
  - 70 years and older
- Created a boxplot to examine how home values vary by the age of the housing stock

3. Statistical Tests

a. T-test for MEDV near vs. not near Charles River
- Performed an independent t-test to determine if there's a statistically significant difference in median home values between properties near the Charles River and those not near it

b. ANOVA for MEDV across AGE groups
- Conducted a one-way ANOVA test to determine if there are statistically significant differences in median home values among the three age categories of housing

c. Correlation Analysis
- Calculated Pearson correlation coefficients between MEDV and other variables
- Identified which features have the strongest relationships with home values

Key Findings
1. Properties near the Charles River tend to have higher median values than those not near the river (statistically significant difference).
2. Newer properties (35 years and younger) generally have higher values than older properties.
3. The number of rooms (RM) and percentage of lower status population (LSTAT) show the strongest correlations with home values.

 How to Use This Notebook
1. Run all cells sequentially to perform the complete analysis
2. The visualizations can be modified by adjusting parameters in the plotting functions
3. Additional statistical tests can be added by following the existing patterns

Dependencies
- Python 3.x
- Jupyter Notebook
- Required libraries:
  - pandas
  - seaborn
  - matplotlib
  - scipy
  - statsmodels

Author
Rizwan Rafique
License
This project is open-source and available for educational purposes.
