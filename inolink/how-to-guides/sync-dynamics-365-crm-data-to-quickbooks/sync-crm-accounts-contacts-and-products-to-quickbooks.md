# Sync CRM Accounts, Contacts & Products to QuickBooks

To sync Dynamics 365 CRM records to QuickBooks, you can follow the steps below:

* Open record you want to sync with QuickBooks. For example, open Account from Dynamics 365 CRM. You will find the **'Promote'** button in the ribbon bar as shown below:

![](<../../../.gitbook/assets/Sync Acc\_1.png>)

* Once you click on this button, the Link Status will be updated to **'To be Linked'** as shown in the below screenshot:

![](<../../../.gitbook/assets/Sync Acc\_2.png>)

* In the background this will initiate a Link Job to be processed by the service to move the update from CRM to QuickBooks.
* A link Job for this account with Link status set as **'Queued'** as shown in the below image will be created.

![](<../../../.gitbook/assets/Sync Acc\_3.png>)

* Similarly, you can schedule jobs for Dynamics 365 CRM to QuickBooks update for **Contact, Product, Quote and Invoice.**
* To unlink a record so that updates are not taken over from one system to the other, you need to click on the **UnLink** button in the ribbon bar.

![](<../../../.gitbook/assets/Sync Acc\_4.png>)

* Clicking on this button will change the Link Status on the record to Unlinked as shown in the below image:

![](<../../../.gitbook/assets/Sync Acc\_5.png>)

* This button is only available on records that are already integrated with QuickBooks.
* Ensure the feature is enabled using the **InoLink Settings Tool**. Go to **InoLink Settings --> Check for the required feature in Dynamics 365 CRM to QuickBooks synchronization.**
* If the job was successfully processed the Link Job status is updated to **Success.** If there was an error in processing the job request, it would be updated to **Error** and the error description would be available in the **Error Description** field on the Link Job.
* When Link job is processed successfully, the Account Link status is updated to **'Linked'.** In case of an error, it is set to **'Error'.**





















