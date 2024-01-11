# studentsandfooddataset
Deriving insights on the impact of food on GPA, sporting activities, and other social indicators of academic performance, healthy wellbeing and physical activity.
The preliminary analysis reveals several points:

Missing Values: There are missing values in various columns. For instance, 'calories_day' and 'type_sports' have 19 and 21 missing values, respectively. This needs to be addressed.

Data Types and Values: Some columns like 'GPA' and 'weight' have unique and possibly inconsistent formats, which may require cleaning or standardization. Also, there are categorical columns with a wide variety of responses (e.g., 'comfort_food').

Numerical Summaries: Certain columns like 'calories_chicken', 'tortilla_calories', and 'waffle_calories' are numerical and could be explored for distribution and correlation analyses.

Given these observations, the next steps include:

Cleaning and standardizing the data, especially for key columns like 'GPA' and 'weight'.
Handling missing values, either by imputation or by removing rows/columns, depending on the context.
Exploring correlations, especially between dietary habits and GPA, gender differences, etc.
Analyzing categorical data like food preferences to identify common trends.
I'll begin by cleaning and standardizing key columns, and then move on to more detailed analysis. Let's start with the 'GPA' and 'weight' columns, as they seem to have some inconsistencies. ​​

The 'GPA' and 'weight' columns have been cleaned and standardized:

GPA: After converting to numeric values, we now have 120 non-null entries. The mean GPA is approximately 3.42, with a standard deviation of 0.39.

Weight: Numeric values were extracted from the 'weight' column, resulting in 122 non-null entries. The mean weight is around 159 pounds, with a standard deviation of 32.38 pounds.

Next, I will address the missing values in the dataset. Given the context, we might either impute these values or drop the rows/columns, depending on the extent of missing data and its potential impact on analysis. After handling missing values, I'll proceed with exploratory data analysis to uncover trends and correlations in the dataset. Let's handle the missing values first. ​​

All missing values in the dataset have been addressed. Columns with a high percentage of missing values were dropped, and the remaining missing values in other columns were imputed with the median for numerical data and the mode for categorical data. The dataset now has no missing values.

Next, I'll conduct exploratory data analysis (EDA). This will include examining distributions of key variables, exploring potential correlations (such as between dietary habits and GPA), and identifying any notable patterns or trends in the data. Let's start the EDA process.
The exploratory data analysis reveals several insights:

GPA Distribution: The GPA values are somewhat normally distributed, centering around the 3.0 to 3.8 range. This suggests that most students have above-average GPAs.

Weight Distribution: The distribution of weight shows a wide range, with a concentration between 100 to 180 pounds.

Relationship between GPA and Weight: The scatterplot does not indicate a strong or obvious relationship between GPA and weight. The data points are quite dispersed, suggesting that if there is a relationship, it is not linear or is influenced by other factors.

Correlation Heatmap: This heatmap of numerical variables provides a visual representation of correlations between different variables. Higher absolute values indicate stronger relationships, whether positive (closer to 1) or negative (closer to -1). Most variables show low correlation with each other, indicating that they are relatively independent.

