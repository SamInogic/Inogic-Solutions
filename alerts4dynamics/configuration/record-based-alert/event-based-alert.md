# Event-Based Alert

Event-Based Alerts are used to show an alert with respect to any event that happens in the CRM.&#x20;

For example, the user wants an alert notification to be shown to all users in CRM once a new **Account** or **Lead** record is created. In order to achieve this, the user has to follow the steps given below:

* Enable entity configuration for **‘Account’** entity.&#x20;

![](<../../../.gitbook/assets/Event\_1 (2).png>)

* Navigate to **Advanced Settings --> Processes --> Create New process**.

![](../../../.gitbook/assets/Event\_2.png)

* Fill the following details and click on **OK**.&#x20;
  * Enter a relevant name for the process •
  * Select the category as **‘Workflow’** and Entity as ‘**Account**’.

<figure><img src="../../../.gitbook/assets/3 (20).png" alt=""><figcaption></figcaption></figure>

* Select the event on which you want the notification to created.

![](<../../../.gitbook/assets/Event\_4 (2).png>)

* Now create a record of **‘Notification Request’.** For this, select **Add Step** --> **Create Record** --> Select **‘Notification Request’** from the dropdown.

![](<../../../.gitbook/assets/Event\_5 (2).png>)

* Click on **‘Set Properties’**.&#x20;

![](../../../.gitbook/assets/Event\_6.png)

* Fill in the following details:&#x20;
  * **Name –** Enter some valid name for the Notification Request record.&#x20;
  * **Message Text –** Enter some valid text (You can also select dynamic value).
* Select the above field and click on **‘Add’** button to add it in the Message Text field.

![](<../../../.gitbook/assets/Event\_1 (1).png>)

* Click **OK**. You will see the dynamic value is set to the **‘Message Text’** field. Similarly add Dynamic values in **‘Name’** field.
* Fill in the following details:&#x20;
  * **Alert As** - Pop up (To display an alert in the form of pop up notification)&#x20;
  * **Alert Level** - Warning/Critical/Informational depending on user’s requirement&#x20;
  * **For Notification Associated With Field** - You will have to select a dynamic record URL of the entity on which you want to show the notification. In this scenario, we want a notification to be shown on the Account entity, so we will select the Record URL of the Account entity.
* Click on **‘Add’.**

![](<../../../.gitbook/assets/Event\_2 (3).png>)

* For the **‘Notification Audiences’** you can select dynamic users like **Owning User** of the record as well as the **Manager of the Owning User** as shown in **Include Users** field.

![](../../../.gitbook/assets/Event\_8.png)

* Once details are filled, click on **‘Save and Close’** and then activate the workflow by clicking **‘Activate’** button.

![](<../../../.gitbook/assets/Event\_9 (1).png>)

To know more about Event-Based Alert, please [click here.](https://docs.inogic.com/alerts4dynamics/features/event-based-alert)

