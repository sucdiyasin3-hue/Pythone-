📌 Project Overview
This project demonstrates the basic steps of loading, exploring, and understanding a dataset using Python and the Pandas library in Google Colab.
The notebook covers essential data-analysis techniques such as:
Importing Python libraries
Loading an Excel dataset
Viewing the first and last records
Selecting random samples
Checking dataset dimensions
Displaying column names
Checking data types
Reviewing dataset information
Generating descriptive statistics
🛠️ Tools and Technologies
Python 3
Google Colab
Pandas
Microsoft Excel — source format of the dataset
📂 Project Structure
Project/
│
├── Copy_of_pythone.ipynb
├── MY Project qayta saxda ah.xlsx
└── README.md
Main Files
Copy_of_pythone.ipynb
The Jupyter/Google Colab notebook containing the Python code used for dataset exploration.
MY Project qayta saxda ah.xlsx
The Excel dataset loaded and explored in the notebook.
📊 Dataset
The notebook loads the Excel dataset using Pandas:
import pandas as pd

data = pd.read_excel(
    "/content/drive/MyDrive/Colab Notebooks/MY Project qayta saxda ah.xlsx"
)
The dataset is then examined to understand its structure, columns, data types, and statistical characteristics.
Note: The notebook records the dataset as having 151 rows and 9 columns. This description should be updated if the source Excel file is changed.
🔍 Data Exploration
1. Import Pandas
Pandas is imported with the alias pd:
import pandas as pd
Pandas provides tools for working with tabular data such as Excel and CSV files.
2. Load the Dataset
The Excel file is loaded into a Pandas DataFrame called data:
data = pd.read_excel("path_to_excel_file.xlsx")
A DataFrame makes it possible to analyze and manipulate the dataset using Python.
3. View the First Five Rows
data.head()
The head() function displays the first five rows of the dataset.
This is useful for getting an initial view of the data.
4. View the Last Five Rows
data.tail()
The tail() function displays the last five rows of the dataset.
This helps verify how the dataset ends and whether the records appear correctly loaded.
5. View a Random Sample
data.sample(5)
The sample() function displays five randomly selected rows.
This provides a quick way to inspect different records rather than only looking at the beginning or end of the dataset.
6. Display Column Names
data.columns
This returns the names of all columns in the dataset.
Understanding the column names is important before performing further analysis.
7. Check Dataset Dimensions
data.shape
The shape attribute returns:
(number of rows, number of columns)
For example:
(151, 9)
means that the dataset contains 151 rows and 9 columns.
8. Check Data Types
data.dtypes
This displays the data type of each column.
Common Pandas data types include:
int64 — integer numbers
float64 — decimal numbers
object — text/categorical data
datetime64 — dates and times
9. Display Dataset Information
data.info()
The info() function provides a summary of the DataFrame, including:
Number of rows
Number of columns
Column names
Non-null values
Data types
Memory usage
This is particularly useful for identifying missing values and understanding the structure of the dataset.
10. Descriptive Statistics for Numerical Data
data.describe()
The describe() function generates descriptive statistics for numerical columns.
It commonly displays:
count
mean
std
min
25%
50%
75%
max
These statistics help summarize the numerical characteristics of the dataset.
11. Descriptive Statistics for All Columns
data.describe(include="all")
Using include="all" requests descriptive statistics for both numerical and categorical columns where applicable.
This provides a broader overview of the dataset.
🧭 Analysis Workflow
The notebook follows this general workflow:
Import Library
      ↓
Load Dataset
      ↓
View First Rows
      ↓
View Last Rows
      ↓
View Random Sample
      ↓
Check Columns
      ↓
Check Dataset Shape
      ↓
Check Data Types
      ↓
Review Dataset Information
      ↓
Generate Descriptive Statistics
🎯 Project Objectives
The main objectives of this notebook are to:
Learn how to use Pandas for data analysis.
Load an Excel dataset into Python.
Understand the structure of a dataset.
Inspect records before analysis.
Identify columns and their data types.
Check for missing or non-null values.
Generate basic descriptive statistics.
Prepare the dataset for further data cleaning and analysis.
🚀 How to Run the Project
Using Google Colab
Open Google Colab.
Upload or open Copy_of_pythone.ipynb.
Make sure the Excel dataset is available in the specified Google Drive location.
Run the notebook cells from top to bottom.
Review the displayed tables, dataset information, and statistics.
Important
If the Excel file is stored in a different location, update the path in:
data = pd.read_excel("path_to_excel_file.xlsx")
📈 Future Analysis
This notebook provides the foundation for more advanced data analysis. Possible next steps include:
Data cleaning
Handling missing values
Removing duplicates
Data type conversion
Filtering and sorting data
Grouping and aggregation
Data visualization
Correlation analysis
Further statistical analysis
👩‍💻 Author
Sucdi Yasin Xusein
This project was created as part of a practical learning project in Python and Data Analysis.
📝 Conclusion
The notebook demonstrates the fundamental process of exploring a dataset with Pandas. By inspecting the dataset's rows, columns, dimensions, data types, missing values, and descriptive statistics, the data becomes easier to understand and ready for further analysis. """
