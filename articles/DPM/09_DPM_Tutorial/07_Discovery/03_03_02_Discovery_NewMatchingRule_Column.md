### Create a New Matching Rule - Column Type

In this example we will describe how to configure a matching rule that inspects the column names at the database in order to identify which fields might contain PII data. The specific rule we will configure in this example is one that looks for column containing social security number. This is a rule that already exists in the built-in rules of the discovery functionality and the description below is used only for the purpose of exemplifying this option. 

Click the ![image](../images/ICON_NewMatchingRule.jpg) button at the top-right of the screen in order to configure a new matching rule. 

![image](../images/07_12_Discovery_RulesTab_Callout.jpg)

The New Matching Rule dialog box displays. 

![image](../images/07_1_Discovery_NewMatchingRule.jpg)

Select a **Matching** **Category**. Categories are used for grouping Matching Rule topics. This field lets the user classify the new rule under an existing Category or select **New Category** to manually enter a new one. In the image below we chose "Contact Info", but you can use any category name.

In the **Field Type** we specify what is the nature of the field we are looking for. It can be one of the built-in options or a new type. We selected **SOCIAL_SECURITY_NUMBER**. 

Set the **Probability** percentage of the New Matching Rule. This describes the level of confidence you attribute to the finding of the discovery process for a field that matches the rule. For this tutorial, we will set the Probability to **80**%. 

Select the **Matching Type**. As here we want to demonstrate the discovery based on column name, we will select a **Column** Matching Type. 

![image](../images/07_7_Discovery_NewMatchingRule5.jpg)

After you select a Matching Type, additional entry fields will display depending upon your selection. When you chose the **Column** matching type the fields that are displayed are  **Match Pattern** and **Exclude Pattern**.

The **Match Pattern** defines the pattern of the column name that you are searching form. You can type any valid Regular expression (regex) in this field. 
The **Exclude Pattern** defines the pattern that you would like to ignore. 
The discovery process will list in its results all the columns that both matched the **Include Pattern** and didn't match the **Exclude Pattern**.

![image](../images/07_8_Discovery_NewMatchingRule6.jpg)

Enter a **Match Pattern**.

![image](../images/07_9_Discovery_NewMatchingRule7.jpg)

Enter an **Exclude Pattern**.

![image](../images/07_11_Discovery_NewMatchingRule9.jpg)

Review your entries as needed, and then click ![image](../images/08_ICON_Save.jpg).

The New Matching Rule displays in the Matching Rules table. If your table contains entries that span across multiple screen pages, you can distill the results by selecting the relevant Matching Type. Since we chose the “Column” Matching Type for the New Matching Rule, select Column from the Matching Type dropdown list.

![image](../images/07_2_Discovery_NewMatchingRule10.jpg)

The New Matching Rule displays in the table.

![image](../images/07_3_Discovery_NewMatchingRule11_Callout.jpg)



[![Previous](../images/Previous.png)]( 03_03_01_Discovery_NewMatchingRule_Landing.md)[<img align="right" width="60" height="54" src="../images/Next.png">](03_03_03_Discovery_NewMatchingRule_Data.md)
