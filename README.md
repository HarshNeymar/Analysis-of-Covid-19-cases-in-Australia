# Code Readme

This repository contains code for processing and analyzing daily COVID-19 case data for different states in Australia. The code is written in Python and utilizes the pandas, numpy, and matplotlib.pyplot libraries.

## Data Files
The code assumes the existence of the following data files in the specified directory:
- daily_cases_nsw.tsv
- daily_cases_qld.tsv
- daily_cases_sa.tsv
- daily_cases_vic.tsv
- daily_cases_wa.tsv

Please make sure to provide the correct file paths for these data files in the code.

## Code Overview
The code performs the following tasks:

1. Reads the data files into separate pandas DataFrames for each state.
2. Defines a function, `remove_commas`, to remove commas from numeric columns in the DataFrame.
3. Defines a function, `process_dataframe`, to process each DataFrame, including the following steps:
   - Prints the shape of the DataFrame.
   - Prints information about the DataFrame, such as column names, non-null counts, and data types.
   - Prints descriptive statistics of the DataFrame.
   - Drops the 'VAR' column from the DataFrame.
   - Checks for null values and prints the count for each column.
   - Converts the 'DATE' column to datetime type.
   - Calls the `remove_commas` function to remove commas from numeric columns.
   - Handles null values by filling them with appropriate values.
   - Prints the modified DataFrame.
   - Returns the processed DataFrame.
4. Calls the `process_dataframe` function for each state's DataFrame.
5. Performs additional data cleaning steps for specific columns in each DataFrame, such as converting data types and handling null values.

## Usage
To use this code, follow these steps:

1. Make sure the required data files are present in the specified directory.
2. Update the file paths in the code to match the location of the data files.
3. Run the code.

The code will process each DataFrame, print relevant information and modified DataFrames, and perform additional data cleaning steps.

Note: This README provides an overview of the code and its functionality. For more detailed information, please refer to the code comments and documentation.

Feel free to customize and extend the code as per your requirements.

Enjoy!
