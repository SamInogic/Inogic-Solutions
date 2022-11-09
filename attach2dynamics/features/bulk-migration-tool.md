# Bulk Migration Tool

Bulk Migration Tool migrates the attachment from Dynamics 365 CRM to SharePoint/Azure Blob Storage. It migrates the attachments faster than the Bulk Migration Job present in CRM.

#### **How to use Bulk Migration Tool?**

* Download and install the Bulk Migration Tool in your system from [here.](https://www.inogic.com/product/productivity-apps/dynamics-365-crm-sharepoint-security-metadata-sync)
* Click on the SharePoint Security Sync Tool icon to open the tool.

![](../../.gitbook/assets/BMT\_1.png)

* Select deployment type as **‘Office 365’** --> Fill in the following details in the given fields.
  * **Display list of available organizations:** Enable the checkbox in case of multiple organizations in CRM
  * **Online Region:** Select the respective region
  * **Username:** Use the CRM username
  * **Password:** Use the CRM password
* Click on **‘Login’**.

![](../../.gitbook/assets/BMT\_2.png)

* Now you will be able to see the Attachment Migration tab as shown in the below image:

![](../../.gitbook/assets/BMT\_3.png)

{% hint style="info" %}
**Note: As the user has Attach2Dynamics License, the user will be able to see the Attachment Migration tab in the Attachment Migration Tool.**
{% endhint %}

The Attachment Migration tab is to perform the **Bulk Migration Job** i.e. **Move/ Copy** the past attachments from Dynamics CRM to SharePoint/Azure Blob Storage. You are required to fill the following fields for smooth migration of attachments:

**For?**: This specifies whether you are doing Bulk Migration for Activities, Notes, or Sales Literature.

**Entity:** Select the entity for which you want to migrate attachments.

**Action:** Select either 'Copy' or 'Move'. To know more about Copy or Move, please follow this link. (add a hyperlink for move and copy)

**From:** Enter the date from which you want to start the migration job.

**To:** Enter the end date till which you want to do the migration.

![](../../.gitbook/assets/BMT\_4.png)

Once done, click on **Proceed** to migrate the attachments in bulk to Azure Blob Storage or SharePoint.
