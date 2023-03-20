# **Data cleansing checklist**

This is a data cleaning checklist that can be used as a guide for cleaning and preparing datasets for analysis.

If data is unstructured i.e. column names can be found in rows along values, then the transpose feature can be utilised.

Ensure query names are relevant to the data it contains.

Columns must contain appropriate names.

If the queries for different data are structured the same and have related data these queries can be combined into one, through appending. Similar query structures can be determined if the column numbers are the same and each column name is identical. Upon merging the queries select a filter for one of the columns to ensure all queries were merged correctly. If they were not, this could be due to different formats for a column. Also, rename the new query.

There should not be any empty fields and errors, go through every column to confirm. Check 'Column Quality', 'Column Distribution' and 'Column Profile' (in Power BI) to view if these issues exist. All columns should have a valid number of 100%

Search through each column, using filters, to ensure data is consistent. If there are inconsistencies with the data, this could be due to the source data or Power BI. First check through the source data to identify if the problem is occuring there. If an error is identified you have to first understand the reason, then replace the values within Power BI as opposed to the source data.

Exlude irrelevant columns, that are unnceccsary to the visualisation process. This is for speed and efficiency purposes.

Ensure dates are formatted correctly based on the country that the data will be displayed to. If the dates are in a different country format, in Power BI, change the locale to the correct one. Verify the locale through either: checking the settings or creating an additional column for the month of each date.

In Power BI, each column should have the correct data type. This can be changed manually or through the 'Detect Data type' button under the 'Transform' ribbon. In Power BI, the altered data type will need to be applied to the whole dataset. This can be done by clicking 'Apply' under the 'Home' tab. Errors may be picked up as a result of this. These will need to be troublehsooted, depending on the error.

If there are several decimal values for each column and the data is related for example prices, the values in these columns should all be rounded to the same decimal place.

Depending on the value of the fields, columns may need to be unpivoted and then pivoted. This is to establish an ordered structure to the columns which will assist in creating visuals, later on.

In Power BI, text in a range (i.e. "0-5") cannot be sorted (neither ascending or descending). Therefore to sort by these values they will need to be first extracted either through the buttons "Split Columns" or "Extract", by their delimeter. These values should then be converted to a number.

## **Contributing**
This checklist is a work in progress and may not cover all data cleaning scenarios. Please note: The properties a dataset, referenced in the checklist (above), will typically be required across all systems. However, methods to cleanse the data will often be in reference to the Business Intelligence tool: Power BI. These cleaning methods can be performed in other tools/software. If you would like to contribute to this checklist, feel free to fork this repository and submit a pull request with your changes.
