# Connect & Configure QuickBooks

### **Prerequisites**

**Given below are the prerequisites required before adding single or multiple QuickBooks companies:**&#x20;

Before proceeding with the configuration of QuickBooks, you need to make sure about the following items:\
It is necessary to enter a redirect URI in QuickBooks which would allow the InoLink application to interact with QuickBooks without any interference. You need to copy the below link and paste it in QuickBooks.

Link: [https://inolinkapi.azurewebsites.net/QBResponse/AccessToken](https://inolinkapi.azurewebsites.net/QBResponse/AccessToken)

Given below are the steps to enter redirect URI in QuickBooks.

* **Step 1:** Copy the above link.
* **Step 2:** Open QuickBooks, login by visiting [https://developer.intuit.com/](https://developer.intuit.com/) with admin credentials (full QuickBooks privileged user).

![](<../../../.gitbook/assets/Connect & Configure QB\_1.png>)

![](<../../../.gitbook/assets/Connect & Configure QB\_2.png>)

* **Step 3:** Click on Dashboard and select the app you have created.

![](<../../../.gitbook/assets/Connect & Configure QB\_3.png>)

If you don’t have existing App then click on **Create New App** as shown in the below screenshot:

![](<../../../.gitbook/assets/Connect & Configure QB\_4.png>)

After clicking on Create new app, a screen will open which would ask to select the platform you want to develop for.

![](<../../../.gitbook/assets/Connect & Configure QB\_5.png>)

Click on **QuickBooks Online and Payments**, it will ask for App Name. Enter the Name of app based on your requirement. Select **com.intuit.quickbooks.accounting** checkbox and click on Create App, as shown below:

![](<../../../.gitbook/assets/Connect & Configure QB\_6.png>)

**A. For OAuth 1.0**

If your developer account has created apps before **July 17, 2017**, and any apps created by that account, including future apps and apps under development now, will use **OAuth 1.0**

Now click on **Keys.** Here you will find **Production & Development** keys. You will need the **‘OAuth Consumer Key’** and **‘OAuth Consumer Secret’** to link QuickBooks Online with InoLink.

![](<../../../.gitbook/assets/Connect & Configure QB\_7.png>)

**B. For OAuth 2.0**&#x20;

After the app is created, Get Started page will open. Here you will find the Production and development Keys. You will need the **Client ID** and **Client Secret** to link QuickBooks Online with InoLink.

![](<../../../.gitbook/assets/Connect & Configure QB\_8.png>)

*   **Step 4:** Click on **Keys and Credentials** and scroll down to find Redirect URIs**.**

    For Production QuickBooks Company you need to add all the details mentioned in the below screenshot to get Client ID and Client secret for Production Company.

![](<../../../.gitbook/assets/Connect & Configure QB\_9.png>)

After verifying all the details, you will be able to see the Client ID and Client Secret as show below:

![](<../../../.gitbook/assets/Connect & Configure QB\_10.png>)

* **Step 5**: Enter the redirect URI provided and click on **Save** button.

Link: [https://inolinkapi.azurewebsites.net/QBResponse/AccessToken](https://inolinkapi.azurewebsites.net/QBResponse/AccessToken)

![](<../../../.gitbook/assets/Connect & Configure QB\_11.png>)

This will allow InoLink to interact with QuickBooks. Once you have all the pre-requisites set in place you are good to add and connect single and multiple companies. Then, you need to configure the **QuickBooks** connection as per your requirement in InoLink Settings. After clicking on **QuickBooks** option in **Enable and connect to Dynamics 365 and QuickBooks system** section in InoLink Settings you will get the window shown below:

![](<../../../.gitbook/assets/Connect & Configure QB\_12.png>)

Here, select the suitable details of the QuickBooks that are to be synced with the CRM system.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
