# Word Template Workflow

Click2Export enables exporting of Dynamics CRM Word Templates using Click2Export workflow.&#x20;

Follow the steps given below to export word templates using workflow:

* Navigate to **Settings > Processes** and click on ‘**New**’ to create a new workflow.

![](<../../../.gitbook/assets/1 (206).png>)

* Enter the ‘**Process Name**’, select the ‘**Category**’ as ‘**Workflow**’ and ‘**Entity**’ for which you want to create this workflow. Click on ‘**OK**’.

![](<../../../.gitbook/assets/2 (47).png>)

* Here you can select whether you want the Workflow to be On Demand or trigger on a change of Options for Automatic Processes.

<figure><img src="../../../.gitbook/assets/27.2 pending.PNG" alt=""><figcaption></figcaption></figure>

* First user needs to click on **‘Add Step’** and add **Perform Action** step that is predefined by Microsoft to select the appropriate **Action** for required word template. Select **Action** as **SetWordTemplate** option and **Entity** as **None** (global).&#x20;

![](<../../../.gitbook/assets/4 (2) (1).png>)

* Now click on **‘Set Properties’** of **Perform Action** step and select the required Word Template in **SelectedTemplate** section and required **Entity** in **Target** section. In order to select the required entity in Target section, it should have **Business Process Flows** ticked in the entity settings like shown below:&#x20;

![](<../../../.gitbook/assets/C2E\_Word Workflow - Copy.png>)

![](<../../../.gitbook/assets/5 (19).png>)

* Click2Export ships with one workflow assembly namely ‘**Inogic.Click2Export.ExportWord.ExportWord2PDF**’. This step is required to call the workflow for performing the selected action.
* Now click on ‘Set Properties’ for **Inogic.Click2Export.ExportWord.ExportWord2PDF**&#x20;

![](<../../../.gitbook/assets/6 (21).png>)

* Once the properties window opens, fill in the correct details as explained below:

<figure><img src="../../../.gitbook/assets/27.1 pending.PNG" alt=""><figcaption></figcaption></figure>

**Document Template:** Select the document that needs to be converted to PDF.

**CRM Report Template:** This will be the Report Template that has been created for the Document Template selected above.

**Attach as a Notes:** If marked as True, then it will attach the converted PDF against the record as a Note else it will not.

**Attach to an Email:** If marked as True, then it will attach the converted PDF in an email. The **Email Recipients** and the **Sender** would be selected based off the **Email Configuration** done on the selected **CRM Report Template**.

**Upload to SharePoint:** If marked as True, the converted file will be uploaded against the record’s respective SharePoint folder.

* Now ’**Save**’  and then ‘**Activate**’ the process.
* You can now see the workflow in ‘**My Processes**’.

![](<../../../.gitbook/assets/8 (5).png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

