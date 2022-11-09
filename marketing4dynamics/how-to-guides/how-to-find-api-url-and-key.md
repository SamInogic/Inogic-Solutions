# How to find API URL and Key

To connect Mailchimp and Dynamics 365 CRM, **API URL** and **API key** from Mailchimp account is necessary. Follow the steps given below to obtain the same.

### API Key

* First, log into the existing Mailchimp account or create a new account.

![](<../../.gitbook/assets/1 (401).png>)

* Go to **Account --> Extras --> Click on API keys.**

![](<../../.gitbook/assets/2 (9).png>)

![](<../../.gitbook/assets/3 (22).png>)

* Navigate to **'Your API keys'** section. If you already have an API key listed and you would like to use it, simply copy it for connecting to your Mailchimp account otherwise, click on **‘Create A Key’** button.

![](<../../.gitbook/assets/4 (32).png>)

* The key will be created shortly. This will be the **API key.**

![](<../../.gitbook/assets/5 (27).png>)

### **API URL**

* Log into the existing Mailchimp account or create a new account.
* The general format of the API URL is like this - **https://{dc}.api.mailchimp.com/3.0/**&#x20;
* To get the {dc} for your URL, look at the URL in your browser. On the home page of Mailchimp you’ll see something like - **https://us6.admin.mailchimp.com/.** Here, the **us6** part is the server prefix **(dc)**. Note that your specific value may be different.&#x20;
* So in the above example, your API URL would be **https://us6.api.mailchimp.com/3.0/**

![](<../../.gitbook/assets/6 (20).png>)

* Now use the **API URL** and **API key** to connect Mailchimp account with Dynamics 365 CRM.

