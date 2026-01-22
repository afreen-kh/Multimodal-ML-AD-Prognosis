# Data Preprocessing

Data preprocessing constitutes a critical component of the proposed pipeline. Raw neuroimaging-derived and clinical data often contain missing values, outliers, and scale inconsistencies that can adversely affect machine learning performance.

In this study, missing values were handled using median imputation, which is robust to outliers and preserves the central tendency of continuous variables. Outlier detection was performed through exploratory statistical analysis to assess data dispersion and variability.

Continuous features were standardized to ensure uniform scaling across attributes, thereby improving model convergence and stability. Categorical variables were encoded appropriately prior to model training.

Preprocessing decisions were guided by both statistical reasoning and clinical interpretability to maintain alignment with real-world diagnostic settings.
