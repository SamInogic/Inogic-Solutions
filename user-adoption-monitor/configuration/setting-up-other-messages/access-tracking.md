# Access Tracking

CRM Access Tracking is a feature to track access of the Dynamics CRM users. It enables the managers to monitor the CRM access of their team members by tracking various web activities performed by them in the CRM manually.

{% hint style="info" %}
**Note: This feature doesn’t give the actual daily login count of a CRM user. It instead provides brief detail on the number of times a user accesses a CRM.**
{% endhint %}

#### STEPS TO TRACK USER’S CRM ACCESS

* The first step to track user’s CRM Access is to **Enable Auditing**. For this, navigate to **Settings --> Auditing (under ‘System’ group).**

![](<../../../.gitbook/assets/Access Trac\_1.png>)

* It opens Audit window as shown below. Click on **‘Global Audit Settings’**.

![](<../../../.gitbook/assets/Access Trac\_2.png>)

* Click on **‘Auditing’** tab. Check **‘Start Auditing’** and **‘Audit user Access’** settings as shown below:

![](<../../../.gitbook/assets/Access Trac\_3.png>)

* After enabling **Auditing,** create a **‘User Adoption Entity Configuration’** record for user login. For this, navigate to **User Adoption Monitor App** **--> Entity Configurations** (under **‘User Adoption Monitor’** group).

![](<../../../.gitbook/assets/Access Trac\_4.png>)

* Click on **(+ New)** to create a new User Adoption Entity Configuration record for login (If no record is already created).

{% hint style="info" %}
**Note: Whether the entity configuration record has already been created or not can be verified from the Entity Configurations home view.**
{% endhint %}

* The User Adoption Entity Configuration record should always be created with the following attributes as shown in the screenshot below:
  * **Entity Label:** “systemuser”&#x20;
  * **Entity Schema:** “systemuser”&#x20;
  * **Message:** “login”&#x20;
  * **Period:** “Daily”&#x20;
  * **Polling:** Select the interval period after which tracking will be conducted.&#x20;
  * **Preferred Start Time:** Select the time to start the tracking.

![](<../../../.gitbook/assets/Access Trac\_4.5.png>)

{% hint style="info" %}
**Note: The period should always be selected as ‘Daily’ as this feature only works for daily tracking.**
{% endhint %}

* Once the Entity Configuration record is created, the User Adoption Monitor will track the CRM Access of each logged in user. The tracking details can be reviewed either from the **‘systemuser-login’** entity configuration record as below or by navigating to the **Settings --> User Adoption Monitor --> Trackings.**

![](<../../../.gitbook/assets/Access Trac\_5.png>)

