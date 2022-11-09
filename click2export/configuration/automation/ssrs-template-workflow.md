# SSRS Template Workflow

Click2Export supports exporting the Dynamics CRM Report Templates using Click2Export workflow.&#x20;

Given below are the steps to export reports through automation:

* Navigate to **Settings > Processes** and click on ‘**New**’ to create a new workflow.

![](<../../../.gitbook/assets/1 (268).png>)

* Enter the ‘**Process Name**’, select the ‘**Category**’ as ‘**Workflow**’ and ‘**Entity**’ for which you want to create this workflow. Click on ‘**OK**’.

![](<../../../.gitbook/assets/2 (30).png>)

* Here you can select whether you want the **Workflow** to be **On Demand** or trigger on a change of Options for Automatic Processes.

![](<../../../.gitbook/assets/3 (28).png>)

* First user needs to click on ‘**Add Step**’.  Click2Export ships with one workflow assembly namely ‘**Inogic.Click2Export.ExportReport.ExportAndScheduleReports**’. This step is required to call the workflow for performing the selected action.

![](<../../../.gitbook/assets/4 (7).png>)

* For **On-Premises**, the work flow assembly will be as follows:

![](../../../.gitbook/assets/SSRS\_7.jpg)

* Now click on ‘**Set Properties**’ for **Inogic.Click2Export.ExportReport.ExportAndScheduleReports**

![](<../../../.gitbook/assets/5 (11).png>)

* Once the properties window opens, fill in the correct details as explained below:

![](<../../../.gitbook/assets/1 (117).png>)

**CRM Report Template:** CRM Report Template for the SSRS report that you want to be converted.

**Attach as a Notes:** If marked as True, then it will attach the converted file against the record as a Note else it will not.

**Attach to an Email:** If marked as True, then it will attach the converted file in an email. The **Email Recipients** and the **Sender** would be selected based off the **Email Configuration** done on the selected **CRM Report Template.**

**Upload to SharePoint:** If marked as True, the converted file will be uploaded against the record’s respective SharePoint folder.

* For **On-Premises**, it will be as follows:

![On-Premises](../../../.gitbook/assets/SSRS\_8.jpg)

* Now ’**Save**’  and then ‘**Activate**’ the process.
* You can now see the workflow in ‘**My Processes**’.

![](<../../../.gitbook/assets/6 (4).png>)
