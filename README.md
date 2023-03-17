# **Data cleansing checklist**

This is a data cleaning checklist that can be used as a guide for cleaning and preparing datasets for analysis.

If data is unstructured i.e. column names can be found in rows along values, then the transpose feature can be utilised.

Ensure query names are relevant to the data it contains.

Columns must contain appropriate names.

If the queries for different data is structured the same and has related data, these queries can be combined into one through appending. Similar query structures can be determined if the column numbers are the same and each column name is identical. Upon merging the queries select a filter for one of the columns to ensure all queries were merged correctly. If they were not, this could be due to different formats for a column. Also, rename the new query.

There should not be any empty fields and errors, go through every column to confirm. Check 'Column Quality', 'Column Distribution' and 'Column Profile' (in Power BI) to view if these issues exist. All columns should have a valid number of 100%

Seaerch through each column, through filters, to ensure data is consistent. If there are inconsistencies with the data, this could be due to the source data or Power BI. First check through the source data to identify if the problem is occuring there. If an error is identified you have to first understand the reason, then replace the values within Power BI as opposed to the source data.

## **Contributing**
This checklist is a work in progress and may not cover all data cleaning scenarios. If you would like to contribute to this checklist, feel free to fork this repository and submit a pull request with your changes.
