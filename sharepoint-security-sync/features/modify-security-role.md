# Modify Security Role

Apart from syncing privileges, we can also modify the security roles in Dynamics 365 which will be replicated in SharePoint. To understand this better, we have created two Business Units apart from root business unit that are: Marketing and Sales. Sales is the parent business unit of Marketing and in this example, we are working with Account entity.

Now, Sales BU has two users, James and Rhea. James is salesperson who has user level read/write access and Rhea as a Sales Manager has Business Unit read/write access.

Marketing BU has one user Joe who is Marketing Manager and has organization level read/write access.

#### Scenario 1 Visibility:

**James:** With user level access, he can see only his records.

![](../../.gitbook/assets/Modify\_1.png)

**Rhea:** With BU level access, she can see records of James and her own.

![](../../.gitbook/assets/Modify\_2.png)

**Joe:** With org level access he can see all records.

![](../../.gitbook/assets/Modify\_3.png)

#### Scenario 2 Visibility:&#x20;

Now we change the access level of Rhea to Parent Child Business Unit, and keep the security level access of Joe and James the same. With this Rhea will be able to see the records of both Joe and James.

![](../../.gitbook/assets/Modify\_4.png)

Apart from these modifications the user level access comes into action even when a security role is associated/dissociated to/from a user/team or a member is added/removed from a team or security role deleted.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}



