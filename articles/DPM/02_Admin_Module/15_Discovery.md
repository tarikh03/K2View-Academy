# PII Discovery

Personally Identifiable Information (PII) data is information that could be criminally used to conduct identity theft or other crimes against a person. This data could be healthcare information, social security numbers, bank account numbers, or credit card data. Understanding where this information resides and preventing an unauthorized release of PII data are important measures that every business should use to keep customers’ personal data secure.

PII data represents an attractive target to criminals because it can be sold and later used for an array of criminal activities from basic fraud to identity theft. Loss of a company’s PII can result in many issues, including customer trust and loyalty.

PII discovery, or sensitive data discovery, is a process that detects patterns by applying various analytical methods, or by visually navigating through the data. A company may have many different systems, and each system has its own database. For each database, you can analyze the data and column names to find out which database table or column holds data that can identify the customer or reveal information that should remain private. 

The Discovery Matching Rules function of the DPM system lets you search databases of all systems within the company for personal data that may be protected by privacy legislation. You can create rules to either match or exclude data during a database search, configure regular expression (RegEx) schema and table patterns to match or exclude, and view the discovery results using an array of filters.

## Discovery Matching Rules Overview

There are 3 phases within the Discovery Matching Rules function.

•	Define a set of rules to be used for the PII discovery process.
•	Define interfaces – systems and databases you can connect to search for PII data.
•	Execute the discovery and review the results to decide what to do on each of the fields indicated by the discovery process.

Matching Rules are configured by accessing the Discovery Matching Rules menu option.

<Image - left menu>

The “Discovery Matching Rules” screen displays.

## Matching Rules Tab Overview

<image-MatchingRulesTab>

In this screen, you can define rules of how to identify where in your system the data may be Personally Identifiable Information (PII) data. 

This functionality provides multiple possibilities for the data inspection. For example, you can inspect data by looking at the column name, by comparing the data itself to a list of values, by running a function that validates the field content, or by comparing the fields content with data in a reference table. The system has a built-in set of rules and any other rules can be built in through configuration, using this screen.

###  Using the Matching Type Drop-Down Options

The Matching Type drop-down list lets you filter according to matching type. The purpose of filtering by Matching Type is to find ways to define columns that hold PII data. For example, in order to identify columns that hold address data, you can search by looking at the Column name or Column content. The DPM system provides 4 different Matching Types, which are defined below. To observe how the different Matching Types are used to formulate rules for the discovery process, click the Matching Type drop-down list. The following options display.

<image>

•	Column – Use the Column Matching Type to configure rules that inspect the column names in the databases that are scanned, and then compare them with an expression you define in the Match Pattern field. Using this option, you can see if the column contains PII data. For example, if a column name is “bank account number”, then it holds a bank account number and should be protected. 

•	Data – The Data Matching Type lets you narrow your view to the data inside a column. This rule compares data in the database within a column using a set of predefined values. 

•	Data Function – The Data Function Matching Type lets you run a function on the content of a sample population from a table. The function verifies the content of the table or column is a valid format. You can set the Probability (percentage) that the function will return content that is PII data.  

For example, you could assume a column holds credit card information. When you run a function and receive a positive answer, then you can assume there is a 100% chance that it holds credit card information because it is unlikely that this string of numbers is not indicative of a credit card number. However, when you validate a social security number, the 9-digit number could be an account number of the same format. Therefore, the Probability would be lower (ex: 70%.)

•	Data Sample – The Data Sample Matching Type lets you compare the column content with what a customer provided. You only need to load the function into the table. For example, if a customer provides a list of postal codes, where many options exist, you will not need to write out each one.

### Create a New Matching Rule

Click the <image>  button at the top-right of the screen in order to configure a new Matching Rule.

<image>

The following dialog box displays.

<image>

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
<p>Select a category that is defined within this  option. Select <b>+New Category</b> from the drop-down to create a new category</p>
</td>
</tr>
<tr>
<td width="85">
<p>Field Type</p>
</td>
<td width="785">
<p>Select a filed type that  is defined within this option. Select <b>+New Field Type</b> to add a new field  type.</p>
</td>
</tr>
<tr>
<td width="85">
<p>Active</p>
</td>
<td width="785">
<p>The “Active” slider is  turned to “On” by default. Turn the slider to “Off” if you do not want the  new Matching Rule to be active in the table. </p>
</td>
</tr>
<tr>
<td width="85">
<p> Probability (1 – 100%)</p>
</td>
<td width="785">
<p>Set the probability  percentage of the new Matching Rule. For example, when you validate a social  security number, the 9-digit number could be an account number of the same  format. Therefore, the Probability would be lower (ex: 70%.)</p>
</td>
</tr>
<tr>
<td width="85">
<p>Matching  Type</p>
</td>
<td width="785">
<p>Select the Matching Type.  Choose between Column, Data, Data Function, and Data Sample.</p>
</td>
</tr>
</tbody>
</table>

### Edit or Delete a Matching Rule

Use the <image> button to delete a Matching Rule. 

Note: If you click the <image> button, the system displays a dialog box, prompting “Are you sure you want to delete matching type?” Click the “OK” button to remove the selected Matching Type from the system.

Use the <image> button to edit the Matching Category, Field Type, Probability, and Matching Type.


