# FAQs

## 1) How can you move history attachments?

With the use of Attach2Dynamics feature called [Bulk Migration](https://docs.inogic.com/attach2dynamics/features/bulk-migration-job) job, you can move your historical notes/email/sales literature attachments.

## 2) How to enable file deletion?

To enable file deletion, you need to create [Security Template](https://docs.inogic.com/attach2dynamics/features/security-templates) with required actions.&#x20;

## 3) We have done a sandbox copy of the production environment to a TEST env. and like to have the 'Attach2Dynamics' solution to work in this new instance. What do we need to do?

You need to delete the Inogic License Details record from your sandbox environment. After deleting the next step would be to [activate the license](https://docs.inogic.com/attach2dynamics/getting-started/license-activation).

To delete the Attach2Dynamics license follow the below steps:

Step 1: Navigate to **Advanced Find.**

![](<../.gitbook/assets/FAQ\_1 (1).jpg>)

Step 2: Select **Inogic License Details** in **‘Look for’** and click on **Results** button.

![](<../.gitbook/assets/FAQ\_2 (2).jpg>)

Step 3: Select the **Attach2Dynamics** record and **delete** it.

![](<../.gitbook/assets/FAQ\_3 (1).jpg>)

## 4) I get the following error while creating an anonymous link of file on Attach2Dynamics UI, how can I resolve this?

![](../.gitbook/assets/A2D\_FAQ.png)

This error is due to insufficient permissions on SharePoint. So, you need enable some settings in SharePoint. For more details, please click [here](https://docs.inogic.com/attach2dynamics/prerequisites/untitled).

## 5) Is it possible to connect with multiple cloud storage?

Yes, you can connect with multiple cloud storage. For this, you have to create different connectors depending upon each cloud storage.

## 6) After importing the solution of Attach2Dynamics from website all the Processes of Attach2Dynamics are in a 'Draft/Deactivated' state. What to do?

Once the solution is imported, please follow the below steps to activate all the processes of Attach2Dynamics.

* Click on the **gear icon** at the top right --> Select **Advanced Settings**.

![](../.gitbook/assets/A4D\_1.png)

* Then select **Processes**.

![](../.gitbook/assets/A4D\_2.png)

* From **All Process View** activate the process shown in the below screenshot.

![](../.gitbook/assets/A2D\_FAQ\_3.png.jpg)

## 7) What to do if I am unable to authenticate the connector?

In such situations, please ensure the credentials are correct and you have a Global administrator privileges and also are a SharePoint site owner.

## 8) I am getting an error pop-up stating ‘Unable to get Tokens’. What should I do?

Firstly, please check if the browser setting is to Enable the cookies. To know more please follow this [link](https://docs.inogic.com/attach2dynamics/how-to-guides/enable-cookies-setting). If the solution still doesn’t work please then try to authenticate the connector once. If you are using **Authentication mode** as **App** then please make sure that you have selected the consent box while authenticating. Please follow this [link](https://docs.inogic.com/attach2dynamics/configuration/connector-configuration/sharepoint#app) to know about how to authenticate the connector.

## 9) What to do if I get ‘Active user count exceeds the user limit’ error?

This message is displayed when the number of the CRM user is increased beyond the subscribed users. If you get this issue then please reach out to us at [crm@inogic.com](mailto:crm@inogic.com) with the total user count. To get the total user count please execute the below condition in **Advanced Find**:

![](<../.gitbook/assets/FAQ\_1 (6).png>)

## 10) What to do if I am not able to see the Attach2Dynamics button?

Please make sure the user has Attach2Dynamics Admin / User security role assigned. To know more about the Attach2Dyamics security role please follow this [link.](https://docs.inogic.com/attach2dynamics/getting-started/set-up-security) Also, please make sure the Entity configuration record is created for the respective entity. To know more about entity configuration please follow this [link.](https://docs.inogic.com/attach2dynamics/configuration/entity-configuration)

## 11) Can Attach2Dynamics UI be shown on a Tab instead of clicking the Attach2Dynamics button?

Yes, Attach2Dynamics can be shown on a tab. To know more regarding the configuration please follow this [link.](https://docs.inogic.com/attach2dynamics/configuration/iframe-configuration)

## 12) I cannot see Ribbon buttons on Connector entity post import of Attach2Dynamics solution. What to do?

Sometimes when you install a Managed solution it takes time for the ribbon buttons to appear. In such situations, please wait for some time and then you will be able to see the buttons.

## 13) I changed my Microsoft account password after which I started facing an issue while using Attach2Dynamics solution. What to do?

In order to solve this issue, you will have to delete the connection detail record of the user who is this getting error.

To delete the connection detail record of the user please follow the steps given below:

* Open **Advanced Find** from your CRM.

![](<../.gitbook/assets/FAQ\_1 (4).jpg>)

* In the **Look for** dropdown select **Connection Details** entity.

![](<../.gitbook/assets/FAQ\_2 (1).jpg>)

* Please add a condition as shown in the below screenshot:

![](../.gitbook/assets/FAQ\_3.jpg)

* Click on **Results.**

![](../.gitbook/assets/FAQ\_4.jpg)

* Select all the records of that user --> Click on **Delete.**

![](../.gitbook/assets/FAQ\_5.jpg)

* Once the record is deleted, authenticate all the connectors and then hit the **Attach2Dynamics** button.

## 14) Is the versioning feature in Azure Blob storage supported in Attach2Dynamics?

Yes, Attach2Dynamics does support the versioning feature in Azure Blob Storage. However, for the versioning feature to work, the versioning needs to be enabled in the **Azure Blob** **properties**.

Kindly follow the below steps to enable the versioning feature in Azure Blob Storage:&#x20;

* Navigate to [https://portal.azure.com/](https://portal.azure.com/)
* Click on **Storage Accounts.**

![](../.gitbook/assets/FAQ\_14.1.jpg)

* Select the **Storage Account** --> Click on **Data Protection.**

![](../.gitbook/assets/FAQ\_14.2.jpg)

* Check the **Enable versioning for blobs** checkbox and click on the **Save** button.

![](../.gitbook/assets/FAQ\_14.3.jpg)

After enabling the above property, the versioning functionality will start working just as shown in the below example:

* Navigate to **Attach2Dynamics** App --> **Entity Configurations** --> Open Account entity configuration -->Enable **Override files** --> Click on **Save**.

![](../.gitbook/assets/FAQ\_14.4.jpg)

* Navigate to **Sales Hub** --> **Accounts** --> Open **any account record** --> Click on **Attach2Dynamics** button.

![](../.gitbook/assets/FAQ\_14.5.jpg)

* Upload any file by clicking on the **Upload** button in Attach2Dynamics UI and then again **upload** the same file with the same name but different content.

![](../.gitbook/assets/FAQ\_14.6.jpg)

* Now, navigate to the **Azure Portal** --> **Storage Accounts** --> **Containers** --> **Account** --> Open the Account for which you have uploaded the file in Attach2Dynamics UI.

![](../.gitbook/assets/FAQ\_14.7.jpg)

* To check the previous versions, click on the file which you have uploaded (“Order Form.txt” in this case), and under the **Versions** tab, you will be able to see the previous versions.

![](../.gitbook/assets/FAQ\_14.8.jpg)

* Also, you can select the **previous version** and click on the **Download** **Version** button to download the previous version files.

![](../.gitbook/assets/FAQ\_14.9.jpg)

## 15) Is there a way to use Attach2Dynamics in offline mode?

Yes, you can use the **Real-time sync** feature of Attach2Dynamics to migrate uploaded documents to SharePoint in offline mode. Please follow this [link](https://www.inogic.com/blog/2022/03/how-to-enable-model-driven-apps-for-offline-use/) to enable the offline mode. For attachment migration, you will need to configure the Entity configuration for the respective entity and set the attachment action as either **Move** or **Copy**. When the offline mode is enabled, the note attachment will not get migrated. Once the user connects back with the mobile data or Wi-Fi, the note attachment will get migrated to the SharePoint/Azure Blob/Dropbox.

Please follow the steps given below to achieve the offline capability for the Note attachment with the associated account entity.

* First, enable the offline mode in your CRM. Please follow this [link](https://www.inogic.com/blog/2022/03/how-to-enable-model-driven-apps-for-offline-use/) for enabling the offline mode in your CRM.&#x20;
* Once you have enabled the offline mode in your CRM, open the Dynamics 365 App on mobile --> Login with the credentials -->Navigate to **Sales Hub -->Account**.

![](../.gitbook/assets/Image1.png)

* Open any account record -->Click on the **+ icon** in the timeline of the account record.

![](../.gitbook/assets/Image2.png)

* Select **notes** and **add** an attachment -->Click on **Add note** in the timeline and the note attachment will get added to the timeline.

![](../.gitbook/assets/Image3.png)

{% hint style="info" %}
**Note: Entity configuration must be created for the Account entity and attachment action should be either Move or Copy.**
{% endhint %}

![](<../.gitbook/assets/Image4 (1).png>)

* Once you connect back with your network connectivity, the note attachment which is added on the account record will get migrated to SharePoint and the link will get generated in the timeline.

![](../.gitbook/assets/Image5.png)

![](../.gitbook/assets/Image6.png)

## 16) **How to fix the following error 'No reply address is registered for the application'?**

![](../.gitbook/assets/FAQ\_16.1.png)

This issue occurs when the Redirect URL has not been added in the **** redirect section of the Azure App as shown in the below image:

![](../.gitbook/assets/FAQ\_16.2.jpg)

Please follow the below steps to add a redirect URL:

* Navigate to **Azure App** --> Click on **Redirect URL**.

![](<../.gitbook/assets/FAQ\_16.3 (1).jpg>)

* Click on **Add a platform** button --> Select **Web**.

![](../.gitbook/assets/FAQ\_16.4.jpg)

* Add the Redirect URL.

![](../.gitbook/assets/FAQ\_16.5.jpg)

{% hint style="info" %}
**Note: To identify the Redirect URL, kindly navigate to the Attach2Dynamics App-> Connectors-> Credentials tab and copy the redirect URL which is highlighted in the below screenshot:**
{% endhint %}

![](../.gitbook/assets/FAQ\_16.6.jpg)

* After adding the redirect URL, click on **Configure** button.

![](../.gitbook/assets/FAQ\_16.7.jpg)

* Navigate to **Attach2Dynamics App** -> **Connectors** --> **Authenticate** the connector again.

![](../.gitbook/assets/FAQ\_16.png)

To know more about this, kindly follow this [link](https://docs.inogic.com/attach2dynamics/configuration/connector-configuration).

## 17) What is the difference between Attach2Dynamics and SharePoint Security Sync?

<figure><img src="../.gitbook/assets/Attach2Dynamics and SharePoint Security Sync Comparison.png" alt=""><figcaption></figcaption></figure>
