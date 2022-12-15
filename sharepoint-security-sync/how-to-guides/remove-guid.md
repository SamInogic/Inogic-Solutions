# Remove GUID

When a document is uploaded to the SharePoint using Attach2Dynamics or using OOB Documents tab in SharePoint, a folder with record name is created in the SharePoint. But along with the name, GUID (Unique ID of the record) is also added in the SharePoint folder name as shown in the below screenshot this GUID:

![](<../../.gitbook/assets/New GUID\_1.png>)

To remove the GUID you first need to change the organization settings of CRM. To change the settings, please follow the steps given below:

* Navigate to the [link](https://urldefense.com/v3/\_\_https:/github.com/seanmcne/OrgDbOrgSettings/releases\_\_;!!HCORQGcuXVTsyh1-D2uGonQ!47A-28I6CHxMnG8ZNQ7cG5DwmlugOASgzIlXJSkbZDciHrJmdJAV\_2kXJu99EfF8h2SNyQ$) and download the **‘OrganizationSettingsEditor’** solution file by clicking on the name as shown in the below screenshot.

![](../../.gitbook/assets/GUID\_1.jpg)

* Once the solution is downloaded, import it into your environment.
* Click on the **gear** icon --> Select **Advanced Settings**.

![](../../.gitbook/assets/GUID\_2.jpg)

* Navigate to Settings --> Solutions --> Click on **'Import solution'** button.

![](../../.gitbook/assets/GUID\_3.jpg)

![](../../.gitbook/assets/GUID\_4.jpg)

* Please choose the downloaded **OrganizationSettingsEditor** solution file and click on the **'Next'** button to proceed.

![](../../.gitbook/assets/GUID\_5.jpg)

![](../../.gitbook/assets/GUID\_6.jpg)

* After the solution is successfully imported, open the solution and navigate to the Configuration page and search for **‘CreateSPFoldersUsingNameandGuid’.**

![](../../.gitbook/assets/GUID\_7.jpg)

* By default, the **‘Current Value’** of **‘CreateSPFoldersUsingNameandGuid’** is set to true, to change it, click on the **edit** button.

![](../../.gitbook/assets/GUID\_8.jpg)

* Enter **‘false’** (lower case) in **‘CreateSPFoldersUsingNameandGuid’** field --> Click on **‘Update’** button --> Click on **‘OK’** button from the confirmation pop-up.

![](../../.gitbook/assets/GUID\_9.jpg)

{% hint style="info" %}
**Note: SharePoint Folders created after applying the above settings will be created without GUID, the history folders in SharePoint which are created before the above settings will remain with GUID.**
{% endhint %}

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

