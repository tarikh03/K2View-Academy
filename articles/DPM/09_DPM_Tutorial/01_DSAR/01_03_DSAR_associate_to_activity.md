# Associate the DSAR Flow with a Regulation and Activity

In the previous steps, we configured a Flow that performs the Tasks to retrieve customer data.

For this Flow to be visible to a customer who wants to submit a Request, it should be associated with an Activity, under a specific Regulation. You can read more details about [Regulations](articles/DPM/02_Admin_Module/08_Regulations.md) and [Activities](/articles/DPM/02_Admin_Module/09_Activities.md) in the DPM User Guide. 

We will now create a new Regulation, add a new Activity under it, and then we will associate the "DSAR Tutorial" Flow. 

1. Select the menu option **Regulation List**.

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Admin_Menu_Regulation.png" width="30%" height="30%">

2. Click <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_New_Regulation_Icon.png" width="10%" height="10%"> to create a new Regulation. Populate the information for this new Regulation as shown below. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Regulations_List.png" width="100%" height="100%">

After you save the new Regulation, the screen of Activities for this Regulation displays, initially empty because no Activity has been created. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Empty_Regulation.png" width="100%" height="100%">

3. Click <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_New_Activity_Icon.png" width="10%" height="10%"> to add a new Activity under this Regulation. Populate the information for this new Activity as shown below, selecting **DSAR Tutorial** in the **Flow Name** field, which was created in the previous steps. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Link_Activity_1.png" width="30%" height="30%">

This screen allows additional configurations, including the following examples.

- Use the <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Link_Activity_Allow_Extension_Icon.png" width="13%" height="13%"> icon in order to allow extension of the duration of the Activity.
-  Use the <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Link_Activity_Automatic_Extension_Icon.png" width="16%" height="16%"> icon, which will result in automatic extension of the Activity SLA before it becomes overdue. The **Days Before Due Date** field defines how many days before the due date of a Request the automatic extension should be triggered.  

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Link_Activity_2.png" width="30%" height="30%">

Saving the new Activity makes the new Flow we created available for customers to submit Requests based on the Flow.  

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Link_Activity_3.png" width="100%" height="100%">

The submission and execution of such requests is described in the next section of this tutorial: [DSAR Request Execution]().  

  

[![Previous](/articles/demo_project/DPM_Demo_Project/images/Previous.png)]( /articles/demo_project/DPM_Demo_Project/01_DSAR/01_02_04_DSAR_Finalize_Flow.md)[<p align="right"> Return to Data Subject Access Request Introduction</p>](/articles/demo_project/DPM_Demo_Project/01_DSAR/01_00_DSAR.md)
