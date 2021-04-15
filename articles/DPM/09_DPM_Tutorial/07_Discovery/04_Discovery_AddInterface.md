## Second Tab: Interfaces Configuration

The Interfaces Configuration tab contains options for telling the system the location of databases you want to scan. This tab has two main functions. You can tell system where the databases are that you want to scan, and you can run a scan of the databases using criteria set in the **Interfaces Configuration** tab.

### Add an Interface

Click the ![image](../images/07_Discovery_Interfaces_Tab.png) tab. 

The Interfaces Configuration screen displays.

![image](../images/07_01_Discovery_Interfaces_Config.png)

Click the ![image](../images/07_02_Discovery_Interfaces_AddNew.png) button at the top-right of the screen in order to configure a new interface. The New Discovery Interface dialog box displays. 

![image](../images/07_01_Discovery_Interfaces_New.png)

Select an **Interface**. This list will include all the systems with which the DPM is integrated in your company and is configured in the DPM fabric studio, as part of your project configuration.

![image](../images/07_02_Discovery_Interfaces_New.png)

The following example shows the **New Discovery Interface** screen populated with sample information.

![image](../images/07_03_Discovery_Interfaces_New.png)

For this tutorial, select **dbSalesforce**.

![image](../images/07_04_Discovery_Interfaces_New.png)

Enter a **Catalog Pattern**. For this tutorial, enter **/^Phone**. 

![image](../images/07_05_Discovery_Interfaces_New.png)

Enter a **Schema Name Inclusion Pattern** if you want the discovery process to scan only tables under specific schemas. 

![image](../images/07_06_Discovery_Interfaces_New.png)

Enter a **Schema Name Exclusion Pattern** if you want the discovery process to ignore specific schemas.  

![image](../images/07_07_Discovery_Interfaces_New.png)

Enter a **Table Name Inclusion Pattern** if you want the discovery process to scan only tables with a specific name pattern.

![image](../images/07_08_Discovery_Interfaces_New.png)

Enter a **Table Name Exclusion Pattern** if you want the discovery process to ignore tables with a specific name pattern.

![image](../images/07_03_Discovery_Interfaces_New.png)

Review your entries as needed, and then click ![image](../images/ICON_Save.png).

The New Discovery Interface displays in the Interfaces Configuration table. 

![image](../images/07_09_Discovery_Interfaces_New.png)



[![Previous](../images/Previous.png)]( 03_03_05_Discovery_NewMatchingRule_DataSample.md)[<img align="right" width="60" height="54" src="../images/Next.png">](05_Discovery_SubmitDiscoveryRequest.md)
