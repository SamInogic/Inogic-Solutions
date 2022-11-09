# Auto Create Folder

This feature allows users to create folder structure in the respective SharePoint Site with the help of workflow. The **‘Auto Create Folder’** field on the entity configuration form serves this purpose.

![](<../../.gitbook/assets/Auto Create Folder\_1.1.png>)

By default the field is set to **‘No’**. The user has to select **‘Yes’** from the dropdown of Auto Create Folder to create folder structure in SharePoint Site. To create the folder automatically, the user has to first create a workflow or can use Power Automate as well and call the **AutoCreateFolderStructure** action.&#x20;

Follow the steps given below to create a workflow.

* Navigate to **Advance settings** --> **Processes** --> Select **‘+New’.**

![](<../../.gitbook/assets/Auto Create Folder Workflow\_1.1.png>)

* Give an appropriate name to the workflow --> For **‘Category’** select **‘Workflow’** --> Choose the entity for which you want to create folders automatically --> Click on **Ok.**

![](<../../.gitbook/assets/Auto Create Folder Workflow\_2.png>)

* As per business requirement this workflow can be run for different events.

![](<../../.gitbook/assets/Auto Create Folder Workflow\_3.1.png>)

* Next, select **Perform Action** step.

![](<../../.gitbook/assets/Auto Create Folder Workflow\_4.1.png>)

* Then from the dropdown select the **AutoCreateFolderStructure** action as shown below:

![](<../../.gitbook/assets/Auto Create Folder Workflow\_5.1.png>)

* Click on **Set Properties** --> Select **Account** and **Record URL(dynamic)** in the **‘Look for’** section --> Click on **Save and Close**.

![](<../../.gitbook/assets/Auto Create Folder Workflow\_6.1.png>)

* **Activate** the workflow.

![](<../../.gitbook/assets/Auto Create Folder Workflow\_7.1.png>)

Once the workflow is activated, based on the triggering event the record would be created in SharePoint. By Auto Create folder feature user will be able to create folder in the SharePoint without hitting the **Attach2Dynamics button** or **Documents tab**.
