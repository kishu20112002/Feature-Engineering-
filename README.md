# Feature-Engineering-
🧩 Feature Engineering — My Notes  Feature Engineering is the process of transforming raw data into meaningful features that improve the performance of machine learning models. It is one of the most important steps in any data science workflow. Below are my personal notes on different Feature Engineering techniques:
🔹 1. Handling Missing Values

Identify which columns have missing or null values.

Fill missing values using:

Mean / Median → for numerical data

Mode (Most Frequent) → for categorical data

Constant values (e.g., “Unknown”, 0) if needed

Tools used: SimpleImputer() from sklearn, pandas fillna().

🔹 2. Encoding Categorical Variables

To use categorical data in ML models, convert them into numbers:

Label Encoding → assigns numbers to categories

One-Hot Encoding → creates binary columns for each category

Ordinal Encoding → when categories have order (e.g., Low < Medium < High)
🔹 3. Feature Transformation

To make numerical features more useful:

Scaling → StandardScaler, MinMaxScaler

Log Transformation → reduce skewness

Normalization → brings all values to same range

🔹 4. Creating New Features (Feature Creation)

Generate new useful features from existing ones:

Combine columns

Extract date parts (year, month, day)

Create bins or categories

Calculate ratios, differences, or aggregates

Example:
bmi = weight / (height^2)

🔹 5. Outlier Detection & Treatment

Outliers affect model performance.
Common methods:

IQR Method

Z-Score

Visual detection using boxplots, scatterplots

🔹 6. Feature Selection

Remove unnecessary or irrelevant features:

Correlation analysis

Variance Threshold

Mutual Information

Model-based selection (Random Forest importance, etc.)

🔹 7. Data Type Correction

Ensuring correct data types:

Convert strings to datetime

Convert floats to integers

Ensure categorical data has proper dtype

🔹 8. Final Prepared Dataset

After feature engineering:

Data becomes clean

More meaningful for EDA

Better for machine learning algorithms

Helps improve model accuracy and performance
