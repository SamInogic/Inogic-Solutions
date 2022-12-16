# Special Messages

User Adoption Monitor supports the following special messages apart from the CRUD operations. You will find sample entity configurations created for these when you install the sample data.

| Entity Name | Message           | Description                                                                                 |
| ----------- | ----------------- | ------------------------------------------------------------------------------------------- |
| Lead        | Qualifylead       | This message is triggered when a lead is qualified.                                         |
| Opportunity | Win               | It is triggered when an opportunity is closed as Won.                                       |
| Quote       | Close             | Triggered when the quote is closed.                                                         |
| Quote       | Win               | It is triggered when the quote is won (Post clicking ‘Create Order’).                       |
| Incident    | Close             | This is triggered when an Incident is closed as Resolved.                                   |
| List        | AddListMembers    | This is triggered when a new member is added to a Static Marketing List.                    |
| Email       | Send              | This is triggered once an email is sent.                                                    |
| Application | loginlogout       | To track user log-in & log-out details.                                                     |
| Case        | \*checkincheckout | To keep track of user Check-in & Check-out activities details in particular Entity records. |

{% hint style="info" %}
**Note: 'checkincheckout' is applicable for OOB and custom entities – Lead, Opportunity, Quote, etc.**&#x20;
{% endhint %}

![](../../../.gitbook/assets/Sp\_Mess\_1.png)

#### Example for Entity Tracking

* First, enable tracking for the following entities:&#x20;
  * **For Account:** Set **‘Create’** to period **‘Daily’**&#x20;
  * **For Contact:** Set **‘Update’** to **‘Weekly’**&#x20;
  * **For Lead:** Set **‘Assign’** to **‘Monthly’**

![](../../../.gitbook/assets/Sp\_Mess\_2.png)

* Upon Save, you will be notified that the Tracking has been enabled/disabled for selected entities.

![](../../../.gitbook/assets/Sp\_Mess\_3.png)

* You can verify the configurations by navigating to the Entity Configuration section of User Adoption Monitor.

![](../../../.gitbook/assets/Sp\_Mess\_4.png)

{% hint style="info" %}
**Note: Through the User Adoption Tracking screen, you can only configure to monitor CRUD operations performed on entities. To monitor other actions performed by the user on the entities you need to create the User Adoption Entity Configuration Record manually.**
{% endhint %}

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
