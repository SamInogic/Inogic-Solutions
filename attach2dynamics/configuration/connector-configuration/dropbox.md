# Dropbox

Follow the steps given below to configure the Dropbox connector:

{% embed url="https://youtu.be/b3ECcQnJNrw" %}

Navigate to **Attach2Dynamics app --> Connectors--> Click on New --> Fill the following details.**

* **Name:** Give name to the connector.
* **Connector Type:** Choose Dropbox from the drop-down.
* **Default connector:** If required, enable the checkbox to set Dropbox\_1 as default connector.

![](../../../.gitbook/assets/DB\_1.png)

{% hint style="info" %}
**Note: The user has to create new app for each new Dropbox connector.**
{% endhint %}

#### Now to get the Id/Secret for Dropbox follow the steps given below:  <a href="#steps" id="steps"></a>

* Go to [www.dropbox.com](http://www.dropbox.com/) and enter your login credentials for Dropbox. After you are logged in you will land on the **‘Home Page.’** At the bottom right corner of the screen click on the **‘Points of Ellipsis (the three dots)’** and then select Developers from the view.

![](../../../.gitbook/assets/DB\_2.png)

![](../../../.gitbook/assets/DP\_1.jpg)

* Now, click on **My apps** on the list in left. If you have already created an app click on the **‘app icon’**. You will be redirected to the App’s home page. Scroll down and you will find **App Key** and **App Secret**. If you don’t have an app click on **Create App**. From **Choose an API** click on **Dropbox API button**.

![](../../../.gitbook/assets/DP\_2.jpg)

* In **Choose the type of access you need** select **Full Dropbox**.

![](../../../.gitbook/assets/DB\_5.png)

* **Name your app** – Here enter the name of the app you are going to create. Check **‘agree to terms’** and click on **Create App** button. After clicking on Create App button you will be redirected to home page of the created app. Select your **App Key** and **App Secret** from here.

![](../../../.gitbook/assets/DB\_6.png)

* Enter these credentials in the **‘New Connector’** Credentials. After you enter the Password/Secret (Dropbox App Secret) it immediately gets encrypted as shown below.

![](../../../.gitbook/assets/DB\_7.png)

* The user can give access of this workspace created in Dropbox cloud storage to their team members if necessary. Go to **WorkSpac**e field and select **Team**. After selecting Team another field will appear termed **Team Folder**. Give name to the team folder.

![](../../../.gitbook/assets/DB\_8.png)

* The below folder will appear outside App folder.

![](../../../.gitbook/assets/DB\_9.png)

* If the WorkSpace field is set as **Personal** then the files and folders will be stored inside App folder.

![](../../../.gitbook/assets/DB\_10.png)

* Next the **redirect URL** in connector page needs to be added in the Dropbox App as in below screenshot. This URL is mentioned on the Connector entity.

![](../../../.gitbook/assets/DB\_11.png)

* Copy this URL and paste it in the App on Dropbox as shown below:

![](../../../.gitbook/assets/DB\_12.png)

* After entering the link click on **'Add'**. This step must not be skipped.
* Once the Connector record is created the connector credentials need to be authenticated. To authenticate the connector, click on the **Authenticate button** on the command bar.&#x20;

![](../../../.gitbook/assets/DB\_Authen.png)

This button is visible only to users with **System Administration** or **Attach2Dynamics Administrator** role.
