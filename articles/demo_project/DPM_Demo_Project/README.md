# DPM DEMO PROJECT 

## Introduction

We invite you to acquire a firsthand experience of our DPM application, by following the step-by-step demo guide we present below. 

This demo will take you through the main activities of implementing and using our DPM application, such as implementing a Data Subject Access Request flow, defining consents, executing PII discovery and more. 

This guide takes you through the set-up activities required to create your dedicated sandbox environment and the detailed steps of implementation and execution of various DPM features.

## Demo Project Presentation

In order to demonstrate the implementation of our DPM application, we first create an environment that simulate a real-world company, having multiple source systems which should be integrated with the DPM platform. To represent those source systems, the sandbox we generate for you includes two separate applications, each holding different information about the company customers. 

The two applications that represent the source systems in this demo were selected for the mare purpose of demonstrating concepts. In real-life implementation you will of course connect to whichever and as many source applications your company utilizes. 

Meet the demo “Source Systems”:

The two systems that we picked up to simulate source systems are:

- ![image](/articles/demo_project/DPM_Demo_Project/images/01_DSAR_Odoo.PNG) - Odoo is an open source ERP and CRM application. You can view more details about this application at their site: https://www.odoo.com/

- ![image](/articles/demo_project/DPM_Demo_Project/images/01_DSAR_opensourcebilling_icon.png) - Open Source Billing (OSB), as its name indicates, is an open source billing system. Access its site https://opensourcebilling.org/ for more information.


When you set up the demo environment, we automatically generate for you not only a running instance of each of those applications, but also populate it with the data of imaginary customers. This data will be used along the demo to demonstrate DPM features and functionality, such as customer matching between applications, fulfilment of data access requests, keeping up with data change scenarios and more.  

## Environment Setup 

Follow the link below in order to access the step-by-step instruction that will generate your dedicated sandbox environment:

Environment Setup 

## Demo Scenarios

Follow the links below in order to access the step-by-step instruction for the generation of  your dedicated sandbox environment

### Data Subject Requests

The first section of our demo takes you through the steps of implementing the automation and streamlining the fulfilment process of data access requests.

- [**Data Subject Access Request (DSAR)**](/articles/demo_project/DPM_Demo_Project/01_DSAR/01_00_DSAR.md) - By demonstrating how to create a DSAR request we will lead you through the implementation steps that allow you to define the flow and automation of any type of Data Subject request that Data Privacy regulations may require. 

- **Execute a DSAR** - In this demonstration, you will simulate the scenario of a customer who submitted a DSAR, and the flow this request goes through from submission to fulfillment. 

- **Seamless sync of source system changes** - By simulating a data change at one of the source systems and submitting a DSAR request for this customer, this section demonstrates the DPM seamless synchronization with the source systems.
- **Data Rectification** - The steps in this section simulate the scenario of  a customer submitting a request to rectify its data. As a result, DPM automatically updates the data in all relevant source systems and confirm when the request fulfilment is completed.
- **Anonymization Request** - Simulate a customer request to anonymize its data at all source systems, and follow this request to completion.
- **Data Deletion Request** -  Simulate a customer request to delete its data at all source systems, and follow this request to completion.

### Personally Identifiable Information (PII) Discovery

DPM PII discovery feature provides you with a powerful tool to identify the location personal data is stored at your organization's systems, in order to take the appropriate measures to protect it.

- **PII Discovery** - In this guided demo we take you through the steps of defining and executing the PII discovery process

### Customer Consent Management

Managing your customer's preferences and consents is made easy with DPM Consent Management capabilities

- Consent Management - this interactive demo demonstrate how to define any consent topic and the way the system manage the consent preferences of each customer. 
