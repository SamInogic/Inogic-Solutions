# Sync Marketing List/Members

In previous section, we synced **Mailchimp Audience** to **Dynamics 365 CRM** and eventually synced Mailchimp **Members** to CRM **Contacts/Leads**.&#x20;

In this section,  we will sync **Dynamics 365 CRM Marketing List** to **Mailchimp** which will eventually sync CRM **Contacts/Leads** to **Mailchimp**.&#x20;

Also, it will only sync those contacts/leads which were **added** to the **Marketing List.**&#x20;

This is helpful when you want to plan and execute marketing activities through Mailchimp targeting the customers in Dynamics 365 CRM. You can create **Marketing List** in CRM with **contacts/leads** and then with a **single click** you can initiate the **sync** process for that Marketing List. Now, any **new member added** to this Marketing List will get **automatically** **synced** to **Mailchimp**. Also any **updates** made to any **members** of Marketing List will get **automatically synced** to **Mailchimp.**&#x20;

**For Example:** You have imported a list of contacts to Dynamics 365 CRM of those who have attended the webinar or any promotional event. Now, you want to push those contacts to Mailchimp so that the Marketing team can send them further exclusive promotional campaigns. In this case, you can create a new Marketing List **'2021 Event Attendees'** in CRM and add all those contacts into it.

Now to sync this Marketing List to Mailchimp, follow the steps given below:

* Go to **Settings --> Setup --> Sync Marketing List/Members --> Click on ‘Manage’.**

![](<../../.gitbook/assets/Sync Mkt List\_1.png>)

* This will be redirected to Marketing List **home grid.**

![](<../../.gitbook/assets/Sync Mkt List\_2.png>)

* Or, directly go to **Marketing4Dynamics App --> Marketing --> Marketing Lists.**

![](<../../.gitbook/assets/Sync Mkt List\_3.png>)

* Click on **'+ New'** to create a new Marketing List.

![](<../../.gitbook/assets/Sync Mkt List\_4.png>)

![](<../../.gitbook/assets/Sync Mkt List\_5.png>)

* In new Marketing List, enter the following information:
  * **Name:** The name of Marketing List.&#x20;
  * **List Type:** Select either **Static** or **Dynamic**. You can sync both types of Marketing List.&#x20;
  * **Target At:** Select either **Contact** or **Lead**. You can add either contact or lead to the marketing list based on the option selected. **Account type** of Marketing list is **not** supported.&#x20;
  * **Audience:** Select the **Mailchimp Audience** with which you want to sync this Marketing List and its members.&#x20;
  * **Tag:** Select the **Tag** that you want to associate to a member in Mailchimp. The selected tag will get attached to member in Mailchimp.

![](<../../.gitbook/assets/Sync Mkt List\_6.png>)

* In **Members** tab, now you can add members from either static or dynamic. Use **'Manage Members'** button to add members to the Marketing list.

![](<../../.gitbook/assets/Sync Mkt List\_7.png>)

* As soon as you save the Marketing List, you will see a **'Sync'** button. Only **System Administrator** or **Marketing4Dynamics Administrator** can sync the Marketing List.

![](<../../.gitbook/assets/Sync Mkt List\_8.png>)

* Once the **'Sync'** button is **clicked,** a dialog box will appear asking **confirmation**. After getting confirmation, the synchronization process will get started in the background.

![](<../../.gitbook/assets/Sync Mkt List\_9.png>)

* Now the **Sync Status** will change into **'In Progress'**.

![](<../../.gitbook/assets/Sync Mkt List\_10.png>)

* Once the process is completed, the Sync Status will change into either **'Synced'** or **'Error'**.

![](<../../.gitbook/assets/Sync Mkt List\_11.png>)

* Sync Status of each individual member can also checked.

![](<../../.gitbook/assets/Sync Mkt List\_12.png>)

* During the process, it checks for any existing members in the selected Mailchimp Audience. And if there are members then it updates the members (profile information) or else it will create new members and attach the selected Tags to them.

![](<../../.gitbook/assets/Sync Mkt List\_13.png>)

&#x20;

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

