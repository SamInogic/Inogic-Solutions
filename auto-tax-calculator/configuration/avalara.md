# Avalara

Auto Tax Calculator can integrate with Avalara's AvaTax product. AvaTax calculations will be used when the Avalara License field in Inogic Settings is populated with the **License Key** provided by Avalara.

![](../../.gitbook/assets/Avalara\_1.png)

![](../../.gitbook/assets/Avalara\_2.png)

You will find the following Avalara Auto Tax Calculator fields:&#x20;

* **Avalara License:** The license key assigned by Avalara for their product.
* **Avalara Account:** Account ID assigned by Avalara when you register for their product.&#x20;
* **Avalara URL:** URL to the Avalara Web Service used for Auto Tax Calculator.
* &#x20;**Enable Avalara Address Validation:** Flag to turn Tax Address Validation on or off. This will be No unless you have registered for Avalara.
* **Avalara Default Ship From Address:** The default Ship From address of the customer to use in calculating taxes. Here, you will get three options – **Business Unit Bill to Address, Business Unit Ship to Address and Alternate Location.**
  * **Business Unit Bill to Address** – If this option is selected than the Ship from Address is picked from the Business Unit Bill to Address of the Logged in User.&#x20;
  * **Business Unit Ship to Address** – If this option is selected than the Ship from Address is picked from the Business Unit Ship to Address of the Logged in User.&#x20;
  * **Alternate Location** – If this option is selected than you can select a record from the Location entity.
* **Avalara Commit on Post:** When using Avalara, the settings inform the systems if the user would like to commit a Tax Document at the same time they Post it.&#x20;
* **Avalara Company Code:** Identifies the company that helps Avalara access your company's tax profile.
* Once all the fields are duly entered, click on **Save** to complete the **Avalara integration**.

If Avalara is set as tax calculation type then on **Account/Contact** under Tax Processing tab additional fields are seen.

* **Business Identification Number:** Here, mention the unique identification number given to the business organization.&#x20;
* **Sales Tax Exemption Number:** Here, mention the unique number that will give exemption from Sales Tax.&#x20;
* **Customer Usage Type:** Select any option from the drop-down that defines the organization. For example - **Federal Government, Local Government, Charitable Organization, etc.** _(This field is used while calculating tax with ‘Avalara’ integration)._

### Tax Actions

On Header entities and line items we have added a fly out button called Tax Actions to execute Avalara commands. This fly out button has 7 options.

![](<../../.gitbook/assets/Tax Actions\_1.png>)

* **Ping Service:** This helps to verify that your connection is working.&#x20;
* **Validate Address:** Resolves an address against Avalara’s address validation system. If the address can be resolved, this API provides the latitude and longitude of the resolved location.&#x20;
* **Adjust Tax:** Replaces the current transaction uniquely identified by this URL with a new transaction.
* **Cancel Tax:** Voids the current transaction uniquely identified by this URL.&#x20;
* **Commit Tax:** Marks a transaction by changing its status to Committed.&#x20;
* **Post Tax:** Marks a transaction by changing its status to Posted.&#x20;
* **Get Tax:** Records a new transaction in Avalara’s AvaTax API and calculates tax and updates in CRM.

