## Create a New Matching Rule

When you create a New Matching Rule for the Discovery process, you need to specify a Matching Type. Your selection determines additional fields that display during the creation process, allowing you to further narrow the scope of the rule. There are four Matching Types: Column, Data, Data Function, and Data Sample.

[Column Matching Type](/articles/demo_project/DPM_Demo_Project/07_Discovery/03_03_02_Discovery_NewMatchingRule_Column.md)

The Column Matching Type lets you configure rules that inspect the column names in the databases that are scanned, and then compare them with an expression you define in the Match Pattern field. Using this option, you can see if the column contains PII data.

[Data Matching Type](/articles/demo_project/DPM_Demo_Project/07_Discovery/03_03_03_Discovery_NewMatchingRule_Data.md)

The Data Matching Type lets you narrow your view to the data inside a column. This rule compares data in the database within a column using a set of predefined values.

[Data Function Matching Type](/articles/demo_project/DPM_Demo_Project/07_Discovery/03_03_04_Discovery_NewMatchingRule_DataFunction.md)

The Data Function Matching Type lets you run a function on the content of a sample population from a table. The function verifies the content of the table or column is a valid format. You can set the Probability (percentage) that the function will return content that is PII data.

[Data Sample Matching Type](/articles/demo_project/DPM_Demo_Project/07_Discovery/03_03_05_Discovery_NewMatchingRule_DataSample.md)

The Data Sample Matching Type lets you compare the column content with what a customer provided. You only need to load the function into the table.



[![Previous](/articles/demo_project/DPM_Demo_Project/images/Previous.png)]( /articles/demo_project/DPM_Demo_Project/07_Discovery/03_02_Discovery_Login.md)[<img align="right" width="60" height="54" src="/articles/demo_project/DPM_Demo_Project/images/Next.png">](/articles/demo_project/DPM_Demo_Project/07_Discovery/03_03_02_Discovery_NewMatchingRule_Column.md)
