# breast-cancer-recurrence-statistical-analysis
<br>Project Title:
<br>**Exploring Clinical Factors Impacting Breast Cancer Recurrence: A Statistical Analysis**

In this project, I perform a statistical analysis to explore the impact of clinical characteristics on breast cancer recurrence. The analysis was performed in R using RStudio.

Methodology and Brief Explanation of the Results:
<br>
<br>**1. Data Preprocessing and Visualization**
<br>: Click for [Source Code](https://github.com/shamita98/breast-cancer-recurrence-statistical-analysis/blob/f657dba4ae63eec52198a8129faf1836683ee890/Breast%20Cancer%20Data%20Preparation%20and%20Visualization%20in%20R.pdf))
<br>The dataset for this project was obtained from [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/14/breast+cancer).
There are nine predictor variables describing the clinical characteristics of 286 breast cancer patients. The outcome/class variable is breast cancer recurrence.
The patient cohort comprises 201 patients without recurrence and 85 patients with recurrence. Nine data points were excluded due to missing values, resulting in a dataset containing 277 data points in total. The distribution of the outcome variable against each of the predictor variable was visualized through stacked bar plots which revealed a class imbalance among categories within a variable. It was evident that the "no-recurrence" class had a higher percentage compared to "recurrence" class. This imbalance could potentially impact the performance of machine learning models or statistical analyses, as the model may be biased towards the majority class. Further investigation into addressing this class imbalance may be necessary to ensure robust and accurate results.

<br>**2. Fisher's Exact Test**
<br>Fisher's exact test was performed to assess the relationship between categorical predictor and outcome variables. Although this study had bigger contingency tables than the required dimension for Fisher's exact test, it was employed as some cells had frequencies less than five. To improve the statistical inference and computational feasibility, the test was performed with Monte Carlo simulations. The statistical analysis revealed that, based on a significance threshold of p < 0.05, five out of the nine variables  were found to have a significant association with the outcome variable. These findings provide valuable insights into the factors influencing the outcome variable and highlight potential areas for further investigation.

<br>**3. Multivariable Logistic Regression**
<br>
