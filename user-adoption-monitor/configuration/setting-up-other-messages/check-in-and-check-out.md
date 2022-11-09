# Check In & Check Out

With this feature you can keep track of records that each user worked on. It will specify the time spent by user on records in a particular Entity.&#x20;

{% hint style="info" %}
**Note: User Adoption Monitor Administrator or User Adoption Monitor User role is necessary to access Check-in/Check-out button.**
{% endhint %}

In order to enable Check-in & Check-out feature for a particular entity, follow the steps given below:

* First, you have to create action for the required entity. For each entity, you have to create separate actions. Go to **Advanced Settings --> Settings --> Processes.** Click on **New**.

![](../../../.gitbook/assets/Checkin\_1.png)

* Next, fill the required fields as follows:
  * **Process name:** Name the process, **for e.g. UAM-Case-CheckInCheckOut .**
  * **Category:** Select **‘Action’.**&#x20;
  * **Entity:** Select the required entity. Here ‘**Case’** entity is selected.
* Once the details are filled, click on **Ok.** Then **‘Activate’** the action as shown below:

![](../../../.gitbook/assets/Checkin\_2.png)

* Now, go to **Entity Configurations** (User Adoption Monitor group) --> Click on **New**.

![](../../../.gitbook/assets/Checkin\_3.png)

* Fill the required fields as follows:
  * **Entity Label:** Give name of required entity. For e.g., Case&#x20;
  * **Message:** checkincheckout. (After populating this field, you will get another lookup field – Action Name)
  * **Entity Schema:** incident&#x20;
  * **Period:** Select period i.e., Daily, Weekly or Monthly&#x20;
  * **Action Name:** Select the action created, for e.g., UAM-Case-CheckInCheckOut
* Click on **Save**.

![](../../../.gitbook/assets/Checkin\_4.png)

* Now go to a particular record in **Case** entity. Here, you will see the **Check-in** button. Click on the same before you start working on the record.

![](../../../.gitbook/assets/Checkin\_5.png)

* Once the task is completed, click on **Check-out** button. Both **Check-in & Check-out Buttons** are interchangeable.

![](../../../.gitbook/assets/Checkin\_6.png)
