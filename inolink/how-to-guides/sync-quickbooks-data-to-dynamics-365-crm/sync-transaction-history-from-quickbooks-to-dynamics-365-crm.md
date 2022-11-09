# Sync Transaction History from QuickBooks to Dynamics 365 CRM

Transaction History is synced automatically by the **InoLink High Priority** service set in Service Scheduling section within the QuickBooks to Dynamics 365 CRM feature option.

InoLink brings in all of the transaction types from QuickBooks like Estimates, Invoices, Sales Receipt, Payments, Credit Memos etc. to Dynamics 365 CRM. These are visible on each of the Dynamics 365 CRM account and contact record as shown below:

![](<../../../.gitbook/assets/Sync Tranc\_1.png>)

This is the same view as can be seen on the Customer Card in QuickBooks.

![](<../../../.gitbook/assets/Sync Tranc\_2.png>)

{% hint style="info" %}
**Note: All of the transactions are imported and stored within the Dynamics 365 CRM database. This allows you to implement Field Level Security to handle access to Accounting Details by only authorized Dynamics 365 CRM users.**
{% endhint %}

There are certain **Custom Entities** shipped along with the solution. These custom entities are developed so as to save the details of enabled features, sync request, payments made and sales transactions performed in them accordingly.&#x20;
