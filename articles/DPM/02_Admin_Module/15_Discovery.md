# PII Discovery

Personally Identifiable Information (PII) data is information that could be used to conduct identity theft or other crimes against a person. High-level examples of this data include healthcare information, social security numbers, bank account numbers, or credit card data. It could also be more simple information, such as last names, addresses, and birth dates. Any personal data can be an attractive target to criminals, as it can be used for an array of unlawful activities, from basic fraud to identity theft. 

Breaches in a company’s PII data can ultimately result in a multitude of losses, including customer trust and loyalty. Understanding where this information resides in your systems and preventing its unauthorized release are important measures that every business should conduct to keep a customer's personal data secure.

PII discovery is a process that detects patterns by applying various analytical methods. A company can have multiple source systems, each one using its own database. For each of these databases, the DPM system can analyze the data and column names at a granular level to discover which database table or column holds data that could identify a customer, or potentially reveal additional information that should remain private. 

The Discovery Matching Rules function of the DPM system lets you search databases of all systems within the company for personal data that may be protected by privacy legislation. You can create rules to either match or exclude data during a database search, configure regular expression (RegEx) schemas and table patterns, and view the discovery results using an array of filters.

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

### Create a New Matching Rule

Click the ![image](/articles/DPM/images/Figure_82_Discovery_NewMatchingRule.jpg) button at the top-right of the screen in order to configure a new Matching Rule.

![image](/articles/DPM/images/Figure_83_Discovery_MatchingRulesTab_Callout.jpg)

The following dialog box displays.

![image](/articles/DPM/images/Figure_78_Discovery_NewMatchingRule.jpg)

<table>
<tbody>
<tr>
<td width="85">
<p><strong>Property</strong></p>
</td>
<td width="785">
<p><strong>Description</strong></p>
</td>
</tr>
<tr>
<td width="85">
<p> Matching  Category</p>
</td>
<td width="785">
<p>Select a category that is defined within this  option. Select <b>+New Category</b> from the drop-down to create a new category.</p>
</td>
</tr>
<tr>
<td width="85">
<p>Field Type</p>
</td>
<td width="785">
<p>Select a filed type that is defined within this option. Select <b>+New Field Type</b> to add a new field  type.</p>
</td>
</tr>
<tr>
<td width="85">
<p>Active</p>
</td>
<td width="785">
<p>The “Active” slider is turned to “On” by default. Turn the slider to “Off” if you do not want the  new Matching Rule to be active in the table.</p>
</td>
</tr>
<tr>
<td width="85">
<p> Probability (1 – 100%)</p>
</td>
<td width="785">
<p>Set the probability  percentage of the new Matching Rule. For example, when you validate a social  security number, the 9-digit number could be an account number of the same  format. Therefore, the Probability would be lower (ex: 70%).</p>
</td>
</tr>
<tr>
<td width="85">
<p>Matching Type</p>
</td>
<td width="785">
<p>Select the Matching Type.  Choose between Column, Data, Data Function, and Data Sample.</p>
</td>
</tr>
</tbody>
</table>

### Edit or Delete a Matching Rule

Click the ![image](/articles/DPM/images/ICON_Delete.jpg) button to delete a Matching Rule. 

Note: If you click the ![image](/articles/DPM/images/ICON_Delete.jpg) button, the system displays a dialog box, prompting “Are you sure you want to delete matching type?” Click the ![image](/articles/DPM/images/ICON_Delete_02.jpg) button to remove the selected Matching Type from the system.

Click the ![image](/articles/DPM/images/ICON_Edit.jpg) button to edit the Matching Category, Field Type, Probability, and Matching Type.

## Interfaces Configuration Tab Overview

The Interfaces Configuration tab contains options for telling the system the location of databases you want to scan. 

The Interface tab has 2 main functions.

- You can tell system where the databases are that you want to scan. 
- You can run a scan of the databases using criteria set in the Interfaces tab.

![image](/articles/DPM/images/Figure_79_Discovery_InterfacesTab.jpg)

The system should not allow more than one entry for this table in the same system. Every database that you connect to should have up to one entry in the table. When you execute a request for mapping, discovery, or Personally Identifiable Information (PII), the system will use only one process per database. It will not use two or more combinations. For each interface, there should be up to 1 entry in the table, or the system will block it.

If you enter an 85% Probability, only results of 85% or more Probability how likely a rule indicates that the columns indeed have data that should be protected. Every Matching Type of data displays a list of options. A Data Sample returns a table with a list of options. This information is in the DPM Fabric and can hold more than what you need to write. Data and Data Sample options—similar only in location—are controlled or impacted by the Probability percentage.

