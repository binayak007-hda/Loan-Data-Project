# Loan-Data-Project
The dataset underwent a thorough cleaning process to ensure quality and consistency. Key steps included:
Handling Missing Values: Missing values were identified and and either imputed with max values or mean values in the column as per data requirements. None of the entries were dropped. 
Data Type Corrections: Dates were converted to datetime format and to use NumPy effectively, converted strings into numerical values.
Encoding Categorical Variables: Categorical fields like `loan_status` were encoded to numerical values (e.g., column contained '', 'Not Verified', 'Source Verified', 'Verified', converted '' and 'Not Verified' as 'bad' and 'Source Verified' and 'Verified' as 'good'. Subsequently, converted them into numerical values 0 and 1 respectively).
Filtering Data: Irrelevant columns like 'grade' with repeated data were removed (e.g., 'grade' column had 'A', 'B', 'C', 'D', 'E' categories and sub-grade had 'A1', 'A2', 'A3', 'A4', 'A5', 'B1', and so on. Filled the missing values in 'sub-grade' with reference to 'grade' column and removed 'grade')
For a detailed look at the data cleaning steps, please refer to the [Loan_data_cleaned.py]
