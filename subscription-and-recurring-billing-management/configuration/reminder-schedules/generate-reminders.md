# Generate Reminders

You can send reminder emails for the Invoices/Orders due. The reminder emails get sent referring the Reminder Rules associated to the Reminder Schedule which is associated to the Invoice/Order which is carried over from the associated Subscription Schedule.

You can either automate the process by creating workflow trigger record which we shall see in the [workflow trigger](https://docs.inogic.com/subscription-and-recurring-billing-management/features/workflow-triggers) section or go by the ad-hoc way of sending the reminder i.e., by manually running the on demand workflow on the Invoice or Order.

The workflow on Invoice is named '**SM - Generate Reminders for Invoices'**.&#x20;

The workflow on Order is named '**SM - Generate Reminders for Orders'**.

To run the workflow kindly follow the below steps:

* Navigate to **Subscription and Recurring Billing Management App --> Invoices/Orders --> Open the record of an Invoice/Order.**&#x20;
* Go to Ribbon bar --> Click on **Flow.**&#x20;
* Click on **‘SM - Generate Reminders for Invoices’** workflow if you are on Invoice record, Or Click on **‘SM - Generate Reminders for Orders’** workflow if you are on Order record.

![](../../../.gitbook/assets/Reminder\_5.png)

* A dialog box will appear --> Click on **OK.**

![](../../../.gitbook/assets/Reminder\_6.png)

* The workflow is now triggered and an email shall be generated shortly which can be seen in the timeline under the Details tab on the respective form.

{% hint style="info" %}
**Note: These workflows stay in draft state which the user needs to activate after importing the solution.**
{% endhint %}

### How to activate the workflow:

* Click on the **Gear** icon.
* Open **Advanced Settings.**
* Navigate to **Settings --> Process.**
* In the Search box type **‘**_**reminder**_**’.**
* Select and open the workflow – **‘SM - Generate Reminders for Invoices’.**

![](../../../.gitbook/assets/Reminder\_7.png)

* Click on the **‘Set properties’** of the Document template.

![](../../../.gitbook/assets/Reminder\_8.png)

* Click on **Save & Close.**

![](../../../.gitbook/assets/Reminder\_9.png)

* Click on **Activate** Button.

![](../../../.gitbook/assets/Reminder\_10.png)
