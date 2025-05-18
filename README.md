# PandasPracticesWorkBook
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
First program 
📊 Casualty Data Analysis (1947–2024)
This project analyzes a dataset of casualties over time, filtering for the years between 1947 and 2024, and visualizing trends in the number of casualties per year. The analysis includes data preprocessing, aggregation, and visualizations using Python's data science stack: Pandas, Seaborn, Matplotlib, and NumPy.

📁 Project Overview
Input dataset: kkk.csv(dataset Between_1947_2024. from dataflow)

Output dataset: dataset Between_1947_2024.csv

Libraries used:

pandas

seaborn

matplotlib

numpy

📌 What the Code Does
Data Import

Reads a CSV file named kkk.csv into a Pandas DataFrame.

Data Filtering

Filters the records to include only those with a Year between 1947 and 2024.

Data Aggregation

Groups the filtered data by Year and Cause.

Counts the number of occurrences for each combination.

Sorts the grouped data by the count in descending order.

Further Filtering

Keeps records between 1947 and 2025 (note: there’s a small redundancy here, since the earlier filter stops at 2024 — could be cleaned up).

Casualty Trend Analysis

Aggregates total casualties per year.

Creates two visualizations:

📈 Line plot showing trends over the years.

📊 Bar plot showing yearly total casualties, with value labels for clarity.

Data Export

Exports the processed and filtered dataset to a new CSV file: dataset Between_1947_2024.csv.

📊 Visualizations
Line Plot:

Shows how total casualties per year have changed over time.

Bar Plot:

Displays total casualties per year with exact counts labeled on each bar.

💾 How to Run
Install required libraries if not already installed:

bash
Copy
Edit
pip install pandas seaborn matplotlib numpy
Place your kkk.csv dataset in the same directory as the script.

Run the script.

Check the generated plots and dataset Between_1947_2024.csv output.

📌 Notes
The code currently filters to 2024 in one place and 2025 in another. This might be redundant and could be harmonized.

Ensure the kkk.csv file has at least Year and Cause columns for this to work correctly.

📎 License
This project is open-source and available under the MIT License (if you want to add one).
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
