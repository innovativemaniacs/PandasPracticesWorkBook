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
Analysis 2 
Web Server Log Analysis
📑 Project Overview
This project parses the Calgary web server access log file, converts it into a structured CSV format, and performs exploratory data analysis using Python, Pandas, Seaborn, and Matplotlib.
It visualizes key metrics like HTTP status distribution, most frequent hosts, most requested files, and API request patterns over time.
________________________________________
📦 Dependencies
Make sure to install the following libraries before running the notebook:
pip install pandas matplotlib seaborn numpy requests
📁 Files Included
calgary_acess_log.txt → Raw web server log file

calgary_api_requests.csv → Parsed and cleaned structured data

log_analysis.ipynb → Jupyter notebook containing the parsing, EDA, and visualization code

README.md → Project description and instructions (this file)

🔍 Project Workflow
1️⃣ Parse Log File
Using regex, extract important components like:

Host

Datetime

HTTP Method

Requested File

Protocol

Status Code

Response Size

And save them into a CSV file calgary_api_requests.csv

2️⃣ Load and Clean Data
Load CSV into a pandas DataFrame

Drop missing values

Convert response size to numeric

Convert datetime strings to proper datetime format with timezone info

3️⃣ Exploratory Data Analysis & Visualizations
Distribution of HTTP Status Codes

Top 10 Most Frequent Hosts

Top 10 Most Requested Files

Distribution of Response Sizes

Identify the Most Active Day

Plot Number of Requests Over Time

All plots generated using Seaborn and Matplotlib.

📊 Key Findings
Most frequent host making requests

Most requested file on the server

Distribution of HTTP response status codes

Peak days based on number of requests

📌 How to Run
Clone the repository or download the files.

Install required dependencies.

Run the log_analysis.ipynb notebook sequentially.

Ensure calgary_acess_log.txt is in the same directory as your notebook.

📚 Notes
Datetime parsing handles timezone info using the format:
%d/%b/%Y:%H:%M:%S %z
Example: 24/Oct/1994:13:41:41 -0600

Error handling with errors='coerce' ensures invalid datetimes are dropped cleanly.

Plots are neatly styled and rotated for readability.

📈 Sample Visualizations
HTTP Status Code Distribution

Top Hosts & Files Requested

Response Size Histogram

Daily Requests Over Time

✍️ Author
Wildreamer | 2025
“Data speaks — listen well.” 📊✨

