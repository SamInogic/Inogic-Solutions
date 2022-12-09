# Set User Sequence

The **'Sequence'** field in the **'User Workload'** entity field is used for deciding the sequence of the users. This Sequence field is a numeric field and starts with 0.&#x20;

Only **Lead Assignment Administrator** or **System Administrator** can change the sequence of the user. An administrator can directly change the sequence from the sub-grid and would not need to open each record to change the sequence.

![](../../.gitbook/assets/Sequence\_1.jpg)

The records will get assigned from lowest to highest sequence and will work with both **Round Robin** and **Capacity** algorithm.&#x20;

By default all users will have **0** sequence. If no sequence is provided then the records will get assigned by date when the user workload is created (i.e. date when a user added in the queue).&#x20;

You cannot add duplicate sequence number for two or more users. It will restrict the user from adding same sequence number for the users.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

###
