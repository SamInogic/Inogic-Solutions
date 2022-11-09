# Round Robin Assignment

In this method, users are assigned Leads in sequence. For e.g. Consider there are 3 members in a team namely – A, B & C. With Round Robin method, the first Lead will be assigned to A, the second Lead to B, third Lead to C and the fourth Lead will be again assigned to A. In this sequence Leads will be assigned to the users.&#x20;

To assign Leads as per Round Robin method, follow the steps given below:

* Navigate to **Lead Assignment & Distribution Automation App --> Administration --> Assignment Configuration -->** Select the respective **Assignment Configuration -->** Click on **New Assignment Rule**.

![](<../../.gitbook/assets/Assign Config\_2.png>)

* Enter mandatory field details as illustrated below and click on **‘Save’.**

![](<../../.gitbook/assets/Round Robin\_1.png>)

* **Name:** Give name, for e.g. Leads from Website&#x20;
* **Assignment Configuration:** Select respective configured Entity, for e.g. Lead.&#x20;
* **Description:** Provide description, for e.g. Leads from Website.&#x20;
* **Criteria Mode:** Select between **‘Simple’** or **‘Advanced’** criteria mode. **‘Simple’** mode is based on **‘Views’** and **‘Advanced’** is based on **Fetch Xml**. Here, Advanced mode is selected.&#x20;
* **Execution Order:** Give numeric value, for e.g. **0**. If there are two or more Round Robin based Assignment Rules then this field states the order in which Rules are to be executed while assigning Leads.&#x20;
* **Queue:** Select the respective Queue.&#x20;
* **Consider Availability:** This field checks the availability status of users before assigning work items. Select **‘Yes’** or **‘No’.**
* **Assignment Algorithm:** Select between Round Robin and Capacity. Here we selected Round Robin.&#x20;
* **Max Work Items Allowed to be Assigned:** This field denotes the maximum number of work items that is allowed to be assigned to users. For example – 5. Here, each user will be assigned maximum 5 Leads.&#x20;
* **Period:** This is an option-set field with the following options - Daily, Weekly, Monthly and Overall. It defines the period for which the work items (Entity records) will be assigned to the users.
* **Open Work Item Statuses:** Select the status from the dropdown, for e.g. Open-New. Here, based on the status ‘Open-New’ Leads will be assigned to users. Once the Lead ‘s status changes from Open-New to another status then then that Lead will be considered as completed and automatically another Lead with status as ‘Open-New’ is assigned to the same user. This process will go on till all the Leads are assigned.

![](<../../.gitbook/assets/Round Robin\_2.png>)

![](<../../.gitbook/assets/Round Robin\_3.png>)

#### Updating of ‘Max Work Items Allowed to be Assigned’ field

It is quite easy to update the maximum number of work items allowed to be assigned to the users. Just go to the existing **‘Assignment Rule’** and enter new value in the **‘Max Work Items Allowed to be Assigned’** field. Once the new value is entered, a dialog box will appear asking for confirmation. Click on **‘Confirm’** tab to update the new value. Now, records that are present in the Queues which are associated with the Assignment Rule will be auto assigned to the users as per the updated value.

![](../../.gitbook/assets/Max\_2.jpg)



