# Create Tasks in the First Stage

We will now create few Tasks within the new Stage you have created in the previous step, in order to exemplify how a Flow is constructed. When configuring a Flow for your company, the actual tasks you create will naturally vary.

The tasks we will create are: 

- **Check Case Duplication** - a task that validates if there is already an open request of the same type for the same customer. If there is such request, the new request will be stopped and a message sent to the customer

- **Get Customer ID**  - in this task, the system identifies the unique ID that represents the customer who submitted the request, in each one of the systems integrated with the DPM, so that it can retrieve the data from each system. In our tutorial, those systems are Odoo and Open Source Billing.

- **Send notification mail to the customer** - once the request was validated and the customer identified, send a message to the customer to inform the request is being processed and the expected due date. 

  We assume you are now looking at the screen showing the new DSAR Tutorial Flow created in the previous step.

  ### Check Case Duplication

This task is an automatic task that verifies if the customer already has another request of the same type which is in process. 

1.  In the screen of the DSAR Tutorial Flow  select <img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_New_Task_Icon.png" width="5%" height="5%"> the at the right side of the window, in order to add a new Task:

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Check_Case_Duplication.png" width="100%" height="100%">

2. Populate the fields in this window in the same way shown in the image above. As this is going to be an automatic activity, we set the Role to be "Case Owner". If the automatic process fails for some reason, it will be the Case Owner of this request who will receive the failure notification. Note that the Task order was set automatically to 1 as this is the first task you created. The order can be changed later on if needed.

3. Move to the "Operations" tab of the Task configuration screen, and select caseCheckIfDuplicate from the operations drop down, as shown below. The caseCheckIfDuplicate is a built in operation which performs the Duplicate Case validation. The DPM includes a long list of such automatic operations, and any other operation that is specific for your project can be created to meet your needs.

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Check_Case_Duplication_operations.png" width="100%" height="100%">

4. The first Task is ready! Save the Task and you will be directed back to the Flow screen, where you can continue and add the following Tasks. 

   <img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Flow_One_Task.png" width="100%" height="100%">

### Get Customer ID

The second task is configured similarly to the first. It demonstrates how to set a Task to run in parallel to another task.

1. Add a new Task, and call it Get Customer ID. Assign the Role to be case owner again. 
2. Note that the system automatically suggests the order of this task to be 2, since this is the second task you have created. Set the task order to be 1, so that it will be executed in parallel with the first task.

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_get_customer_id.png" width="80%" height="80%">

3. At the Operations tab, select the automatic operation getCaseCustomerId

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_get_customer_id_operations.png" width="80%" height="80%">

4. Save the new task. 

### Send notification mail to the customer

This third task is the last we will configure under the first Stage. It will demonstrate how to configure operations parameters. 

1. Add a new task and give it the name: Send notification mail to the customer. 
2. The system automatically suggests that this task order will be 2, meaning it will run after the first two tasks were completed (they are order 1).

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Send_notification_mail.png" width="80%" height="80%">

3. in the operations tab, select the automatic operation SendNewCaseCreationEmail. As you can see below, this operation requires few inputs for its execution:

   - The customer ID, which can be obtained from the previous task "Get Customer ID" output

   - The customer email to which the mail should be sent. We will configure the task so that this information will be collected from the customer at the request submission moment

   - Indicator whether the case is duplicate, in order to inform the customer case the request is rejected on this base. We will get this information from the previous task "Check Case Duplication" output

   - If the request was identified as duplicate - what is the ID of the request that is already open. This information we too get from the previous task output.

     <img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Send_notification_mail_operations_empty.png" width="80%" height="80%">

Use the example below in order to select from the dropdown of each of the parameters types. The additional dropdowns for each line will be presented as you select the input type for each parameter.

​			<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_Send_notification_mail_operations.png" width="80%" height="80%">

4. Save the new task. 

<img src="/articles/demo_project/DPM_Demo_Project/images/01_02_02_DSAR_first_stage_complete.png" width="100%" height="100%">