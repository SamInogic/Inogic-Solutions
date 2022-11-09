# Sync CRM Quotes, Orders & Invoices to QuickBooks

InoLink allows Quotes, Order and Invoices to be promoted from Dynamics 365 CRM to QuickBooks once.

Once you are ready to move the transaction to QuickBooks, set the Link status to **'To be linked'** by using the Promote button available in the ribbon bar as shown below:

![](<../../../.gitbook/assets/Sync Quote\_1.png>)

![](<../../../.gitbook/assets/Sync Quote\_2.png>)

This will create a Link Job with **'Queued**' status that will be processed by the enable feature of syncing the Invoice from Dynamics 365 CRM to QuickBooks.

Once Invoice is successfully transferred to QuickBooks the Link job status is updated to **'Success'** and Invoice link status is changed to **'Linked'** as shown below:

![](<../../../.gitbook/assets/Sync Quote\_3.png>)

In case of an error, the link job status is updated to **'Error'** and so is the Invoice record Link Status field.

In case of a successful transfer of transaction from Dynamics 365 CRM to QuickBooks, the QuickBooks document No. is copied to CRM for a quick reference to the associated QuickBooks record.

{% hint style="info" %}
**Note: Once a transaction has been successfully promoted to QuickBooks, it cannot be updated in Dynamics 365 CRM.**
{% endhint %}

