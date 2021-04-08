## Case Owner Reviews Results

When we built the tutorial Flow that fulfills the DSAR Request, we defined that the Task following the Legal team review would be a Case Owner review. 

The Case Owner review can be performed similarly to the review by the Legal Data Steward. The Case Owner user can be given Data Steward access privileges and can complete a Task in the same way that the Legal Data Steward completed one. However, we will demonstrate another option that allows the Case Owner to access the Task and complete it by using the Case Owner screens. 

For this tutorial, login to the DPM system as the same Case Owner user from the Case Owner View step. 

- **username**: caseowner
- **Password**: k2view

From the left menu, select the **Requests List** option.

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Menu.png" width="30%" height="30%">

The table with the submitted Requests displays. Select the Request created in the previous steps. In the example below, it is the top Request in the table. The red circle next to the Request status indicates that this Request includes at least one Task that is overdue.

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Requests_List.png" width="100%" height="100%">

Once you clicked the selected Request, the Request details screen displays. This view provides the Case Owner with the overall view of the Request progress, as well as additional information, including which Tasks contain notes. A Task that contains notes is marked with a <img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Notes_icon.png" width="5%" height="5%"> icon in the **Notes** column. 

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Request_Details.png" width="100%" height="100%">

Click the line of the **Case Owner Review** Task. The Task details screen displays. This is the same Task details screen as the one used for the Data Steward. 

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Task.png" width="100%" height="100%">

The Case Owner actions on this screen are the same actions described for the Legal Data Steward Task handling.

Use the <img src="/articles/demo_project/DPM_Demo_Project/images/02_03_DSAR_Fulfillment_Steward_Get_Task.png" width="3%" height="3%"> button at the top-right of this screen to take ownership of the Task. Review the information that was provided. 

Compare the data that was collected by the DPM system with the data in the source systems for the requesting customer. 

Once you confirm the data is correct, click <img src="/articles/demo_project/DPM_Demo_Project/images/02_03_DSAR_Fulfillment_Complete_Task.png" width="10%" height="10%"> to prompt the system to move the Request to the next Task in the fulfillment process.

Close the Task details screen and logout from the DPM. 



[![Previous](/articles/images/Previous.png)](/articles/demo_project/DPM_Demo_Project/02_DSAR_Fulfillment/02_03_DSAR_Fulfillment_Steward_View.md)[<img align="right" width="60" height="54" src="/articles/images/Next.png">](/articles/demo_project/DPM_Demo_Project/02_DSAR_Fulfillment/02_05_DSAR_Fulfillment_Customer_View_Completed_Request.md)
