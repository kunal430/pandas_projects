# Exploratory Data Analysis (EDA) of Titanic Dataset

This notebook performs an initial exploratory data analysis of the Titanic dataset.  The analysis is incomplete and serves as a starting point for further investigation.

## Data Loading and Initial Exploration

The notebook begins by loading the necessary libraries (pandas, matplotlib, seaborn) and mounting Google Drive to access the dataset.  The dataset is then loaded into a pandas DataFrame. Basic exploratory steps include:

- `data.head()`: Displaying the first few rows of the dataset.
- `data.describe()`: Generating descriptive statistics for numerical columns.
- `data.info()`: Providing information about the data types and non-null values in each column.


## Data Cleaning

Several columns are deemed irrelevant for further analysis and are dropped:

- 'PassengerId'
- 'Name'
- 'Ticket'
- 'Fare'
- 'Cabin' (due to a high number of missing values)

A heatmap of missing values is generated to visually identify columns with missing data.  The 'Cabin' column is dropped due to its substantial number of missing values.


## Missing Value Handling

The percentage of missing values in each column is calculated. The 'Age' column contains missing values, which are analyzed in the code to determine appropriate handling strategies.  Further work will be needed to fill or remove the missing values.
