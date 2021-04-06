## Case Owner Reviews Results

When we built the tutorial flow that fulfills the DSAR request, we defined that the task following the Legal team review would be the Case Owner review. 

The Case Owner review can be done very similarly to the review by the Legal data steward: The Case Owner user can be given Data Steward access privileges and can complete its  task in the same way that the Legal Data Steward performed that. Here, however, we would like to demonstrate another option that allows the Case Owner to access the task and complete it by using the Case Owner screens. 

For this, login to the DPM with a Case Owner user used in the Case Owner View step: 

- user: caseowner
- password: k2view

From the left menu, select the Requests List option

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Menu.png" width="30%" height="30%">

The table with the submitted requests is presented. Select the request created in the previous steps. In the example below, it is the top request in the table. The red circle next to the request status indicates that this request includes at least on task which is overdue: 

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Requests_List.png" width="100%" height="100%">

Once you clicked the selected request line, the request details screen is presented. This view provides the Case Owner the overall view of the Request progress, as well as additional information such as  which tasks contain notes - marked with a <img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Notes_icon.png" width="5%" height="5%"> icon in the Notes column. 

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Request_Details.png" width="100%" height="100%">

Click on the line of the "Case Owner Review" task. The Task Details screen is presented. This screen is the same as the Task Details screen of the Data Steward. 

<img src="/articles/demo_project/DPM_Demo_Project/images/02_04_DSAR_Fulfillment_Case_Owner_Review_Task.png" width="100%" height="100%">

The Case Owner actions in this screen are the same actions as described for the Legal Data Steward Task handling:

Use the <img src="/articles/demo_project/DPM_Demo_Project/images/02_03_DSAR_Fulfillment_Steward_Get_Task.png" width="3%" height="3%"> button at the top right of this screen in order to take ownership on the task. Review the information that was provided. 

Compare the data that was collected by the DPM with the data in the source systems for the requesting customer. 

Once you confirmed the data correctness, click on the <img src="/articles/demo_project/DPM_Demo_Project/images/02_03_DSAR_Fulfillment_Complete_Task.png" width="10%" height="10%"> in order to signal the system to move the request to the next task in the fulfillment process

Close the Task Details screen and logout from the DPM. 

[![Previous](/articles/images/Previous.png)](/articles/demo_project/DPM_Demo_Project/02_DSAR_Fulfillment/02_03_DSAR_Fulfillment_Steward_View.md)[<img align="right" width="60" height="54" src="/articles/images/Next.png">](/articles/demo_project/DPM_Demo_Project/02_DSAR_Fulfillment/02_05_DSAR_Fulfillment_Customer_View_Completed_Request.md)
