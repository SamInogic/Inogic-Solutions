# Drill down through Relationships

The way **‘Drill down’** feature behaves with connection relationships is a little different than how it works with other entities within CRM. In general, this feature allows user to drill through the relationship N-level further down and see its associated entity records.

Let’s consider a scenario where user wants to see the associated contact connection record of a particular account in CRM and further drill the connection down to see its few other associated account records.

#### Pre-requisites for above scenario:

* An account record should exist in the CRM system having at least one associated contact connection further holding a few associated account records.
* Map My Relationship view control must already be configured for an account entity.

### Drill down feature configuration steps:

* Firstly, navigate to **Map My Relationships --> Entity Configuration --> New**.
* Create and save the entity configuration as shown below:
  * **Name:** Give a valid name for configuration.&#x20;
  * **Entity:** Account (as we want to see the connection record of an account).&#x20;
  * **Set As Default:** Can be ignored for this occasion since this field won’t play any role here in this scenario because this is not going to be used as a child configuration.&#x20;
  * **Entity Node Image:** Set an image as per requirement.&#x20;
  * **Allowed Actions:** Set quick activity actions as required.

![](<../../../.gitbook/assets/Child Conf\_1.png>)

* Similarly, fill the fields to configure relationships:
  * **Relationship Type:** One to Many (Account holding one to many relationship with connections).&#x20;
  * **Relationship:** account\_connections1(connection).&#x20;
  * **Relationship Node Image:** As required.&#x20;
  * **Allowed Actions:** As required.&#x20;
  * **View to show fields on Tooltip:** Active Connections.&#x20;
  * **Use Default Configuration:** Yes (Another entity configuration for **‘Contact’** will also be created to see further associated records of contact connection record).

![](<../../../.gitbook/assets/Child Conf\_2.png>)

![](<../../../.gitbook/assets/Child Conf\_3.png>)

* Next, let’s create another entity configuration for **‘Contact’** to see further associated account records of the contact connection, and set it to default as **‘Yes’** as shown below:
  * **Name:** Give a valid name for configuration.&#x20;
  * **Entity:** Contact&#x20;
  * **Set As Default:** Yes (Here, we need to set this as ‘Yes’ which is already enabled in the connection relationship configuration that we have configured earlier above).&#x20;
  * **Entity Node Image:** As required.&#x20;
  * **Allowed Actions:** As required.

![](<../../../.gitbook/assets/Child Conf\_4.png>)

* In a similar way, fill the respective fields for configuring relationships
  * **Relationship Type:** One to Many.&#x20;
  * **Relationship Type:** account\_primary\_contact(account).&#x20;
  * **Relationship Node Image:** As required.&#x20;
  * **Allowed Actions:** As required.&#x20;
  * **View to show fields on Tooltip:** My Active Accounts.&#x20;
  * **Child Configuration:** Leave this blank since we don’t want to see any further associated entity records of the account(s).

![](<../../../.gitbook/assets/Child Conf\_5.png>)

![](<../../../.gitbook/assets/Child Conf\_6.png>)

{% hint style="info" %}
**Note - At a time, application will accept only one entity configuration set as default to be used as a child configuration to see the associated entity records of the connection (associated account records of contact connection in this instance).**
{% endhint %}

* Now, navigate to **Account entity** --> Open a **record** --> Click on **‘Relationship Connection’**.

![](<../../../.gitbook/assets/Child Conf\_7.png>)

* Double click on **‘Connections’** to expand it and it will show a connection record.

![](<../../../.gitbook/assets/Child Conf\_8.png>)

* Now further expand (double click) contact record **‘Cathan Cook’** and it will show you the association of accounts with the contact connection record.

![](<../../../.gitbook/assets/Child Conf\_9.png>)

* Again double click on **‘Accounts’** to expand it and it will show the associated account records of the contact connection record **‘Cathan Cook’**.

![](<../../../.gitbook/assets/Child Conf\_10.png>)

Using this approach, you will be able to drill down through the connection relationship to see its related entity records i.e. **Accounts** in this illustration.