If you have a Matching Type of Data or Data Sample, you can define within the system each Role to inspect before the system decides whether a column contains PII data. The result lets you flag the column as a probable PII and displays in the Results tab. Refer to *9.4* *Results Tab Overview* for additional information.

### Add an Interface

Click the ![image](/articles/DPM/images/Figure_85_Discovery_AddInterface.jpg) button at the top-right of the screen in order to configure a new Interface.

![image](/articles/DPM/images/Figure_87_Discovery_AddInterface_Callout.jpg)

The following dialog box displays.

![image](/articles/DPM/images/Figure_81_Discovery_NewInterface.jpg)

<table>
<tbody>
<tr>
<td width="85">
<p><strong>Property</strong></p>
</td>
<td width="785">
<p><strong>Description</strong></p>
</td>
</tr>
<tr>
<td width="85">
<p> Interface</p>
</td>
<td width="785">
<p>Select an interface from the drop-down list. For example, select “dbsalesforce”. This list is populated by options configured in the DPM fabric software. </p>
</td>
</tr>
<tr>
<td width="85">
<p>Catalog Pattern (Regex)</p>
</td>
<td width="785">
<p>Information Needed</p>
</td>
</tr>
<tr>
<td width="85">
<p>Schema Name Inclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>All tables in the database are defined in the Schema part of the DPM fabric software Creator Interface. For example, for a new Interface called “dbsalesforce”, select “SFORCE” from the Schema Name Inclusion Pattern drop-down list.</p>
</td>
</tr>
<tr>
<td width="85">
<p> Probability (1 – 100%)</p>
</td>
<td width="785">
<p>Set the probability  percentage of the new Matching Rule. For example, when you validate a social  security number, the 9-digit number could be an account number of the same  format. Therefore, the Probability would be lower (ex: 70%).</p>
</td>
</tr>
<tr>
<td width="85">
<p>Schema Name Exclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>All tables in the database are defined in the Schema part of the fabric software Creator Interface. For example, for a new Interface called “dbsalesforce”, select “PUBLIC” from the Schema Name Exclusion Pattern drop-down list.</p>
</td>
</tr>
<tr>
<td width="85">
<p>Table Name Inclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>Refine your search further by telling the system to include specific tables. For example, you can include the database tables for all instances of “ACCOUNT.” </p>
</td>
</tr>
<tr>
<td width="85">
<p>Table Name Exclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>Refine your search further by telling the system to exclude specific tables. For example, you can exclude searching the database tables for all instances of “ACCOUNT.” </p>
</td>
</tr>
<tr>
<td width="85">
<p>Active</p>
</td>
<td width="785">
<p>The “Active” slider is turned to “On” by default. Turn the slider to “Off” if you do not want the new Interface to be active in the table.</p>
</td>
</tr>
</tbody>
</table>

###  Edit or Delete an Interface

Use the ![image](/articles/DPM/images/ICON_Delete.jpg) button to delete an Interface. 

**Note**: If you click the ![image](/articles/DPM/images/ICON_Delete.jpg) button, the system displays a dialog box, prompting “Are you sure you want to Delete Interface: [InterfaceName]?” Click the ![image](/articles/DPM/images/08_ICON_OK.png) button to remove the selected Interface from the system.

Click the ![image](/articles/DPM/images/ICON_Edit.jpg) button to edit the Interface name, Schema information, and table information.

### Submit a Discovery Request

Click the ![image](/articles/DPM/images/Figure_84_Discovery_SubmitDiscRequest.jpg) button. 

![image](/articles/DPM/images/Figure_x_image.jpg)

The system will check which Interfaces have been written and that are Active. It will run all the matching rules. The result of your submission will display under the Discovery Requests section, located along the bottom of the Interfaces Configuration tab.

## Results Tab Overview

The Results tab displays the results of clicking ![image](/articles/DPM/images/Figure_84_Discovery_SubmitDiscRequest.jpg) in the Interfaces Configuration tab.

![image](/articles/DPM/images/Figure_x_image.jpg)

Click the ![image](/articles/DPM/images/ICON_Clear.jpg) button to reset all criteria for returning results to the default selections.


 
[![Previous](/articles/DPM/images/Previous.png)](/articles/DPM/02_Admin_Module/14_DPM_Main_Menu.md)[<p align="right"> Return to Admin Model Overview</p>](/articles/DPM/02_Admin_Module/01_Admin_Module_Overview.md)
