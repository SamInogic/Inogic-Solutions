# Connector Settings

With three different cloud storages available for document management, the following prerequisites will depend on which of the connectors you will be using to manage and store attachments/documents in cloud.&#x20;

### SharePoint:

In case of SharePoint, it is necessary to enable server-based SharePoint integration for your Dynamics 365 CRM environment.&#x20;

To do this, follow the steps given below:

* Navigate to **Advanced Settings --> Settings --> Document Management**.

![](../../.gitbook/assets/PRE\_1.png)

* Go to **‘Enable Sever-Based SharePoint Integration’**.

![](../../.gitbook/assets/PRE\_2.png)

* Click on **Next**.

![](../../.gitbook/assets/PRE\_3.png)

* Now, select the location of **SharePoint site** and click on Next.

![](../../.gitbook/assets/PRE\_4.png)

* Now, enter the **URL of SharePoint site** that you want to use --> Click on **Next**.

![](../../.gitbook/assets/PRE\_6.png)

* Once the site is validated, click on **Finish**.

![](../../.gitbook/assets/PRE\_7.png)

* The server-based integration of SharePoint site is now enabled for your Dynamics 365 CRM environment. Now, go back to **Settings --> Document Management Settings**.

![](../../.gitbook/assets/PRE\_10.png)

* Select the **Entities** for which Document Management needs to be enabled --> Enter the **URL of active SharePoint sites** where you want to store documents --> Click on **Next**.

![](../../.gitbook/assets/PRE\_11.png)

* Check **‘Based on entity’** to automatically create document libraries and folders that are based on the Dynamics 365 Account on the SharePoint site. Users will not be prompted to create them. If you don't want folders automatically created, do not select the **‘Based on entity’** check box. Click on **Next** button.

![](../../.gitbook/assets/PRE\_12.png)

* Click on **Finish**.

![](<../../.gitbook/assets/PRE\_14 (1).png>)

Once this is done, you can easily **store Documents/Attachments** related to selected **Entities** in the respective **SharePoint site using Attach2Dynamics**.

### Dropbox:

If you are using Dropbox connector, you need to **create app on Dropbox**. To know more, click [here.](https://docs.inogic.com/attach2dynamics/configuration/connector-configuration/dropbox#now-to-get-the-id-secret-for-dropbox-follow-the-steps-given-below)

![](../../.gitbook/assets/Dropbox\_1.png)

### Azure Blob Storage:

If you are using Azure Blob Storage connector, then you need to create a **storage account**. To know more, click [here](https://docs.inogic.com/attach2dynamics/configuration/connector-configuration/azure-blob-storage).

![](../../.gitbook/assets/Azure\_1.png)
