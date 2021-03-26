# Associate DSAR Flow to Activity of a Specific Regulation

In the previous steps we have configured the Flow that performs the tasks to retrieve customer data.

For this flow to become visible to a customer who wants to submit a request, it should be associated with an Activity, under a specific regulation. You can read more details about [Regulations](articles/DPM/02_Admin_Module/08_Regulations.md) and [Activities](/articles/DPM/02_Admin_Module/09_Activities.md) at the DPM User Guide. 

We will now create a new Regulation, add under it a new Activity, and then we will associate the "DSAR Tutorial" Flow. 

1. Select the menu option "Regulation List"

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Admin_Menu_Regulation.png" width="30%" height="30%">

2. use the <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_New_Regulation_Icon.png" width="10%" height="10%"> to create a new Regulation. Populate the information for this new Regulation as presented below. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Regulations_List.png" width="100%" height="100%">

Once you saved the new Regulation, the screen of the Activities for this Regulation is presented, initially empty as no Activity was created yet. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_Empty_Regulation.png" width="100%" height="100%">

3. Select the <img src="/articles/demo_project/DPM_Demo_Project/images/01_03_DSAR_New_Activity_Icon.png" width="10%" height="10%"> in order to add a new Activity under this Regulation. Populate the information for this new Activity as presented below, selecting for the Flow field the DSAR Tutorial Flow which was created in the previous steps. 

![image](/articles/demo_project/DPM_Demo_Project/DPM_Demo_Project/images/01_03_DSAR_New_Activity.png)

Saving the new Activity makes the new flow we created available for customers to submit requests based on it.  The execution of such requests is described in the next section of this tutorial: [DSAR Request Execution](). 

  

