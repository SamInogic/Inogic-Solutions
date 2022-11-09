# Set Credentials

This step is mandatory in case of **Scheduling and Export of Excel/Word templates** (if **PDF** format is selected) using Clik2Export UI.

Once you have set credentials and generated token, you can then perform the above mentioned tasks with ease.

For this, you have to navigate to **Personalization Settings --> General Tab --> User Information --> Click on Set Credentials button and generate token.**

![](<../../.gitbook/assets/Sch Rep\_3.png>)

If Multi Factor Authentication is enabled then in this case you need to create **Azure Active Directory App.** For details, please click [here](https://www.inogic.com/blog/c2e-azure-active-directory-app/).

Follow the same steps and make sure the redirect URL is '**https://crmurl/WebResources/ikl\_/Click2Export/html/Callback.html**'.&#x20;

Once app is created, navigate to **Click2Export Configuration Entity --> Paste client id and secret key --> Save the record.**

![](<../../.gitbook/assets/Set Cred\_1.jpg>)

Now navigate to **Personalization Settings --> General Tab --> User Information --> click on Set Credentials button and generate token.**

You will get confirmation if it is successfully connected.

![](<../../.gitbook/assets/Set Cred\_2.jpg>)
