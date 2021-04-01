# DSAR Fulfillment Process

In the previous section of this tutorial, we prepared the Flow that executes the fulfilment process of a Data Subject Access Request (DSAR) activity, and associated it to an Activity that can be requested by a customer.  

We can now demonstrate the fulfilment process itself, simulating the scenario where a customer access the DPM Customer User Interface, and submits a DSAR request. 

This section will take you through the steps this request follows from submission till its completion, based on the stages and tasks we configured in the previous section of this tutorial.

Remember that the tasks we created are only as an example. The actual sequence and content of tasks is fully configurable and in your project you can implement the process to fit your company needs.

So far in this tutorial, we demonstrated the activities of a user that holds the administrator role - such as configure new Flow, Regulation and Activity. As part of the customer request fulfillment flow you will be presented with some of the additional user roles that make part of the DPM tool, such as:

- **Customer** - customer is an example of a user that can submit data privacy related requests to the company. It could be a company customer, prospect, employee or any other end user about whom the company may hold data. 
- **Representative** -  This role is used by users such a call center representative or an internet bot, who responds to customer's calls or chats. A Representative can perform actions on behalf of the customer, submitting a DSAR request, report request status to a customer or alter the customer's consent preferences.
- **Data Steward** - This role can be associated with any user that performs back-office activities as part of the fulfillment process. In our example, we defined that the Legal team should review the data before sending it to the customer, so we defined the users of the legal team to a role that has data steward permission
- **Case Owner** - The Case Owner is the overall responsible for the timely execution of all customer's requests and can review the status of all tasks. In the example we created, in addition to the overall responsibility over the request, we also allocated to the Case Owner the task of final review, to demonstrate this scenario as well.



[![Previous](/articles/images/Previous.png)](/articles/demo_project/DPM_Demo_Project/README.md)[<img align="right" width="60" height="54" src="/articles/images/Next.png">](/articles/demo_project/DPM_Demo_Project/02_DSAR_Fulfillment/02_01_DSAR_Fulfillment_Customer_Request.md)