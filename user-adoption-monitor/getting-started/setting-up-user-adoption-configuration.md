# Setting up User Adoption Configuration

Once the User Adoption Monitor solution is installed and activated, there is already a User Adoption Configuration record created for you. In case if the record is not created or you wish to update the existing record please follow the below-mentioned steps.

* Navigate to **User Adoption Monitor App --> Configuration**.

![](../../.gitbook/assets/UAT\_1.png)

* Click on **(+ New)** to create a new User Adoption Configuration record (if no record is already created) --> Fill values in the following fields.

![](<../../.gitbook/assets/UAM Config.png>)

![](<../../.gitbook/assets/UAM Config\_2.png>)

| **Field**           | **Description**                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Enable**          | Choose Yes, to enable system-wide flag for monitoring user actions. To disable system-wide monitoring set this flag as No.                                                                                                                           |
| **Track Details**   | You can select either Yes or No. If you choose yes, it creates Tracking Details record otherwise, it won\`t create Tracking Details record.                                                                                                          |
| **CRM URL**         | CRM URL to be used to generate record links in tracking information                                                                                                                                                                                  |
| **Notify Failures** | Click on the checkbox and fill email details which will appear below. Enabling this feature will send the user a daily email at 12:05 AM consisting the error logs if there are any failures at any point of time while using User Adoption Monitor. |

#### Importance of Tracking Details

If you enable Track Details in User Adoption Configuration entity, then the tool will also store a link to the record on which the action was performed by the user.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
