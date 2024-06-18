# Deloitte

From CSV files to Staging DB
This step is a must to get all the data from the flat files into one table in the DB.
Such step will accumalte the data with all inconsistencies in one place

From Staging to DWH
Splitting the solo table into 5 tables to distinguish the fact table (transactions) and the dimention tables as a lookup.
This schema (snowflake) is a great step to filter the data and drop the redunadant records
This schema is powerful when its come to get the historical needs from the tables.
This schema is powerful to clear the tables from the inconsistencies.

Considerations
The data dublication is cleared by tale the most recent record and consider the rest as a dimention table.
The data pipileine are set to be every 5 min up to 5 times daily depends of the stack holder needs 


Suggestions
Building a data cube as a data mart will decalre more and more reports from one data mart.
The primary key must turn into intergers.
the data migration must be down immediatly (not after one month)
