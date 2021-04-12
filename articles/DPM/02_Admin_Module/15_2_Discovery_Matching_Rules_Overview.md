## Discovery Matching Rules Overview

There are three activity phases in the Discovery Matching Rules function.

- Define a set of rules to use for the PII discovery process.
- Define interfaces (systems and databases you can connect to search for PII data).
- Execute the discovery and review the results to determine which actions to take for each field indicated by the discovery process.

Matching Rules are configured by accessing the Discovery Matching Rules menu option.

![image](/articles/DPM/images/Figure_75_Discovery_LeftPanel.jpg)

The “Discovery Matching Rules” screen displays.

## Matching Rules Tab Overview

![image](/articles/DPM/images/Figure_76_Discovery_MatchingRulesTab.jpg)

In this screen, you can define rules of how to identify where in your system the data may be Personally Identifiable Information (PII) data. 

This functionality provides multiple possibilities for the data inspection. For example, you can inspect data by looking at the column name, by comparing the data itself to a list of values, by running a function that validates the field content, or by comparing the fields content with data in a reference table. The system has a built-in set of rules and any other rules can be built in through configuration, using this screen.

###  Using the Matching Type Drop-Down Options

The Matching Type drop-down list lets you filter according to matching type. The purpose of filtering by Matching Type is to find ways to define columns that hold PII data. For example, in order to identify columns that hold address data, you can search by looking at the Column name or Column content. The DPM system provides 4 different Matching Types, which are defined below. To observe how the different Matching Types are used to formulate rules for the discovery process, click the Matching Type drop-down list. The following options display.

![image](/articles/DPM/images/Figure_77_Discovery_MatchingType.jpg)

- **Column** – Use the Column Matching Type to configure rules that inspect the column names in the databases that are scanned, and then compare them with an expression you define in the Match Pattern field. Using this option, you can see if the column contains PII data. For example, if a column name is “bank account number”, then it holds a bank account number and should be protected. 
- **Data** – The Data Matching Type lets you narrow your view to the data inside a column. This rule compares data in the database within a column using a set of predefined values. 
- **Data Function** – The Data Function Matching Type lets you run a function on the content of a sample population from a table. The function verifies the content of the table or column is a valid format. You can set the Probability (percentage) that the function will return content that is PII data.  

  For example, you could assume a column holds credit card information. When you run a function and receive a positive answer, then you can assume there is a 100% chance that it holds credit card information because it is unlikely that this string of numbers is not indicative of a credit card number. However, when you validate a social security number, the 9-digit number could be an account number of the same format. Therefore, the Probability would be lower (ex: 70%.)
- **Data Sample** – The Data Sample Matching Type lets you compare the column content with what a customer provided. You only need to load the function into the table. For example, if a customer provides a list of postal codes, where many options exist, you will not need to write out each one.


[![Previous](/articles/DPM/images/Previous.png)]( /articles/DPM/02_Admin_Module/15_1_Discovery_Introduction.md)[<img align="right" width="60" height="54" src="/articles/demo_project/DPM_Demo_Project/images/Next.png">](/articles/DPM/02_Admin_Module/15_3_Discovery_Create_New_Matching_Rule.md)