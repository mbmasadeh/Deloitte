# Deloitte

<p>From CSV files to Staging DB</p>
<p>This step is a must to get all the data from the flat files into one table in the DB.</p>
<p>Such step will accumalte the data with all inconsistencies in one place</p>

<p>From Staging to DWH</p>
<p>Splitting the solo table into 5 tables to distinguish the fact table (transactions) and the dimention tables as a lookup.<p>  
<p>This schema (snowflake) is a great step to filter the data and drop the redunadant records</p>
<p>This schema is powerful when its come to get the historical needs from the tables.</p>
<p>This schema is powerful to clear the tables from the inconsistencies.</p>

<p>Considerations</p>
<p>The data dublication is cleared by tale the most recent record and consider the rest as a dimention table.</p>
<p>The data pipileine are set to be every 5 min up to 5 times daily depends of the stack holder needs </p>


<p>Suggestions</p>
<p>Building a data cube as a data mart will decalre more and more reports from one data mart.</p>
<p>The primary key must turn into intergers.</p>
<p>the data migration must be down immediatly (not after one month)</p>
