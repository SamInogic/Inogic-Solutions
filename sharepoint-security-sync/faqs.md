# FAQs

## 1) After importing the solution of SharePoint Security Sync from website all the Processes of SharePoint Security Sync are in a 'Draft/Deactivated' state? What to do?

Once the solution is imported, please follow the below steps to activate all the processes of SharePoint Security Sync.

* Click on the **gear icon** --> Select **Advanced Settings**.&#x20;

![](../.gitbook/assets/A4D\_1.png)

* Next, select **Processes**.

![](../.gitbook/assets/A4D\_2.png)

* From **'All Process'** View activate the process shown in the below screenshot:

![](../.gitbook/assets/SSS\_1.jpg)

## 2) Is there a way to sync the previous records in bulk?

Yes, by using the [Bulk Synchronization Tool](https://docs.inogic.com/sharepoint-security-sync/sharepoint-security-sync-tool) you can sync the previous records in bulk.

## 3) How to enable file deletion?

You can enable file deletion by creating the [Security Template ](https://docs.inogic.com/sharepoint-security-sync/features/security-templates)for users with required actions.&#x20;

## 4) Why is there an error while creating an anonymous link of file?

The error is due to insufficient permission on SharePoint.

## 5) How can I move history attachments?

You can move/copy your history attachments by using [Bulk Migration Job](https://docs.inogic.com/sharepoint-security-sync/features/bulk-migration-job) feature.&#x20;

## 6) We have done a sandbox copy of the production environment to a TEST env. and like to have the 'SharePoint Security Sync' solution to work in this new instance. What do we need to do?

You need to delete the Inogic License Details record from your sandbox environment. After deleting the next step would be to [activate the license](https://docs.inogic.com/sharepoint-security-sync/getting-started/license-activation).

To delete the SharePoint Security Sync license follow the below steps:

Step 1: Navigate to **Advanced Find.**

![](<../.gitbook/assets/FAQ\_1 (5).png>)

Step 2: Select **Inogic License Details** in **‘Look for’** and click on **Results** button.

![](<../.gitbook/assets/FAQ\_2 (1).png>)

Step 3: Select the **SharePoint Security Sync** record and **delete** it.

![](<../.gitbook/assets/FAQ\_1 (1).png>)

## 7) What to do if I am unable to authenticate the connector?

In such situations, please ensure the credentials are correct and you have a Global administrator privileges and also are a SharePoint site owner.

## 8) I am getting an error pop-up stating ‘Unable to get Tokens’. What should I do?

Firstly, please check if the browser setting is to Enable the cookies. To know more please follow this [link.](https://docs.inogic.com/sharepoint-security-sync/how-to-guides/enable-cookies-setting) If the solution still doesn’t work please then try to authenticate the connector once. If you are using **Authentication mode** as **App** then please make sure that you have selected the consent box while authenticating. Please follow this [link](https://docs.inogic.com/sharepoint-security-sync/configuration/connector-configuration#app) to know about how to authenticate the connector.

## 9) Which types of SharePoint Site does SharePoint Security Sync support?

Currently, we support only SharePoint Communication and Team site. SharePoint Subsite is not supported.

## 10) What to do if I get ‘Active user count exceeds the user limit’ error?

This message is displayed when the number of the CRM user is increased beyond the subscribed users. If you get this issue then please reach out to us at [crm@inogic.com](mailto:crm@inogic.com) with the total user count. To get the total user count please execute the below condition in **Advanced Find**:

![](<../.gitbook/assets/FAQ\_1 (3).png>)

## 11) What to do if I am not able to see the Attach2Dynamics button?

Please make sure the user has Attach2Dynamics Admin / User security role assigned. To know more about the Attach2Dyamics security role please follow this [link.](https://docs.inogic.com/sharepoint-security-sync/getting-started/set-up-security) Also, please make sure the Entity configuration record is created for the respective entity. To know more about entity configuration please follow this [link](https://docs.inogic.com/sharepoint-security-sync/configuration/entity-configuration).

## 12) Can Attach2Dynamics UI be shown on a Tab instead of clicking the Attach2Dynamics button?

Yes, Attach2Dynamics can be shown on a tab. To know more regarding the configuration please follow this [link.](https://docs.inogic.com/attach2dynamics/configuration/iframe-configuration)

## 13) I changed my Microsoft account password after which I started facing an issue while using SharePoint Security Sync solution. What to do?

In order to solve this issue, you will have to delete the connection detail record of the user who is this getting error.

To delete the connection detail record of the user please follow the steps given below:

* Open **Advanced Find** from your CRM.

![](<../.gitbook/assets/FAQ\_1 (1).jpg>)

* In the **Look for** dropdown select **Connection Details** entity.

![](<../.gitbook/assets/FAQ\_2 (1).jpg>)

* Please add a condition as shown in the below screenshot:

![](<../.gitbook/assets/FAQ\_3 (1).jpg>)

* Click on **Results.**

![](../.gitbook/assets/FAQ\_4.jpg)

* Select all the records of that user --> Click on **Delete.**

![](<../.gitbook/assets/FAQ\_5 (1).jpg>)

* Once the record is deleted, you have to authenticate all the connectors and then hit the **Attach2Dynamics** button. For this, click on the Authenticate button on the ribbon bar.

![](../.gitbook/assets/FAQ\_13.1.png)

* Check the **consent** box as shown below:

![](../.gitbook/assets/FAQ\_13.2.jpg)

{% hint style="info" %}
**Note: The Consent box will be available only when App is used to create the connector.**
{% endhint %}

## 14) What are the steps to export Log in Excel sheet?

To export the log record in Excel, follow the steps given below:

* Open **'Advance find'** in CRM.

![](../.gitbook/assets/FAQ\_14.1.png)

* In the **'Look for'** dropdown, select Logs entity.

![](../.gitbook/assets/FAQ\_14.2.png)

* Add a condition for the error, as shown in the below screenshot.

![](../.gitbook/assets/FAQ\_14.3.jpg)

* Now click on the Edit Columns button.

![](../.gitbook/assets/FAQ\_14.4.png)

* After clicking on 'Edit Columns', you have to click on the **Add Column** option present inside the Common Task section.

![](../.gitbook/assets/FAQ\_14.5.png)

* Next, select the **Trace Log** field and then click on the **OK** button.

![](../.gitbook/assets/FAQ\_14.6.png)

* Once again click on the **OK** button on Edit Column window.

![](../.gitbook/assets/FAQ\_14.7.png)

* Click on the **Result.**

![](../.gitbook/assets/FAQ\_14.8.png)

* Now click on the **Export Logs** button dropdown and then click on the **Static Worksheet** option.

![](../.gitbook/assets/FAQ\_14.9.png)

* In a short time, an excel file will be downloaded for offline consumption.

## 15) **Is it safe to delete the completed Batching and Sync Status**?

Yes, it is safe to delete the batching and sync status which are completed. By using the Bulk deletion job, you can delete such batching and sync status records. You can make use of the below queries in the bulk deletion job to delete the records.

**Query for Sync status:**

![](<../.gitbook/assets/FAQ\_15.1 (1).jpg>)

**Query for Batching:**

![](<../.gitbook/assets/FAQ\_15.2 (1).jpg>)

## 16) **How to fix the following error 'No reply address is registered for the application'?**

![](../.gitbook/assets/FAQ\_16.1.png)

This issue occurs when the Redirect URL has not been added in the **** redirect section of the Azure App as shown in the below image:

![](../.gitbook/assets/FAQ\_16.2.jpg)

Please follow the below steps to add a redirect URL:

* Navigate to **Azure App** --> Click on **Redirect URL**.

![](../.gitbook/assets/FAQ\_16.3.jpg)

* Click on **Add a platform** button --> Select **Web**.

![](../.gitbook/assets/FAQ\_16.4.jpg)

* Add the Redirect URL.

![](../.gitbook/assets/FAQ\_16.5.jpg)

{% hint style="info" %}
**Note: To identify the Redirect URL, kindly navigate to the SharePoint Security Sync App-> Connectors-> Credentials tab and copy the redirect URL which is highlighted in the below screenshot:**
{% endhint %}

![](../.gitbook/assets/FAQ\_16.6.jpg)

* After adding the redirect URL, click on **Configure** button.

![](../.gitbook/assets/FAQ\_16.7.jpg)

* Navigate to **SharePoint Security Sync App** -> **Connectors** --> **Authenticate** the connector again.

![](../.gitbook/assets/FAQ\_16.8.jpg)

To know more about this, kindly follow this [link](https://docs.inogic.com/sharepoint-security-sync/configuration/connector-configuration#app).

## 17) What is the difference between SharePoint Security Sync and Attach2Dynamics?

<figure><img src="../.gitbook/assets/Attach2Dynamics and SharePoint Security Sync Comparison.png" alt=""><figcaption></figcaption></figure>
