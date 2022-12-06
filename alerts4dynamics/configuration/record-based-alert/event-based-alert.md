# Event-Based Alert

Event-Based Alerts are used to show an alert with respect to any event that happens in the CRM.&#x20;

For example, the user wants an alert notification to be shown to all users in CRM once a new **Account** or **Lead** record is created. In order to achieve this, the user has to follow the steps given below:

* Enable entity configuration for **‘Account’** entity.&#x20;

![](<../../../.gitbook/assets/Event\_1 (1).png>)

* Navigate to **Advanced Settings --> Processes --> Create New process**.

![](<../../../.gitbook/assets/Event\_2 (2).png>)

* Fill the following details and click on **OK**.&#x20;
  * Enter a relevant name for the process •
  * Select the category as **‘Workflow’** and Entity as ‘**Account**’.

<figure><img src="../../../.gitbook/assets/3 (12).png" alt=""><figcaption></figcaption></figure>

* Select the event on which you want the notification to created.

![](../../../.gitbook/assets/Event\_4.png)

* Now create a record of **‘Notification Request’.** For this, select **Add Step** --> **Create Record** --> Select **‘Notification Request’** from the dropdown.

![](../../../.gitbook/assets/Event\_5.png)

* Click on **‘Set Properties’**.&#x20;

![](../../../.gitbook/assets/Event\_6.png)

* Fill in the following details:&#x20;
  * **Name –** Enter some valid name for the Notification Request record.&#x20;
  * **Message Text –** Enter some valid text (You can also select dynamic value).&#x20;
* Select the above field and click on **‘Add’** button to add it in the Message Text field.

![](<../../../.gitbook/assets/Event\_1 (2).png>)

* Click **OK**. You will see the dynamic value is set to the **‘Message Text’** field. Similarly add Dynamic values in **‘Name’** field.
* **Message Rich Text -** Select the appropriate Message Rich Text from the lookup. for this type of message to appear in the lookup users need to create these messages before creating an Event-Based Alert.

{% hint style="info" %}
**Note: Message Rich Text gives users provisions to create more interactive messages by doing all kinds of text formatting, adding links and images, etc., to make their messages more descriptive and engaging.**
{% endhint %}

* To create and add **Message Rich Text** in an **Event-Based Alert** follow the steps given below:
* Navigate to **Alerts4Dynamics App -->  Message Texts -->** Click on the **'New'** Button**.**

<figure><img src="../../../.gitbook/assets/Message Rich Text 1.png" alt=""><figcaption></figcaption></figure>

* Fill in the following details:
  * **Name -** Provide an appropriate name for the Message Rich Text.
  * **Message Rich Text -** Enter some valid text and do the desired text formatting to create Message Rich Text that will be shown on the notification.
* Click on **'Save'.**

<figure><img src="../../../.gitbook/assets/Message Rich Text 2.png" alt=""><figcaption></figcaption></figure>

* Once you have created the message

{% hint style="info" %}
**Note:**&#x20;

* **If both Message Text and Message Rich Text fields are filled, then preference will be given to Message Rich Text when displaying the notification.**
* **Message Rich Text cannot be displayed as a bar in a form notification.**&#x20;
{% endhint %}

* Fill in the following details:&#x20;
  * **Alert As** - Pop up (To display an alert in the form of pop up notification)&#x20;
  * **Alert Level** - Warning/Critical/Informational depending on user’s requirement&#x20;
  * **For Notification Associated With Field** - You will have to select a dynamic record URL of the entity on which you want to show the notification. In this scenario, we want a notification to be shown on the Account entity, so we will select the Record URL of the Account entity.
* Click on **‘Add’.**

![](<../../../.gitbook/assets/Event\_2 (4).png>)

* For the **‘Notification Audiences’** you can select dynamic users like **Owning User** of the record as well as the **Manager of the Owning User** as shown in **Include Users** field.

![](<../../../.gitbook/assets/Event\_8 (2).png>)

* Once details are filled, click on **‘Save and Close’** and then activate the workflow by clicking **‘Activate’** button.

![](../../../.gitbook/assets/Event\_9.png)

To know more about Event-Based Alert, please [click here.](https://docs.inogic.com/alerts4dynamics/features/event-based-alert)



{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
