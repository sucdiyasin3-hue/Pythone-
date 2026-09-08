Python Data Analysis Project

## Project Overview

This project focuses on exploring and understanding a dataset using Python and the Pandas library in Google Colab.

The project demonstrates basic data analysis techniques, including importing libraries, loading an Excel dataset, viewing records, checking the structure of the dataset, examining data types, and generating a summary of the data.

## Tools and Technologies

- Python
- Google Colab
- Pandas
- Microsoft Excel

## Dataset

The dataset contains information about job applicants and their application process.

The dataset contains:

- 300 rows
- 7 columns

### Dataset Columns

| Column | Description |
|---|---|
| Applicant_ID | Unique identification number for each applicant |
| Application_Date | Date when the application was submitted |
| Department | Department applied to |
| Experience_Years | Number of years of work experience |
| Education_Level | Educational qualification of the applicant |
| Interview_Score | Score received during the interview |
| Application_Status | Current status of the application |

## Import Libraries

The Pandas library is imported and given the alias `pd`.

```python
import pandas as pd
Pandas is used for reading, exploring, and analyzing the dataset.
Load Dataset
The Excel dataset is loaded from Google Drive using the read_excel() function.
data = pd.read_excel("/content/drive/MyDrive/Colab Notebooks/MY Project qayta saxda ah.xlsx")
The dataset is stored in a DataFrame named data.
Understanding the Dataset
Reading the First 5 Rows
The head() function is used to display the first five rows of the dataset.
data.head()
This helps us get an initial understanding of the data and its values.
Reading the Last 5 Rows
The tail() function is used to display the last five rows of the dataset.
data.tail()
This allows us to inspect the final records in the dataset.
Reading Sample Data
The sample() function is used to display five randomly selected records.
data.sample(5)
This provides a random view of the dataset and helps us inspect different records.
Dataset Information
The info() function is used to display a summary of the dataset.
data.info()
The dataset contains 300 entries and 7 columns.
The columns and their non-null values are:
Column
Non-Null Count
Applicant_ID
285
Application_Date
285
Department
284
Experience_Years
282
Education_Level
282
Interview_Score
285
Application_Status
282
The output also shows that all seven columns are initially stored as object data types.
Data Exploration Functions
The following Pandas functions were used in the project:
head()
Displays the first five rows.
data.head()
tail()
Displays the last five rows.
data.tail()
sample()
Displays randomly selected rows.
data.sample(5)
info()
Provides information about:
Number of rows
Number of columns
Column names
Non-null values
Data types
Memory usage
data.info()
Missing Values
The info() output shows that some columns contain missing values.
For example:
Applicant_ID has 15 missing values
Application_Date has 15 missing values
Department has 16 missing values
Experience_Years has 18 missing values
Education_Level has 18 missing values
Interview_Score has 15 missing values
Application_Status has 18 missing values
These missing values should be examined and handled during the data-cleaning stage.
Project Workflow
The project follows these main steps:
Import Pandas
Load the Excel dataset
View the first five rows
View the last five rows
Display random sample records
Check the dataset information
Identify columns and data types
Identify missing values
Prepare the dataset for further analysis
Project Objectives
The main objectives of this project are:
To learn how to use Python for data analysis.
To understand how Pandas works with datasets.
To load Excel data into Python.
To explore the structure of a dataset.
To inspect rows and columns.
To identify missing values.
To understand data types.
To prepare the dataset for further data cleaning and analysis.
Example Python Code
import pandas as pd

# Load dataset
data = pd.read_excel(
    "/content/drive/MyDrive/Colab Notebooks/MY Project qayta saxda ah.xlsx"
)

# Display first 5 rows
data.head()

# Display last 5 rows
data.tail()

# Display random 5 rows
data.sample(5)

# Display dataset information
data.info()
Conclusion
This project demonstrates the basic process of exploring a dataset using Python and Pandas.
The dataset contains 300 records and 7 variables related to job applicants, including their application date, department, experience, education level, interview score, and application status.
Using functions such as head(), tail(), sample(), and info(), the dataset was inspected and its structure, missing values, and data types were identified.
This exploration provides a foundation for the next stages of data cleaning, transformation, visualization, and analysis.
Author
Sucdi Yasin Xusein
