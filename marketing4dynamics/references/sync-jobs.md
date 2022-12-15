# Sync Jobs

Whenever you synchronize the data between Dynamics 365 CRM and Mailchimp, a Sync Job record is created for each of the records. Sync Job represents a sync request between Dynamics 365 CRM and Mailchimp.&#x20;

You can easily view these jobs against the records that is synced either from Mailchimp to Dynamics 365 CRM or from Dynamics 365 CRM to Mailchimp by following the steps mentioned below

Go to **Marketing4Dynamics App --> Settings --> Sync Jobs.**

![](<../../.gitbook/assets/Sync Jobs.png>)



![](<../../.gitbook/assets/Sync Jobs\_2.png>)

![](<../../.gitbook/assets/Sync Jobs\_3.png>)

* **Entity Type:** This section, specifies the type of record i.e., Contact, Lead, Marketing Activity, Marketing List, Campaign, Recipient and Tag associated with this job.&#x20;
* **Sync Status:** This field denotes the status of the job. It can hold the following values:&#x20;
  * **Success** – The job request was successfully processed.&#x20;
  * **Error** – There was an error in processing the request. The Error Description will provide detailed information about error.&#x20;
* **Source:** This field denotes the source system that generated this job. If it is Marketing, then the record is synced from Mailchimp to Dynamics 365 CRM; and if the source is CRM, then the record is synced from Dynamics 365 CRM to Mailchimp.&#x20;
* **Submitted By:** The user who have synced the record between the two systems.&#x20;
* **Submitted At:** The date and time when the syncing of record has taken place.
* **Processed At:** The time when the record is successfully synced following the direction specified by the user.&#x20;
* **Error Description:** Error description would provide the information about error. You need to resolve the error for it to be re-processed by the service.

### What triggers a job request?

A new Sync Job request is created when one of the following actions is performed in Dynamics 365 CRM:

* When **Sync Now** button is pressed while syncing an Audience.

![](<../../.gitbook/assets/Sync Jobs\_4.png>)

* When **Sync** button is clicked on a marketing list.

![](<../../.gitbook/assets/Sync Jobs\_5.png>)

* When **Sync Now** button is clicked on marketing list.

![](<../../.gitbook/assets/Sync Jobs\_6.png>)

* When **Sync Now** button is pressed while syncing a Campaign.

![](<../../.gitbook/assets/Sync Jobs\_7.png>)

* When a new tag is created in CRM.

![](<../../.gitbook/assets/Sync Jobs\_8.png>)

* When Mailchimp related fields (first name, last name, business phone & so on) are updated on Contact/Lead which is member of any marketing list that has **Sync Status** as **synced.**&#x20;
* On update of any synced record, a new sync job will be created.



{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
