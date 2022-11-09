# Workflow Triggers

In simple words the basic purpose of this entity is to automate the processes, be it the billing process or the reminder process or delayed charge process. A workflow trigger record must be created for each automation process.&#x20;

### How to create a Workflow Trigger record:

* Navigate to **Subscription and Recurring Billing Management App --> Workflow Triggers --> Click on the ‘New’ button.**
* Fill in the values as shown below and create the Workflow trigger record.
  * **Workflow Trigger Name:** The name of the workflow trigger record.&#x20;
  * **Description:** Details to explain the purpose of this Workflow Trigger.&#x20;
  * **Poll Interval:** Set the polling duration for the automation be it X Day(s), X Week(s), X Month (s) or X Year(s).&#x20;
  * **Interval:** This field goes in conjunction with the field **Poll Interval** where the **X** in the option selected is the value set in the Interval.&#x20;
  * **Workflow Options:** Select the option based on what you want to automate. The options available for this field and their purpose are as below:
    * **Auto Generate Document:** To automate the billing process of generating the Invoices/Orders from Subscription Schedule.&#x20;
    * **Auto Generate Reminder:** To automate the process of generating a reminder to notify your Invoice/Order due.&#x20;
    * **Auto Generate Delayed Charge:** To automate the process of levying penalty charge past invoice due.&#x20;
    * **Auto Generate Renewal Reminder:** To automate the process of generating a reminder to notify customers and owner of subscription schedule about subscription renewal.
    * **Other:** To automate any process using custom workflow. By selecting this option, a lookup field named **'Workflow'** pointing to the Process entity shows up from where you can select your own active process. But the process has to be created on the Workflow Trigger entity itself.
  * **Workflow Start Time:** The preferred date and time from when you want to start the process to automate the respective process.

{% hint style="info" %}
**Note: Select the workflow that has been created for the entity 'Workflow Trigger' only.**
{% endhint %}

![](<../../.gitbook/assets/Work Trig\_1.png>)

![](<../../.gitbook/assets/Work Trig\_2.png>)
