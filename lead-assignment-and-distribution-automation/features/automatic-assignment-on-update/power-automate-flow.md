# Power Automate Flow

To enable automatic assignments on the update, follow the steps given below:

* Create a new Power Automate Flow and add **‘When a record is created, updated or deleted’** step of **‘Common Data Service (Current Environment)’** connector.

![](<../../../.gitbook/assets/Power Auto WF\_1.png>)

* Select **Trigger** condition (For example, Update).&#x20;
* Select entity for which you want to enable automatic assignment --> Select Scope as **‘Organization’.**&#x20;
* Based on the requirement add **Filtering attributes** and **Filter expression**. For Example, if you want to run the assignment on change of only **‘status reason’** field then add **‘statuscode’** as logical name of the field. The flow will trigger only on change of the **Status Reason** field.

![](<../../../.gitbook/assets/Power Auto WF\_2.png>)

* Add **‘Perform an unbound action’** step.

![](<../../../.gitbook/assets/Power Auto WF\_3.png>)

* Select **‘ikl\_InogicAddItemsToQueue’** in Action Name --> Enter **logical name** of your main entity in **Primary Entity** name --> Select unique identifier of the current record in **PrimaryEntityId.**

![](<../../../.gitbook/assets/Power Apps WF\_4.png>)

* **Save and test** the Power Automate flow.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

