# Azure Active Directory App

Please follow the below steps to create Azure Active Directory (AAD) app:

Step 1 – Login into Azure portal – [https://portal.azure.com/](https://portal.azure.com/)

Step 2 – Click on Azure Active Directory.

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image1.png)

Step 3 – Navigate to App registrations and then click on new registration.

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image2.png)

Display name of app –

If you are going to use this app for Recurring Billing Manager then “Inogic\_RecurringBillingManager”.

Redirect URI should be in below format –

“https://CRMUrl/WebResources/ikl\_/SM/html/Callback.html”

Here CRMUrl is like “https://octtrial.crm8.dynamics.com”. After filling these details click on register.

![](<../../.gitbook/assets/Azure direct\_1.png>)

Step 4 – Now you need to give some permissions to app. So navigate to API permissions. Here you need to add permission for Dynamics CRM.

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image4.png)

Please follow below screenshot for add permissions.

Adding Dynamics CRM permissions:

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image5.png)

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image6.png)

After adding permissions we need to Grant this by clicking **Grant admin consent** button.

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image7.png)

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image8.png)

Step 5 – Now we need to create secret key. For this, navigate to Certificate & secrets and create secret key.

Please copy/paste it somewhere because after some time it will disappears.

![How to create Azure Active Directory App](https://www.inogic.com/blog/wp-content/uploads/2020/10/image9.png)

![](https://www.inogic.com/blog/wp-content/uploads/2020/10/image10.png)

We are done with AAD app, now copy/paste your app id and secret key in connector in credentials section then you can authenticate it.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
