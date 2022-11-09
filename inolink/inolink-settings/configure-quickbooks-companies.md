# Configure QuickBooks Companies

Before configuring QuickBooks companies, let's have a look at the attributes based on which the QuickBooks data is synced:

![](<../../.gitbook/assets/Config QB Attributes.png>)

* **Account Attribute:** This is a dropdown that populates all the **Lookup** as well as **Option Set** fields on **Account** entity. You have to select value which would be considered as criteria for syncing data from CRM to QuickBooks and vice-versa. The default value is considered **Owning Business Unit**.
* **Contact Attribute:** This drop-down populates all the **Lookup** as well as **Option Set** fields on **Contact** entity. You have to select value which would be considered as criteria for syncing data from CRM to QuickBooks, and vice-versa. The default value is considered **Owning Business Unit**.
* **Use Field Service Tax:** Field Service Tax works only for **US QuickBooks companies**. This is a dropdown that gives the user an option to either choose **Field Service Tax** entity or **InoLink Tax** entity. Tax data would be synced in the chosen tax entity. If the user has selected **No**, then **InoLink Tax** entity would be considered, if the user has selected **Yes**, then **Field Service Tax** entity would be considered. If **Field Service Tax** is set as **‘Yes’**, then **Tax Code** and **Tax Code** **Details** (Field Service tax entities) privilege must be given to **InoLink security roles** for Tax synchronization.

{% hint style="info" %}
**Note: Selected values of Account and Contact Attribute must be the same.**
{% endhint %}

### Configuring Single or Multiple QuickBooks companies

QuickBooks Company can be synced on basis of **Lookup** values or **Option Set** fields.

#### Case 1: Configuring Dynamics 365 CRM with 1 QuickBooks Company.

![](<../../.gitbook/assets/Config QB Case1.1.png>)

* **Company Name:** It will display the name of the QuickBooks Company. Initially, it will be empty, once the company data has been saved, you can see the name of the company.

{% hint style="info" %}
**Note: User cannot add the same company twice at the same time. As once the company is added it is saved in QuickBooks Companies section. The user can add the same Company again after removing the Company from the selected list.**
{% endhint %}

* **Country:** It will display the country of QuickBooks Company. Initially, it will be empty, once the company data has been saved, you can see the country.
* **Base Currency:** It will display the base currency of QuickBooks Company. Initially, it will be empty, once the company data has been saved, you can see the base currency.
* **OAuth Version:** Select the OAuth version of the QuickBooks Company.
* **Use Sandbox:** Select **Yes** for configuring company of the **Sandbox** environment and **No** for configuring company of **Production/Live** environment.
* **OAuth Consumer Key/Client ID:** This depends on the OAuth version of QuickBooks i.e. **OAuth 1.0 or OAuth 2.0.** You need to copy the key obtained from the QuickBooks Developer/Production Account App as mentioned in the [Prerequisites.](https://docs.inogic.com/inolink/inolink-settings/enable-and-connect-dynamics-365-and-quickbooks-system/connect-and-configure-quickbooks#prerequisites)
* **OAuth Consumer Secret/Client Secret:** This depends on the OAuth version of **OAuth 1.0 or OAuth 2.0.** You need to copy the key obtained from the QuickBooks Developer/Production Account App as mentioned in the [Prerequisites.](https://docs.inogic.com/inolink/inolink-settings/enable-and-connect-dynamics-365-and-quickbooks-system/connect-and-configure-quickbooks#prerequisites)
* **Owning Business Unit:** Select which **Business Unit** to be considered for syncing the data from CRM to QB and vice-versa. If you select **Root/Parent BU,** then all CRM data would be integrated with configured QB Company. If you select a **child BU**, then only records of selected child BU would be integrated with QB.
* **User:** Select a **CRM user** under whom the records would be created (i.e. Owner of the record would be the selected CRM user).

![](<../../.gitbook/assets/Config QB Case1.2.png>)

![](<../../.gitbook/assets/Config QB Case1.3.png>)

![](<../../.gitbook/assets/Config QB Case1.4.png>)

After clicking on **Authorize & Save** button you will get the above message to proceed further. Once you click on **Yes** you will be redirected to **sign in your QuickBooks system**. There you need to select the required company with which you want to sync Dynamics 365 CRM.

![](<../../.gitbook/assets/QB Company Selection.png>)

![](<../../.gitbook/assets/Config QB Case1.6.png>)

After clicking on Connect you will get success message as shown below:

![](<../../.gitbook/assets/Config QB Case1.7.png>)

#### Case 2: Configuring Dynamics 365 CRM with Multiple QuickBooks Company.

Click on **(+) Add** button to configure more than one QuickBooks company and fill the required details as shown in below screenshot:

![](<../../.gitbook/assets/Config QB Case2.1.png>)

Now, you need to click on **Authorize & Save** button and you will re-directed to QuickBooks company list screen. In case you are not logged-in to QuickBooks then you will be re-directed to **Sign in** page. Next, select the required company with which you want to sync Dynamics 365 CRM.

![](<../../.gitbook/assets/Config QB Case2.2.png>)

![](<../../.gitbook/assets/QB Company Selection.png>)

![](<../../.gitbook/assets/Config QB Case2.4.png>)

After clicking on **Connect** you will get success message as shown below:

![](<../../.gitbook/assets/Config QB Case2.5.png>)

{% hint style="info" %}
**Note: If users configure the Root/Parent Business Unit for the first time in QuickBooks Companies then they cannot add and configure the multiple QuickBooks companies. Only when the Child Business Unit is added for the first time the user can configure multiple QuickBooks companies.**
{% endhint %}

![](<../../.gitbook/assets/Config QB Case2.6.png>)

{% hint style="info" %}
**Note: If users configure the Child Business Unit for the first time in QuickBooks Companies and try to add another company with Root Business Unit then the user gets the below error. Once the company is linked with particular child business unit then user can only select child business unit to configure another QuickBooks company.**&#x20;
{% endhint %}

![](<../../.gitbook/assets/Config QB Case2.7.png>)

{% hint style="info" %}
**Note: If the user wants to delete the selected company from InoLink Settings then he/she first needs to unlink the Accounts/Contacts/Products. After doing so there is an option of Remove QuickBooks Companies as shown below.**
{% endhint %}

![](<../../.gitbook/assets/Config QB Case2.8.png>)

#### InoLink Settings Display Window

![](<../../.gitbook/assets/Config QB Case2.9.png>)

{% hint style="info" %}
**Note: QuickBooks side the status displayed is 'Mappings installation in process. This may take a while'. For integration between two systems i.e. Dynamics 365 and QB requires mappings to say which field of QuickBooks must map with which field of Dynamics 365 and vice versa. This status indicates that the mappings installation is in process.**
{% endhint %}
