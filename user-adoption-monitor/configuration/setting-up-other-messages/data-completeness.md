# Data Completeness

Using **‘Data Completeness’** you can ensure that the necessary data has been captured for an entity record in Dynamics 365 CRM as per the business requirement. Here, one shall choose the field(s) that are essential for an organization to be captured and ensure that data is within CRM. If it is not captured, then the status of that record will be shown as **‘Incomplete’**.

Follow the steps given below to configure **‘Data Completeness’**.

* Navigate to **Entity Configuration** --> Click on **New.**

![](../../../.gitbook/assets/Datacomp\_1.png)

* Fill the following fields:
  * **Entity Label:** Set the display name of the entity for which you want to configure datacompleteness. For example: Contact.&#x20;
  * **Entity Schema:** Set the logical name of the entity for which you want to configure datacompleteness. For example: contact.&#x20;
  * **Message:** datacompleteness (Once this field is set the ‘Period’ field will hide and the Attribute grid shows up).&#x20;
  * Select the attributes needed for completeness of data from the Attributes grid.
* Click on **Save** button over the **Attribute** grid as shown in the screenshot below:

![](../../../.gitbook/assets/Datacomp\_2.png)

* Once this entity configuration is saved, an Optionset type of field with the below details gets created for the entity for which datacompleteness has been configured.&#x20;
  * **Display Name:** Completeness Logical&#x20;
  * **Name:** ikl\_completeness&#x20;
  * **Data Type:** Optionset&#x20;
  * **Options:** Complete & Incomplete
* Now every time the record of the entity (for which datacompleteness has been configured) gets created or updated, the process shall check the existence of value in the fields which have been selected for completeness. If the value is present in all those fields then the value of the custom option set field **i.e. the ikl\_completeness** gets set as **Complete** or else it will be set as **Incomplete**.

{% hint style="info" %}
**Note: Whether to add this custom field on the form or view is totally up to the administrators of the respective organizations, and will have to be done manually. Also, it is imperative to remove this field from the forms or views before deleting the datacompleteness entity configuration.**
{% endhint %}

### Data Completeness for History Records

The records created after the configuration of Data Completeness entity can be tracked and monitored to ensure that all the defined fields in the records are duly filled. But this is not applicable for the already existing records in CRM. In order to check the completeness of the history records one has to create a separate on-demand workflow and run the same for these history records.&#x20;

Follow the steps given below to create workflow to monitor the completeness of History records:

* Navigate to **Advanced Settings --> Settings --> Processes.**

![](../../../.gitbook/assets/Datahis\_1.png)

* Select **New** --> Set the following fields --> Click on **OK**.
  * **Category:** Workflow.&#x20;
  * **Entity:** Select the entity for which the datacompleteness has been configured and the completeness of the history records that needs to be monitored.

![](../../../.gitbook/assets/Datahis\_2.png)

* Select **‘As an on demand process’** --> Select scope as **Organization** --> Click on ‘**Add Step**’ to call User Adoption Monitor assembly.

![](../../../.gitbook/assets/Datahis\_3.png)

* Select **‘Inogic.User.Adoption.Actions (1.0.0.0.)’ -->** Select **‘Inogic.User.Adoption.Actions.Execute.DataCompleteness’**.

![](../../../.gitbook/assets/Datahis\_4.png)

* Click on **Save** and then activate the process.

![](../../../.gitbook/assets/Datahis\_5.png)

* Navigate to any of the records of the configured entity --> Go to **Flow** --> Click on newly created workflow.

![](../../../.gitbook/assets/Datahis\_6.png)

![](../../../.gitbook/assets/Datahis\_7.png)

* Once the workflow has run the value of the **Completeness** field shall get set.

![](../../../.gitbook/assets/Datahis\_8.png)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
