# Link Jobs

Whenever you synchronize data between Dynamics 365 CRM and QuickBooks, a Link Job request is created for individual records. Link Job represents a sync request between Dynamics 365 CRM and QuickBooks.

**You can easily view these jobs against any Dynamics 365 record that is enabled for sync between Dynamics CRM and QuickBooks by following the steps mentioned below;**

To see all the link jobs, go to **Settings > InoLink > Link Jobs** as seen in the screenshot below;

**In Classic Web:**

![](<../../.gitbook/assets/Link Jobs\_1.png>)

**In Unified Interface:**

![](<../../.gitbook/assets/Link Jobs\_2.png>)

You can view these jobs against any Dynamics 365 **** CRM record that is enabled for Dynamics 365 CRM to QuickBooks sync.

![](<../../.gitbook/assets/Link Jobs\_3.png>)

**1) Entity Type:** This section, which specifies the record **Account, Contact, Product, Quote, Order** and **Invoice** associated with this job.

![](<../../.gitbook/assets/Link Jobs\_4.png>)

![](<../../.gitbook/assets/Link Jobs\_5.png>)

**2) Link Status:** This field denotes the status of the job. It can hold the following values:

* **Queued** – This denotes the job is in the queue and waiting to be picked up by the service.&#x20;
* **Success** – The job request was successfully processed.&#x20;
* **Error** – There was an error in processing the request. The Error description would provide detailed information about error. You need to resolve the error and change the status of the job back to **Queued** for it to be re-processed by the service.

**3) Source:** This field denotes the source system that generated this job. If it is **Accounting**, then the record is synced from **QuickBooks to Dynamics 365 CRM**. And if the source is **CRM** then the record is coming from **Dynamics 365 CRM to QuickBooks.**

**4) Submitted By:** The user who have promoted the record between the two systems.

**5) Submitted At:** The date and time when the promoting of record have taken place.

**6) Processed At:** The time when the record is successfully synced following the direction specified by the user.

**7) Accounting ID:** It is the reference number to identify the record promoted in QuickBooks system from Dynamics 365 CRM.

**8) Processed Count:** This represents the number of times the record was processed and this is used while data is synced from QuickBooks to Dynamics 365 CRM, if the record gets into error status.

**9) Error Description:** Error description would provide the detailed information about error. You need to resolve the error and change the status of the job back to Queued for it to be re-processed by the service.

### What triggers a job request?

A new Link Job request is created when one of the following actions is performed in Dynamics 365 CRM:

* **Link Status** for a record of entities like Account, Contact, Product, Quote and Invoice is set as '**To be Linked'** once clicked on **Promote** button.&#x20;

![](<../../.gitbook/assets/Link Jobs\_6.png>)

A Link Job is executed with the link status updated as **Success** and on record the status updated as Linked. This works for Account, Contact and Product Entities.

![](<../../.gitbook/assets/Link Jobs\_7.png>)

* On **update** of **linked records** the Link Job will be created.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

