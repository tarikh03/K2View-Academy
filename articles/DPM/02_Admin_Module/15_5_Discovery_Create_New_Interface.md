## Add an Interface

Click the ![image](/articles/DPM/images/Figure_85_Discovery_AddInterface.jpg) button at the top-right of the screen in order to configure a new Interface.

![image](/articles/DPM/images/Figure_87_Discovery_AddInterface_Callout.jpg)

The following dialog box displays.

![image](/articles/DPM/images/Figure_81_Discovery_NewInterface.jpg)

<table>
<tbody>
<tr>
<td width="85">
<p><strong>Property</strong></p>
</td>
<td width="785">
<p><strong>Description</strong></p>
</td>
</tr>
<tr>
<td width="85">
<p> Interface</p>
</td>
<td width="785">
<p>Select an interface from the drop-down list. For example, select “dbsalesforce”. This list is populated by options configured in the DPM fabric software. </p>
</td>
</tr>
<tr>
<td width="85">
<p>Catalog Pattern (Regex)</p>
</td>
<td width="785">
<p>Information Needed</p>
</td>
</tr>
<tr>
<td width="85">
<p>Schema Name Inclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>All tables in the database are defined in the Schema part of the DPM fabric software Creator Interface. For example, for a new Interface called “dbsalesforce”, select “SFORCE” from the Schema Name Inclusion Pattern drop-down list.</p>
</td>
</tr>
<tr>
<td width="85">
<p> Probability (1 – 100%)</p>
</td>
<td width="785">
<p>Set the probability  percentage of the new Matching Rule. For example, when you validate a social  security number, the 9-digit number could be an account number of the same  format. Therefore, the Probability would be lower (ex: 70%).</p>
</td>
</tr>
<tr>
<td width="85">
<p>Schema Name Exclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>All tables in the database are defined in the Schema part of the fabric software Creator Interface. For example, for a new Interface called “dbsalesforce”, select “PUBLIC” from the Schema Name Exclusion Pattern drop-down list.</p>
</td>
</tr>
<tr>
<td width="85">
<p>Table Name Inclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>Refine your search further by telling the system to include specific tables. For example, you can include the database tables for all instances of “ACCOUNT.” </p>
</td>
</tr>
<tr>
<td width="85">
<p>Table Name Exclusion Pattern (Regex)</p>
</td>
<td width="785">
<p>Refine your search further by telling the system to exclude specific tables. For example, you can exclude searching the database tables for all instances of “ACCOUNT.” </p>
</td>
</tr>
<tr>
<td width="85">
<p>Active</p>
</td>
<td width="785">
<p>The “Active” slider is turned to “On” by default. Turn the slider to “Off” if you do not want the new Interface to be active in the table.</p>
</td>
</tr>
</tbody>
</table>

###  Edit or Delete an Interface

Use the ![image](/articles/DPM/images/ICON_Delete.jpg) button to delete an Interface. 

**Note**: If you click the ![image](/articles/DPM/images/ICON_Delete.jpg) button, the system displays a dialog box, prompting “Are you sure you want to Delete Interface: [InterfaceName]?” Click the ![image](/articles/DPM/images/08_ICON_OK.png) button to remove the selected Interface from the system.

Click the ![image](/articles/DPM/images/ICON_Edit.jpg) button to edit the Interface name, Schema information, and table information.



[![Previous](/articles/DPM/images/Previous.png)]( /articles/DPM/02_Admin_Module/15_4_Discovery_Interfaces_Overview.md)[<img align="right" width="60" height="54" src="/articles/demo_project/DPM_Demo_Project/images/Next.png">](/articles/DPM/02_Admin_Module/15_6_Discovery_Submit_Discovery_Request.md)