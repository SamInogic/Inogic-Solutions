# SharePoint

Follow the steps given below to configure SharePoint connector:

{% embed url="https://youtu.be/pZzZjULKGcs" %}

Navigate to **Attach2Dynamics app --> Connectors --> Click on New --> Fill the following details**.

* **Name:** Give name to the connector&#x20;
* **Connector Type:** Choose SharePoint from the drop-down.&#x20;
* **Default Connector:** If required, enable the checkbox to set SharePoint\_1 as default connector.
* **SharePoint Site:** This is valid only for SharePoint. It is the location of SharePoint, where files and folders will be stored. Select the valid SharePoint site here. This field is not visible for Dropbox and Azure Blob Storage.

![](../../../.gitbook/assets/SP\_1.png)

{% hint style="info" %}
**Note: The user has to create new SharePoint site for each new connector.**
{% endhint %}

* **Auth-Type:** You can select the value **‘App’** or **‘Credential’** here. This indicates whether **Authentication** with the connector is done through App or Credential. For SharePoint both **App** and **Credential** are supported.&#x20;

![](../../../.gitbook/assets/SP\_2.png)

*   After the Connector record is created the connector credentials need to be authenticated.

    To authenticate the connector, click on the **Authenticate button** on the command bar.&#x20;

![](<../../../.gitbook/assets/SP Authen.png>)

This button is visible only to users with **System Administration** or **Attach2Dynamics Administrator** role.

Now let's see the two different ways to authenticate connector.

### **Credentials:**&#x20;

Here the Authentication with connector is done through Credential i.e. **id and password**. It is mandatory to enter credentials in order to create a new Connector. For authentication through credentials, for any attachment action, the name of user appears who has authenticated the Connector.&#x20;

Enter value for Id and Password/Secret --> Authenticate the credentials.

![](../../../.gitbook/assets/SP\_3.png)

{% hint style="info" %}
**Note: The Id/Password origin differs for SharePoint, Dropbox and Azure Blob Storage.**

**• Id and Password for SharePoint: In the Id field enter your username and in Password enter password. It can be your normal Dynamics 365 CRM credentials.**&#x20;

**• Id and Password/Secret for Dropbox: Enter your ‘Developer’ App Key and App secret for the app you are developing.**&#x20;

**• Id and Password for Azure Blob Storage: Enter your Storage Account Name and Access Key as password.**
{% endhint %}

### **App:**&#x20;

In App authentication, if any action is performed then the name of logged-in user appears.

![](<../../../.gitbook/assets/Share\_App\_1 (1).png>)

* In order to know how to generate Id and Password/Secret for App [click here](https://www.inogic.com/blog/how-to-create-azure-active-directory-app/). After you have generated the Id and Password enter them in the fields provided.

![](../../../.gitbook/assets/Share\_App\_2.png)

* Once the record is saved, click on the **Authenticate** Button.

![](<../../../.gitbook/assets/Authenticate (1).png>)

* A Pop-up window will appear. Fill in your credentials and then confirmation Pop-up will be opened.&#x20;
* In the Pop-up, please select **Consent on behalf of your organization** --> Click on the **Accept** button.
* After clicking on the Accept button if the credentials are correct then you will get a Success message window.

![](<../../../.gitbook/assets/Connector Config\_1 (1).png>)

* Now if any logged in user uploads or performs any attachment action using Attach2Dynamics UI, their name will appear for the action.&#x20;

![](<../../../.gitbook/assets/Connector Confg\_SharePoint 1 (1).png>)

* In the below screenshot, name of the admin appears when they are logged in and have uploaded the file.

![](<../../../.gitbook/assets/Connector Confg\_SharePoint 2.png>)

* Now if another person is to upload a file then that person's name will be displayed on the site due to authenticating connector through app.&#x20;

![](<../../../.gitbook/assets/Connector Confg\_SharePoint 3.png>)
