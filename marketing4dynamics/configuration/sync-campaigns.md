# Sync Campaigns

In previous sections, we synced Mailchimp **Audiences, Tags** and **Members** to Dynamics 365 CRM and then we synced CRM **Marketing List (Contacts or Leads)** to **Mailchimp**.&#x20;

These two sections ensure that the customer data in both Mailchimp and Dynamics 365 CRM is up to date. Because of this Marketing Team can be assured of the customer data and will not need to depend on manual data creation or data imports in Mailchimp. Marketing team can go ahead and run campaign against the subscribed members.&#x20;

In this section we will sync Mailchimp campaigns and members activities in CRM. This will help CRM users to get marketing stats directly in CRM and will further help to decide future sales strategies.&#x20;

All the campaigns in Mailchimp which has been sent to the subscribers will be synced to Dynamics 365 CRM. To sync the campaigns, follow the steps given below:

* Go to **Settings --> Setup --> Sync Campaigns --> Click on ‘Manage’.**

![](<../../.gitbook/assets/Sync Camp\_1.png>)

* Select the campaign **-->** Enter the number of days in **‘Auto Sync Activities’ -->** Click on **‘Sync Now’**. In the **‘Campaign Sent On’** section, the latest campaign will be listed on top followed by the previous campaign and so on. The ‘**Auto Sync Activities’** section is to determine the period for which the campaign activities will be synced to CRM.

![](../../.gitbook/assets/Campaign\_2.png)

* A pop-up will appear stating that the sync process has started **-->** Click on **Ok.**

![](<../../.gitbook/assets/Sync Camp\_2.png>)

* After a short while, the campaign activities in Mailchimp will be synced to Dynamics 365 CRM and can be seen in ‘**Campaigns’** entity.

![](<../../.gitbook/assets/Sync Campaigns\_1.png>)

*   Here, a summary of the campaign will be available which will include the following details:

    * **Recipients:** It displays the list to whom the mails have been sent and its status.

    <img src="../../.gitbook/assets/Sync Campaigns_2.png" alt="" data-size="original">    <img src="../../.gitbook/assets/Sync Campaigns_3.png" alt="" data-size="original">&#x20;

    * **Marketing Lists:** The Marketing List associated with the campaign. For example, if the campaign is sent to the whole audience then the campaign get associated with the Marketing List in CRM where the Audience lookup value is equal to the Audience of Mailchimp. If the campaign is sent to the particular Tag members then the campaign get associated with the Marketing List in CRM where Audience Lookup is the Mailchimp Audience and Tag Lookup is equal to the Tag selected on the Campaign in Mailchimp.
    * **Marketing Activities:** The list of activities tracked by the Mailchimp for that campaign. For example, to whom was mail sent, who opened mail, who clicked on links, who unsubscribed, and bounced mails.

{% hint style="info" %}
**Note: Marketing4Dynamics does not supports synchronization of Campaigns which has been sent to segments.**
{% endhint %}

* In the **‘Statistics’** section, the following details will be available:
  * **Open Rate:** The number of unique opens divided by the total number of successful deliveries.&#x20;
  * **Unique Opens:** The number of unique opens.&#x20;
  * **Opens:** The total number of opens for a campaign.&#x20;
  * **Successful Deliveries:** The number of recipients who successfully received the mails.&#x20;
  * **Click Rate:** The number of unique clicks divided by the total number of successful deliveries.&#x20;
  * **Unique Clicks:** The number unique clicks.&#x20;
  * **Clicks:** Total number of clicks on the links by the recipients.

![](<../../.gitbook/assets/Sync Campaign\_1.png>)

* Further you can see the graphical representation of the above data.

![](<../../.gitbook/assets/Sync Campaign\_3.png>)

* The same data will be available in Mailchimp without graphical representation.

![](<../../.gitbook/assets/Sync Campaign\_2.png>)

* In **Contacts** also, each record will show the marketing activities in its timeline.

![](<../../.gitbook/assets/Sync Campaigns\_4.png>)

* After the sync is completed the **‘Last Sync Time’** will be populated in the **‘Sync Campaigns’** section. This workflow will run **once** every day updating the **‘Last Sync Time’** till the sync period is completed.

![](<../../.gitbook/assets/Sync Campaigns\_5.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

