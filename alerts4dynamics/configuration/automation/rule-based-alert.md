# Rule-Based Alert

In order to understand how this provision works let’s consider a scenario where user wants an alert to auto dismiss once the account record moves out of **‘My Active Accounts’** entity view.

Given below are the steps to configure workflow to auto-dismiss alerts:

* Create a new alert of type **‘Rule Based’** and define the rule mode as **‘Simple’** with a view as **‘My Active Accounts’.**

<figure><img src="../../../.gitbook/assets/1 (276).png" alt=""><figcaption></figcaption></figure>

* Add a message to this alert.

<figure><img src="../../../.gitbook/assets/2 (21).png" alt=""><figcaption></figcaption></figure>

* Set **‘Auto Dismissible’** as **‘Yes’**.

<figure><img src="../../../.gitbook/assets/3 (19).png" alt=""><figcaption></figcaption></figure>

* Navigate to **Accounts** --> **My Active Accounts** --> **Open** **any record**. Here, an alert will be displayed as a Form dialog post opening the record and it will continue showing up as long as it satisfies the rule defined in the alert configuration i.e. **‘My Active Accounts’**.

<figure><img src="../../../.gitbook/assets/4 (14).png" alt=""><figcaption></figcaption></figure>

* Now deactivate this account record so that it will move out of **‘My Active Accounts’** entity view.

<figure><img src="../../../.gitbook/assets/5 (17).png" alt=""><figcaption></figcaption></figure>

![](<../../../.gitbook/assets/Event\_6 (1).png>)

* Once deactivated, a record is moved from **‘My Active Accounts’** view to **‘Inactive Accounts’** which means it no more satisfies the rule (‘My Active Accounts’) defined in the alert configurations. As soon as this happens, the alert will be auto dismissed in about 5-10 seconds. So now, if we switch to **‘Inactive Accounts**’ view and open the account record, you will no longer see an alert. **(Note: It might take a while for an alert to get auto dismissed.)**

<figure><img src="../../../.gitbook/assets/7 (14).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/8 (5).png" alt=""><figcaption></figcaption></figure>

