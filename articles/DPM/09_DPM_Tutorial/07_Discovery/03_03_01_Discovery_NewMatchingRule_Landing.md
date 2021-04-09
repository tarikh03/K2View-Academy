## Create a New Matching Rule

Click the ![image](../images/ICON_NewMatchingRule.jpg) button at the top-right of the screen in order to configure a new matching rule. 

![image](../images/07_12_Discovery_RulesTab_Callout.jpg)

The New Matching Rule dialog box displays. 

![image](../images/07_1_Discovery_NewMatchingRule.jpg)

Before guiding you through the creation of new discovery rules, we would like to describe the different types of rules that can be created. Those types are defined by the Matching Type field. 

There are four Matching Types: Column, Data, Data Function, and Data Sample. Each of those types allows you to configure the process to search PII fields in the database based on a different aspect:

[Column Matching Type](03_03_02_Discovery_NewMatchingRule_Column.md)

The Column Matching Type lets you configure rules that inspect the column names in the databases that are scanned, and then compare them with an expression you define in the Match Pattern field. Using this option, you can identify if the column contains PII data based on the column name.

[Data Matching Type](03_03_03_Discovery_NewMatchingRule_Data.md)

The Data Matching Type lets you narrow your view to the data themselves under each column. This rule compares data in the database for each column using a set of predefined values.

[Data Function Matching Type](03_03_04_Discovery_NewMatchingRule_DataFunction.md)

The Data Function Matching Type lets you run a function on the content of a sample population from a table. The function logic is used to predict if the content of the column is likely to be PII data.

[Data Sample Matching Type](03_03_05_Discovery_NewMatchingRule_DataSample.md)

The Data Sample Matching Type lets you compare the column content with a set of sample data that were previously loaded into a reference table.



[![Previous](../images/Previous.png)]( 03_02_Discovery_Login.md)[<img align="right" width="60" height="54" src="../images/Next.png">](03_03_02_Discovery_NewMatchingRule_Column.md)
