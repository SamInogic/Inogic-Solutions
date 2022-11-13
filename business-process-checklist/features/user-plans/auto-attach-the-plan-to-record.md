# Auto-Attach the Plan to Record

Plans defined by the manager will automatically get attached to the records as per the matched criteria.

**Below is an example:**

Now, the manager has created a plan for Lead Nurturing for the Lead entity, where the criteria are set as "Lead Source as "Web"

<figure><img src="../../../.gitbook/assets/connect records 1.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Note: If there are no criteria set this plan will be auto-attached to records.
{% endhint %}

* **Criteria for the execution of the Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will run against those records for which the criteria match). Select either **Simple** or **Advanced**.
  * **Simple:** Connect records based on the View of an entity.
  * **Advanced:** Connect records **** based on filter criteria or conditions (conditions defined in Fetch XML). e.g. If you want to attach a plan to open leads with lead source as web then you have to enter the Fetch XML for it. Below is the Fetch XML for the open lead where the lead source is the web.
* Navigate to **Sales Hub -->** Go to **Leads -->** Create a **New Lead.**

<figure><img src="../../../.gitbook/assets/connect records  lead 1.png" alt=""><figcaption></figcaption></figure>

* &#x20;Go to **Business Process Checklist App** **--> Plan Step Items,** here you can see your record is now automatically connected to the plan.

<figure><img src="../../../.gitbook/assets/Connect record final ss.png" alt=""><figcaption></figcaption></figure>
