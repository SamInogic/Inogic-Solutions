# Set up Security

**SharePoint Security Sync** has the following security roles:

{% tabs %}
{% tab title="SharePoint Security Sync Administrator" %}
**SharePoint Security Sync Administrator** has the privilege to create and modify '**Entity Configurations**', '**Connector entity records'**, '**Security Templates'**, and '**Bulk Migration Jobs'**.
{% endtab %}

{% tab title="SharePoint Security Sync User" %}
**SharePoint Security Sync User** will be able to '**Read**' and can create '**Bulk Migration Job'** and utilize all the Attach2Dynamics features in SharePoint such as Upload, Download, Create, Delete, etc.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
**Note: It is necessary to assign any one of the above security roles to use SharePoint Security Sync Solution**
{% endhint %}

Follow the simple steps given below to assign security roles to CRM users.

* Navigate to **SharePoint Security Sync App** --> **License Registration** Page --> Click on the **Assign Security Role** button.

![](../../.gitbook/assets/Sec\_1.png)

* A confirmation dialog box will appear. Click on **Ok.**

![](../../.gitbook/assets/Sec\_2.png)

The **SharePoint Security Sync user** security role will be now assigned to all the users present in Dynamics 365 CRM.

OR, you can follow another alternative method mentioned below:

* Go to **Advanced Settings** --> **Settings** --> **Security**.

![](<../../.gitbook/assets/f (1).png>)

* Select **Users**

![](<../../.gitbook/assets/g (2).png>)

* Select user --> Click on **MANAGE ROLES**

![](<../../.gitbook/assets/i coopy.png>)

* Click on any one of the security roles --> Click **OK**.

![Admin Role](<../../.gitbook/assets/Set Security\_1 (1).png>)

![User Role](../../.gitbook/assets/i.png)
