# Set up User Availability

Vacations, holidays or sick leaves are part and parcel of the user work life. When such situations arise, where users are not available to work on Leads (other entities), managers has to manually assign the workload of that user to others. With ‘Vacation’ entity in Lead Assignment and Distribution Automation, managers can set the availability for each user and depending on this Leads (other entities) will be assigned.

For example, suppose there are three users – **Harry, Rick** and **Sam**. If **Rick** goes on a short vacation after new year, then manager can set the availability of Rick for that particular time period as **‘unavailable’**. Now the incoming Leads for that period of time will be automatically assigned to Harry and Sam.

To set user availability automatically, follow the steps given below:

* Navigate to **Lead Assignment and Distribution Automation --> Administration --> Vacations -->** Click on **‘New’.**

![](../../.gitbook/assets/Vacations\_4.1.png)

* Enter the following details and click on **‘Save’.**
  * **Name:** Enter appropriate leave detail. For eg. Christmas vacation, sick leave, etc.&#x20;
  * **User:** Select the user.&#x20;
  * **Status:** Select the nature of absence.&#x20;
  * **Description:** Provide a short description for the unavailability of the user.&#x20;
  * **Vacation Period:** Enter the **‘Start date’** and **‘End Date’** of the vacation.

![](../../.gitbook/assets/Vacations\_2.png)

![](../../.gitbook/assets/Vacations\_5.png)

{% hint style="info" %}
**Note:**

* **Vacation records will not be created if the same date is conflicting with another existing record of that particular user. Since there is an already existing record with the same date another records will not be created.**
* **If any vacation record pertaining to current date (today's date) is activated, deactivated or deleted then the status of the respective user will be duly updated w.r.t that vacation record.**&#x20;
{% endhint %}

### Status Types

By default, this solution offers two status types - ‘Available’ and ‘Unavailable’ – when the solution is first installed in the CRM. These status types defines the nature of availability of users. To create new ‘Status Types’ records follow the steps given below:

* Navigate to **Lead Assignment and Distribution Automation --> Administration --> Status Types -->** Click on **‘New’**.

![](<../../.gitbook/assets/Status Types\_1.png>)

* Give appropriate name -->Select the availability status --> Click on **‘Save’.**

![](<../../.gitbook/assets/Status Types\_2.png>)

### Update User Availability

There can be situations where user may take leave and then cancel it. And since the vacation record is already created, it would show the availability status as ‘Unavailable’ for that particular user. In such situations, the admin or that particular user can manually update the status of availability.&#x20;

To update availability, follow the steps given below:

* Navigate to **Lead Assignment and Distribution Automation --> Administration --> Users.**

![](<../../.gitbook/assets/Update user\_1.png>)

* Select the **user** --> In ‘**Assignment Details’** update the **Availability** status --> Click on **‘Save’.**

![](<../../.gitbook/assets/Update user\_2.1.png>)

![](<../../.gitbook/assets/Update user\_3.1.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
