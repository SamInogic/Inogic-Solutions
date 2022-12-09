# Capacity Assignment

In this Assignment Rule, Leads are assigned on the basis of user capacity. Each user is assigned a base capacity by the manager. For e.g. Let’s consider that 1 Lead is equivalent to 5 units. Based on this A is given capacity of 5 units, B is given capacity of 10 units and C is given capacity of 12 units. As Lead comes it is systematically assigned to A, B and C. Now depending on capacity A has zero units left whereas B has 5 units and C has 7 units left. This is automatically highlighted in the ‘Available Capacity’ field of each user. So, the next Lead will be assigned to B and then C. The **‘Available Capacity’** field is auto-populated as per available capacity of user. Here, if A closes the Lead then the ‘Available Capacity’ field will auto-populate and display 5 units against A. Now, A is eligible to be assigned incoming Leads. In this way, on the basis of available user capacity Leads will be assigned to each user.

Now to assign Leads on the basis of User Capacity follow the steps given below:

* Navigate to **Lead Assignment & Distribution Automation App --> Administration --> Assignment Configuration -->** Select the respective **Assignment Configuration -->** Click on **New Assignment Rule.**

![](<../../.gitbook/assets/Round Robin\_1.png>)

* Enter the mandatory details and click on **‘Save’.**
  * **Name:** Give name to the Assignment Rule.&#x20;
  * **Assignment Configuration:** This field is auto-populated.&#x20;
  * **Description:** Provide description.&#x20;
  * **Criteria Mode:** Select between **‘Simple’** or **‘Advanced’** criteria mode. **‘Simple’** mode is based on **‘Views’** and **‘Advanced’** is based on **Fetch Xml**. Here, Simple mode is selected.&#x20;
  * **Execution Order:** Give numeric value, **for example - 1.** If there are two or more Round Robin based Assignment Rules then this field states the order in which Rules are to be executed while assigning Leads.&#x20;
  * **Queue:** Select the respective Queue.&#x20;
  * **Consider Availability:** This field checks the availability status of users before assigning work items. Select **‘Yes’** or **‘No’.**
  * **Assignment Algorithm:** Select between Round Robin and User Capacity. Here we selected Capacity. Once the field is populated another field – **Unit Effort Required For Work Item** – becomes visible.&#x20;
  * **Unit Effort Required For Work Item:** Define the units required for per work item. For example: 1 Lead = 2 units.&#x20;
  * **Max Work Items Allowed to be Assigned:** This field denotes the maximum number of work items that is allowed to be assigned to users. For example – 10. Here, each user will be assigned maximum 5 Leads.
  * **Period:** This is an option-set field with the following options - **Daily, Weekly, Monthly and Overall**. It defines the period for which assignment rule will be run checking for incoming work items (Entity records) and assigning it to the users defined in the assignment rule.
    * **Daily:** The assignment rule will be triggered daily assigning work items to users as per their capacity.&#x20;
    * **Weekly:** The assignment rule will be triggered weekly assigning work items to users as per their capacity.
    * **Monthly:** The assignment rule will be triggered monthly assigning work items to users as per their capacity.
    * **Overall:** The assignment rule will be triggered as and when user closes the Lead or completes the task and updates the status of the work item.
  * **Open Work Item Statuses:** Select the status from the dropdown, for e.g. Open-New. Here, based on the status ‘Open-New’ Leads will be assigned to users. Once the Lead’s status changes from Open-New to another status then that Lead will be considered as completed and automatically another Lead with status as ‘Open-New’ is assigned to the same user. This process will go on till all the Leads are assigned.

![](<../../.gitbook/assets/Capacity\_1 (1).png>)

![](../../.gitbook/assets/Capacity\_2.png)

* To specify user capacity, go to **Lead Assignment and Distribution Automation App --> Administration --> Users --> Lead Assignment Users --> Select User --> Assignment Details --> Populate Base Capacity field --> Click on ‘Save’.**

{% hint style="info" %}
**Note: For On-Premises, you will have to use Classic way to specify user capacity as UCI will be read only. For classic way, follow the steps given below.**
{% endhint %}

*   Go to **Advanced Settings --> Settings --> Lead Assignment Distribution -->**&#x20;

    **Users --> Select User --> Assignment Details --> Populate Base Capacity field --> Click on ‘Save’.**

![](<../../.gitbook/assets/User workload\_2.png>)

![](<../../.gitbook/assets/image (224).png>)

![](<../../.gitbook/assets/image (40).png>)

* Now in **'Assignment Rule'** go to second tab – **User Workload.** Every individual user has their own capacity and has their priority to work on new items. A senior member can work on more items than a junior member. User Workload is used to handle such cases. The User workload records get created when 'Assignment Rule' records get created and when new member is added in the queue (which is set on the Assignment Rule).

![](<../../.gitbook/assets/Capacity\_5 (1).png>)

* Click on any one user and get detailed workload information about that particular user. It gives you information about the total number of active records owned by the user in CRM. Further, you can also update the maximum records assigned to user.

![](<../../.gitbook/assets/Capacity\_6 (1).png>)

![](<../../.gitbook/assets/Capacity\_7 (1).png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

####
