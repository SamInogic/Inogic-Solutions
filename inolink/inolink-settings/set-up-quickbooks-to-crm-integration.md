# Set up QuickBooks to CRM integration

In this section, we will dive deep into the process of syncing data from QuickBooks to Dynamics 365 CRM.

![](<../../.gitbook/assets/QB to CRM\_1 (2).png>)

### Customer

Using this option you can enable the feature to sync the data from QuickBooks to Dynamics 365 CRM **Accounts/Contacts**. After clicking on **Customer** you will get the below displayed window.

![](<../../.gitbook/assets/QB to CRM\_Cust\_1.png>)

Here, you need to enable the feature by switching **ON** the button at top right corner which will then turn green.

![](<../../.gitbook/assets/QB to CRM\_Cust\_2.png>)

#### Name Matching Criteria:

You have two options here:-

* **Exact** – It will look for an exact name match.&#x20;
* **Pattern** – It will perform a pattern match to cover for any typos in data entry in the two systems. E.g. **InfoMedia** and **IfnoMedia** will be treated as the same record and updated instead of creating duplicates.

#### Deadlock Win:

You have two options here i.e. **CRM** or **QuickBooks.**

If you have configured a two-way sync, use this property to define the application that will hold the last change, in case changes are made in both systems to the same record.

#### Allow Primary contact to sync:

Set this as **Allow** if you would like the **Contact** from **QuickBooks** to be Synced with the **Account or Contact** field in **Dynamics 365 CRM**.

Given that Accounting Contact may be different from the Business Contact stored in Dynamics 365/CRM, you may not want to override the Primary contact set in Dynamics CRM from QuickBooks and vice versa. In that case, set this option as **‘Do not Allow’.**

#### Last Modified From:

Only those Customer records would sync from QuickBooks to CRM which were created or modified after the specified date.

After clicking on Save button, depending on whether you have services on or off, you’ll get pop-up message**.** If your services are off, you’ll get the below message:

![](<../../.gitbook/assets/QB to CRM\_Cust\_3.png>)

On clicking **No**, this screen will be closed. On clicking **Yes,** **Service Scheduling** screen would open.

If your services are on, you’ll get success message.

![](<../../.gitbook/assets/QB to CRM\_Cust\_4.png>)

There are **3 cases** that will help you to analyze and understand how the data will be replicated in Dynamics 365 CRM when the data is synced from QuickBooks to Dynamics 365 CRM.

#### Case 1 – Let’s take an example of a customer that is having Company, First name and Last name details in QuickBooks.

This customer is saved as an **Account** same as that of the **company** name and **Primary contact** same as that of the First name and Last name of the customer.

QuickBooks side the customer with **Company, First and Last name** looks like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_5.1.png>)

Dynamics 365 CRM side after syncing the **Account** along with the **Primary** contact looks like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_5.2.png>)

#### Case 2 - Let’s take an example of a customer having Company and sub-customer details in the record.

This customer is saved as an **Account** with the same details as that of the **Company** and **Parent Account** field is populated with the details same as that of the **sub-customer.**

QuickBooks side the customer with **Company** and **sub-customer** looks like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_6.1.png>)

Dynamics 365 CRM side after syncing the **Account** along with **Parent Account** will look like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_6.2.png>)

#### Case 3 - Let’s take an example of a customer having a first and last name details in the record.

The customer is saved as **Contact** in Dynamics 365 CRM with the same details as that of the first and last name.

QuickBooks side the customer with **First and Last name** looks like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_7.1.png>)

Dynamics 365 CRM side after syncing the **contact** looks like:

![](<../../.gitbook/assets/QB to CRM\_Cust\_7.2.png>)

### Product

Using this option you can enable the feature to move and sync the data of **Products** from QuickBooks to Dynamics 365 CRM. After clicking on **Product** you will get the below displayed window.

![](<../../.gitbook/assets/QB to CRM\_Prod\_1.png>)

**Product feature Setting for US QuickBooks Company**

![](<../../.gitbook/assets/QB to CRM\_Prod\_2.png>)

{% hint style="info" %}
**Note: User should select the Base Price List based on the Country of QuickBooks Company.**
{% endhint %}

Here, you need to enable the feature by switching ON the button at top right corner which will then turn green.

#### Name matching criteria:

You have two options here:-

* **Exact** – It will look for an exact name match.&#x20;
* **Pattern** – It will perform a pattern match to cover for any typos in data entry in the two systems.

#### Deadlock Win:

You have two options here i.e. **CRM** or **QuickBooks.**

If you have configured a two-way sync, use this property to define the application that will hold the last change, in case changes are made in both systems to the same record.

#### Unit Group & Unit:

Products in Dynamics 365 CRM need to have the Unit Group and Unit specified. Provide the default Unit Group and Unit to be set for new products created in Dynamics 365 CRM from QuickBooks.

#### Base Price List:

Products in Dynamics 365 CRM need to have a Default Price List provided. This default value will be used for Products created from QuickBooks. Price List Items for the Products would be created for this Price List.

{% hint style="info" %}
**Note: While selecting the Base Price List user needs to verify if the currency of the price list is matching with the country of QuickBooks.**
{% endhint %}

![](<../../.gitbook/assets/QB to CRM\_Prod\_3.png>)

{% hint style="info" %}
**Note: User needs to select same price list that is defined as a Base Price List in Product feature for Dynamics 365 CRM to QuickBooks or else user will get the below error message.**
{% endhint %}

![](<../../.gitbook/assets/QB to CRM\_Prod\_4.png>)

{% hint style="info" %}
**Note: If you are already using Price List in Dynamics 365 CRM, specify the Price List you have created to store the product prices.**
{% endhint %}

#### Decimal Supported:

The Default value to be set for the Decimal supported attribute of the Product in Dynamics 365 CRM.

#### Last Modified From:

Only those Product records would sync from QuickBooks to CRM which were created or modified after the specified date.

After clicking on **Save** button you will get below success message.

![](<../../.gitbook/assets/QB to CRM\_Prod\_5.png>)

### Transaction History

Using this option you can enable the feature to create and update the details from QuickBooks histories within the Dynamics 365 CRM. After clicking on **Transaction History** you will get the below displayed window.

![](<../../.gitbook/assets/QB to CRM\_Tran\_1.png>)

**InoLink** brings in all of the transaction types from **QuickBooks** like **Credit Memos Estimates, Received Payments, Sales Receipt, Estimate, Invoices,** etc. to **Dynamics 365 CRM.** These are visible on each of the Dynamics 365 CRM **Account** and **Contact** record as shown below.

![](<../../.gitbook/assets/QB to CRM\_Tran\_2.png>)

This is the same view as can be seen on the **Customer Card** in **QuickBooks.**

![](<../../.gitbook/assets/QB to CRM\_Tran\_3.png>)

{% hint style="info" %}
**Note: All of the transactions are imported and stored within the Dynamics 365 CRM database. This allows you to implement Field Level Security to handle access to Accounting Details by only authorized Dynamics 365 CRM users.**
{% endhint %}

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
