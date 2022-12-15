# Event-Based Alert

To understand how this provision works in case of Event-Based Alerts,  let’s consider that the user wants to create an alert notification to be shown when the value of a **‘Subject’** field of the case record changes. And later, user wants this alert to auto-dismiss once the case is resolved.

#### Steps to Auto-dismiss Alerts

* Navigate to **Advanced Settings** --> **Settings** --> **Process** --> **New Process**.

![](../../../.gitbook/assets/Event\_1.png)

* Select category as **‘Workflow’** and choose the **Entity** --> Click on **OK.**

![](../../../.gitbook/assets/Event\_2.png)

* Go to **‘Record fields change’** --> Select the field **‘Subject’** from the list.

![](../../../.gitbook/assets/Event\_3.png)

![](<../../../.gitbook/assets/Event\_4 (2).png>)

* Create a notification request record to create an alert.

![](<../../../.gitbook/assets/Event\_5 (1).png>)

* Select **‘Notification Request’.**

![](<../../../.gitbook/assets/Event\_6 (3).png>)

* Click on **‘Set Properties’**.

![](<../../../.gitbook/assets/Event\_7 (1).png>)

* Perform the dynamic field selection as required.

![](<../../../.gitbook/assets/Event\_8 (1) (1).png>)

* To display alert on the case record, set the **‘Notification Associated With’** as shown below:

![](../../../.gitbook/assets/Event\_9.png)

![](<../../../.gitbook/assets/Event\_10 (1).png>)

* After creating an alert, now add a **‘Wait’** condition which will wait till the case is resolved.

![](../../../.gitbook/assets/Event\_11.png)

![](<../../../.gitbook/assets/Event\_12 (1).png>)

Let’s further configure the condition.

![](../../../.gitbook/assets/Event\_13.png)

![](../../../.gitbook/assets/Event\_14.png)

* To auto-dismiss the alert once the case is resolved, select the row and add a new step as shown below:

![](../../../.gitbook/assets/Event\_15.png)

* Select the below assembly from the list for auto dismissing the alert notification.

<figure><img src="../../../.gitbook/assets/16 (3).png" alt=""><figcaption></figcaption></figure>

* Click on **‘Set Properties’.**

<figure><img src="../../../.gitbook/assets/17 (1).png" alt=""><figcaption></figcaption></figure>

* Select the below option from the list for **‘Look for’** field. This is a first step description that was added to create a notification request record.

![](../../../.gitbook/assets/Event\_18.png)

* Click on **‘Add’**.

![](../../../.gitbook/assets/Event\_19.png)

* Click on **‘OK’.**

![](../../../.gitbook/assets/Event\_20.png)

![](../../../.gitbook/assets/Event\_21.png)

* Click on **‘Save and Close’**.

![](../../../.gitbook/assets/Event\_22.png)

* Next, activate the workflow.

![](../../../.gitbook/assets/Event\_23.png)

![](../../../.gitbook/assets/Event\_24.png)

* Navigate back to **Case** --> **Open a case record** --> **Change** the value of the field **‘Subject’**.

![](../../../.gitbook/assets/event\_25.png)

* Change the subject from **‘Delivery’** to **‘Query’**.

![](../../../.gitbook/assets/Event\_26.png)

![](../../../.gitbook/assets/Event\_27.png)

* Click on **‘Save’.**

![](../../../.gitbook/assets/Event\_28.png)

* Once saved successfully, an alert will be shown as a **Dialog** on the case record. It will continue showing up until the case is resolved.

![](../../../.gitbook/assets/Event\_29.png)

* Now, let’s mark this case record as resolved.

![](../../../.gitbook/assets/Event\_30.png)

![](../../../.gitbook/assets/Event\_31.png)

![](../../../.gitbook/assets/Event\_32.png)

* Once the case is resolved, the alert is dismissed automatically.

![](../../../.gitbook/assets/Event\_33.png)

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

