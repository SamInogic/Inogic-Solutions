# Track Opening of Records

You can also track the touch of the records by tracking the opening of the records. To track the opening of the records, certain customization is required. For example, consider a scenario where you want to track the touch/opening of the account records.

* Create a record of the User Adoption Entity Configuration Entity with the following details;
  * **Entity Label:** Account (entity on which you need track open/read)&#x20;
  * **Entity Schema:** account (schema name of the entity)&#x20;
  * **Message:** ikl\_open&#x20;
  * **Period:** Daily (period you want to track)

![](../../../.gitbook/assets/Track\_1.png)

* Add the following User Adoption Monitor JavaScript libraries which are shipped along with the product to the ‘Account’ form in the same order as mentioned below;

**ikl\_/UserAdoption/scripts/jquery.js**

![](../../../.gitbook/assets/Track\_2.png)

**ikl\_/UserAdoption/scripts/UserAdoption.CrmJS.js**

![](<../../../.gitbook/assets/UAM Track records\_2.png>)

**ikl\_/UserAdoption/scripts/UserAdoption.WebAPI.js**

![](<../../../.gitbook/assets/UAM Track records\_1.png>)

**ikl\_/UserAdoption/scripts/UserAdoption.ExecuteReadAction.js**

![](../../../.gitbook/assets/Track\_4.png)

![](../../../.gitbook/assets/Track\_5.png)

* Then finally call the ‘getRecordDetails’ function on the Form OnLoad event as shown in the below screenshot from the Java Script Library ikl\_/UserAdoption/scripts/UserAdoption.ExecuteReadAction.js (which has already been included in the form) onload of the form and then save and publish the customizations.

![](../../../.gitbook/assets/Track\_6.png)

![](../../../.gitbook/assets/Track\_7.png)

![](../../../.gitbook/assets/Track\_8.png)

{% hint style="info" %}
**Note:**&#x20;

* **You need to make the above mentioned changes on each of the form being used in case you have multiple forms configured for role-based access.**
* **To make the above mentioned changes one needs to have the System Administrator privilege.**
{% endhint %}



{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

