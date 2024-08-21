# Describe

This project predicts the minimum and maximum salary ranges for Software Engineers based on features such as company, job title, and location. The project utilizes both a Linear Regression model and a Random Forest Regressor to estimate salary ranges.

# Project Overview
The goal of this project is to predict the salary ranges for Software Engineers. The dataset includes company ratings, job titles, and locations, and the target variables are the minimum and maximum salary values. We use machine learning models to predict these salaries based on categorical and numerical input features.

Two models are trained and evaluated:

- Linear Regression
- Random Forest Regressor

# Dataset

The dataset includes the following columns:

- Company: Name of the company offering the job.
- Company Score: A rating for the company.
- Job Title: The job title.
- Location: The location of the job.
- Min_Salary: The minimum salary for the job.
- Max_Salary: The maximum salary for the job.

# Data Preprocessing
Several preprocessing steps were applied to the dataset:

- Cleaning Salary Data: Removing extra text such as "(Glassdoor est.)" and "(Employer est.)" from the salary column.
- Extracting Salary Ranges: Salary values were split into Min_Salary and Max_Salary using regular expressions.
- Encoding Categorical Variables: Columns like Company, Job Title, and Location were transformed into dummy variables.
- Handling Missing Data: Rows with missing values were removed.
- Outlier Removal: Outliers with salaries below a threshold were removed to improve model performance.

# Results
The models achieved the following results:

- Linear Regression (R²): 67.65%
- Random Forest Regressor (R²): 60.86%

While the Linear Regression model performed slightly better in this case, both models provide reasonable accuracy in predicting the salary ranges based on the input features.

# Technologies Used
- Python: The primary programming language.
- Pandas & NumPy: For data manipulation and preprocessing.
- Scikit-learn: For building and evaluating machine learning models.
- Google Colab: For running the notebook.
