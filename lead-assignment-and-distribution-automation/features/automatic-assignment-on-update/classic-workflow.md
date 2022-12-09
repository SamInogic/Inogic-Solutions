# Classic Workflow

To enable automatic assignments on the update, follow the steps given below:

* Create a workflow that will trigger on change of the field (e.g. Status Reason).

![](<../../../.gitbook/assets/Classic WF\_1.jpg>)

* If required add condition to check and run assignment only if your criteria meets. For the demo purposed, we had used condition to check if Status Reason is Ready.

![](<../../../.gitbook/assets/Classic WF\_2.png>)

* **Get the GUID of the record:** Add workflow assembly to get the GUID of the current record. Download and install [Dynamics 365 Workflow Tools Solution 1.0.60.1](https://github.com/demianrasko/Dynamics-365-Workflow-Tools/releases/tag/1.0.60.0) managed solution in your environment. This managed solution provides assembly called **‘msdyncrmWorkflowTools: Get Record ID’** to get the GUID of the record.

![](<../../../.gitbook/assets/Classic WF\_3.jpg>)

* You would need to pass the Record URL from current lead to Record URL parameter.

![](<../../../.gitbook/assets/Classic WF\_4.png>)

* This step will return the GUID of the current lead record.
* Call **‘Inogic.AddItemsToQueue’** action of Inogic --> Add **‘Perform Action’** step --> Select **‘Inogic.AddItemsToQueue’** action. This action is already available in the Lead Assignment and Distribution Automation solution.

![](<../../../.gitbook/assets/Classic WF\_5.jpg>)

![](<../../../.gitbook/assets/Classic WF\_6 (1).jpg>)

* Pass **PrimaryEntityName** and **PriamryEntityID** as Logical name of the entity e.g. lead, incident etc. and **‘GUID of the record return by the msdyncrmworkflow tools step’** respectively. This action will perform automatic assignment based on the Assignment Rules.&#x20;

![](<../../../.gitbook/assets/Classic WF\_7.jpg>)

* **Save and Activate** the workflow. The final workflow will look as below:

![](<../../../.gitbook/assets/Classic WF\_8.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
