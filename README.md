📊 DeepFlow Data Analysis Notebooks
This repository contains two Jupyter notebooks focused on structured data preprocessing and exploratory analysis. Each notebook targets a different dataset, applying essential steps to prepare the data for machine learning or derive valuable insights.

📁 Notebook Summaries
🔹 A1.ipynb — Auction Sales Data: Preprocessing & Encoding
Objective:
Clean and encode a machinery auction sales dataset using standard preprocessing techniques to prepare it for predictive modeling.

Main Tasks Covered:

Load training and test CSV files using pandas.

Parse the saledate column and sort the data chronologically.

Eliminate columns with over 30% missing data.

Drop identifier and date-related fields (SalesID, MachineID, ModelID, saledate) that are not useful for modeling.

Apply median imputation to handle missing numeric values.

Use LabelEncoder from sklearn.preprocessing to encode categorical features.

Outcome:
A cleaned and encoded version of both training and test sets, suitable for use in machine learning models.

🔹 A2.ipynb — Zomato Dataset: Exploratory Analysis
Objective:
Conduct an initial exploration of a restaurant dataset to understand its structure and prepare for further analysis or visualization.

Main Tasks Covered:

Load the zomato.csv dataset (commonly exported from Excel).

Display the first few rows using .head() to get a quick overview.

Summarize the structure of the dataset using .info() and .describe().

Print all column names to understand available features.

Outcome:
A structured overview of the dataset with basic statistical summaries and feature listings, laying the groundwork for deeper analysis.

