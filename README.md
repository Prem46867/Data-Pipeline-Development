# Data-Pipeline-Development 

Company Name:  CodeTech It Solutions

Name : Prem M 

Domain : Data Science

Duration : 4 Weeks

Intern ID : CTIS6711

Desprition of the task:

This Python script demonstrates a structured approach to data preprocessing using powerful libraries like pandas and scikit-learn. The primary objective of the code is to clean and standardize a dataset so that it becomes suitable for further analysis or machine learning tasks.

The process begins by importing the required modules. Pandas is used for data manipulation and handling tabular datasets, while components from scikit-learn are used to build a preprocessing pipeline. The dataset is loaded from a CSV file named "student_data.csv" using the read_csv() function. This file is expected to contain various features related to students, possibly including both numeric and non-numeric data. After loading, the script prints the original dataset, allowing the user to inspect its structure and identify missing values or inconsistencies.

Next, the script focuses specifically on numeric data by selecting columns with data types int64 and float64. This step is crucial because many preprocessing techniques, such as scaling and imputation, are applicable only to numerical features. By isolating numeric columns, the script avoids errors and ensures that transformations are applied appropriately.

A key feature of this script is the use of a pipeline. A pipeline is a sequence of data processing steps applied in a fixed order, making the workflow more organized and reproducible. In this case, the pipeline consists of two steps: imputation and scaling. The SimpleImputer is used to handle missing values by replacing them with the mean of the respective column. This ensures that no null values remain, which could otherwise cause issues in machine learning algorithms. Following imputation, the StandardScaler standardizes the data by transforming it so that each feature has a mean of zero and a standard deviation of one. This is particularly important for algorithms that are sensitive to the scale of input features.

Once the pipeline is defined, it is applied to the numeric data using the fit_transform() method. This method first learns the necessary parameters (such as column means) and then transforms the data accordingly. The resulting processed data is stored in a new variable and then converted back into a pandas DataFrame. Column names are preserved to maintain clarity and consistency.

Finally, the cleaned and scaled dataset is saved to a new CSV file called "prepared_data.csv". This allows the processed data to be reused in future tasks without repeating the preprocessing steps. A completion message is printed to indicate that the pipeline has executed successfully.

Overall, this script provides a clean and efficient example of how to preprocess data using a pipeline approach. It ensures that missing values are handled, features are standardized, and the workflow remains modular and easy to maintain.

output of the task :

<img width="866" height="482" alt="Image" src="https://github.com/user-attachments/assets/3ae5c3ea-8e17-4484-b0ce-df47cbb25550" />
