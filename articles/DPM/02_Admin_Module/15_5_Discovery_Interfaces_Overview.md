## Interfaces Configuration Tab Overview

The Interfaces Configuration tab contains options for telling the system the location of databases you want to scan. 

The Interface tab has 2 main functions.

- You can tell system where the databases are that you want to scan. 
- You can run a scan of the databases using criteria set in the Interfaces tab.

![image](/articles/DPM/images/Figure_79_Discovery_InterfacesTab.jpg)

The system should not allow more than one entry for this table in the same system. Every database that you connect to should have up to one entry in the table. When you execute a request for mapping, discovery, or Personally Identifiable Information (PII), the system will use only one process per database. It will not use two or more combinations. For each interface, there should be up to 1 entry in the table, or the system will block it.

If you enter an 85% Probability, only results of 85% or more Probability how likely a rule indicates that the columns indeed have data that should be protected. Every Matching Type of data displays a list of options. A Data Sample returns a table with a list of options. This information is in the DPM Fabric and can hold more than what you need to write. Data and Data Sample options—similar only in location—are controlled or impacted by the Probability percentage.

If you have a Matching Type of Data or Data Sample, you can define within the system each Role to inspect before the system decides whether a column contains PII data. The result lets you flag the column as a probable PII and displays in the Results tab. Refer to *9.4* *Results Tab Overview* for additional information.


[![Previous](/articles/DPM/images/Previous.png)]( /articles/DPM/02_Admin_Module/15_4_Discovery_Create_New_Matching_Rule.md)[<img align="right" width="60" height="54" src="/articles/DPM/images/Next.png">](/articles/DPM/02_Admin_Module/15_6_Discovery_Create_New_Interface.md)
