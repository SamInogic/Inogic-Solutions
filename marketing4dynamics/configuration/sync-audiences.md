# Sync Audiences

Mailchimp Audience is where you keep all your contacts/members, Tags and then use campaigns to sent mails to your specific audiences or Tags.&#x20;

This section will enable you to choose which Mailchimp Audiences you want to sync to CRM from the list as there could be more than one Audiences in Mailchimp. You can sync one or more Mailchimp Audience.&#x20;

From this section, you can select Mailchimp Audience from the list of Audiences and sync to CRM but it requires to tie/associate CRM Marketing List to it.&#x20;

Upon syncing Audience, the synchronization process starts in the background which syncs Mailchimp Tags and creates Mailchimp Members as Contact/Lead based on the associated Marketing List in the CRM.

To sync audiences, follow the steps given below:

* Go to **Settings --> Setup --> Sync Audiences.**

![](<../../.gitbook/assets/7 (4).png>)

* Click on **‘Manage’**.

![](<../../.gitbook/assets/8 (3).png>)

* Now select the **Marketing List** in CRM that you want to map with Mailchimp Audience. Here, the Mailchimp members will be mapped with the contacts/leads in CRM marking list. If there are no existing marketing list then create a new one. If your selected Marketing List is of type **Contact** then **Mailchimp members** would be created as **Contacts in CRM** whereas if type is **Lead** then it would be created as **Leads in CRM.**

{% hint style="info" %}
**Note: You can select only static marketing list of type (Target At) Lead and Contact. Account type of Marketing List is not supported.**
{% endhint %}

![](<../../.gitbook/assets/9 (6).png>)

* In this case, we have created a new Marketing List. For this, go to **Marketing List** --> Click on **‘Search’** icon --> Click on **‘New Marketing List’.**

![](<../../.gitbook/assets/10 (3).png>)

* Fill the required details in marketing list and click on **‘Save’.**

![](<../../.gitbook/assets/11 (8).png>)

![](<../../.gitbook/assets/12 (7).png>)

* A new marketing list is created. Now go back to **‘Sync Audiences’** and add this Marketing List.

![](<../../.gitbook/assets/13 (7).png>)

* Click on **‘Sync Now’**.

![](<../../.gitbook/assets/14 (4).png>)

* A pop-up will appear stating that the sync process has started --> Click on **Ok.**

![](<../../.gitbook/assets/15 (4).png>)

* **The status is now changed to 'In-progress' which indicates that the synchronization of Audience is in under process.** (See Status section to know meaning of each Sync Status).

![](<../../.gitbook/assets/16 (1).png>)

* Refresh or revisit the page to see current Sync Status.

![](<../../.gitbook/assets/17 (1).png>)

* Another way to verify **Sync Status** is to navigate to **Settings --> Audiences**.

![](<../../.gitbook/assets/18 (2).png>)

* Once sync is complete, there will be two distinct changes in CRM data. Firstly, Mailchimp Tags will get synced to CRM.&#x20;

![Mailchimp Tags](<../../.gitbook/assets/19 (2).png>)

* The tags in Mailchimp will be be synced and can be seen in both **‘Tags’** and **‘Audiences’** entity. To verify this, go to **Audiences --> Tags** or **Settings --> Tags**.

![](<../../.gitbook/assets/20 (2).png>)

![](<../../.gitbook/assets/21 (1).png>)

* Secondly, Mailchimp Members will get created as Contacts/Leads and associated with the selected Marketing List. Members can be seen under the **Marketing List** that you **map** with **Mailchimp Audience**. You can identify the Marketing List by **Audience Lookup.**

![](<../../.gitbook/assets/22 (2).png>)

![](<../../.gitbook/assets/23 - Copy.png>)
