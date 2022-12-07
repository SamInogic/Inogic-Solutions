# Set User Preference

Alerts4Dynamics gives a provision of setting up the preferences to receive an alert which completely leaves it to the users to choose how they want to receive an alert.&#x20;

### Scenario 1:&#x20;

Admin configures an alert as **‘User Preference’**. Let’s say an admin does not have any specific preference to receive an alert.&#x20;

**Admin – No preference**&#x20;

But there are another two users having a preference to receive an alert in the following manner:&#x20;

**User 1 – Email Notification**&#x20;

**User 2 – Pop up**&#x20;

#### Outcome:&#x20;

Admin will not be able to see an alert since an alert is configured as only **‘User Preference’** and admin did not set any preference to receive an alert.&#x20;

**User 1** will receive an alert only through **Email.**&#x20;

**User 2** will be able to see an alert only as a **Pop up**.

#### Steps to set User Preference

* Navigate to **Advanced settings** --> **Settings** --> **Security** --> **Users**.

![](<../../.gitbook/assets/Set Pref1\_1.png>)

* Open the user record.

![](<../../.gitbook/assets/Set Pref1\_2.png>)

* **For Admin** - Do not set any preference (make sure it is **blank**).

![](<../../.gitbook/assets/Set Pref1\_3.png>)

**For User 1** – Set the preference as **‘Email Notification’**.

![](<../../.gitbook/assets/Set Pref1\_4.png>)

**For User 2** – Set the preference as **‘Pop up’**.

![](<../../.gitbook/assets/Set Pref1\_5.png>)

* Next, select user from whom an email is to be sent as **‘From’** in Alerts4Dynamics configurations. For this, navigate to **Alerts4Dynamics app** --> **Configurations.**

![](<../../.gitbook/assets/Set Pref1\_6.png>)

* Open the configuration record.

![](<../../.gitbook/assets/Set Pref1\_7 (1).png>)

* Select the user (this is the user from whom an alert will be sent via email to that user who has preference to receive an alert set as **‘Email Notification’**).

![](<../../.gitbook/assets/Set Pref1\_8 (1).png>)

* Configure and activate the message.

![](<../../.gitbook/assets/Set Pref1\_9 (1).png>)

* Once the message is activated - **User 1** will receive an alert only through an **Email.**

![](<../../.gitbook/assets/Set Pref1\_10.png>)

The user will be directed to the record page by clicking on the record link available in the email body.

![](<../../.gitbook/assets/Set Pref1\_11.png>)

In case of an announcement alert being sent through an email, there will be no such link since announcements are not record specific.

![](<../../.gitbook/assets/Set Pref1\_12.png>)

**User 2** will get an alert only through **Pop-up.**

![](<../../.gitbook/assets/Set Pref1\_13.png>)

![](<../../.gitbook/assets/Set Pref1\_14.png>)

### Scenario 2:

Admin configures an alert as both **‘User Preference’** and **‘From Notification – Dialog’**. Let’s say the admin does not have any specific preference to receive an alert.

**Admin – No preference**

**User 1 – Email Notification**

**User 2 – Pop-up**

#### Outcome:

**Admin** will be able to see an alert only as a **‘Form Notification – Dialog’.**

**User 1** will receive an alert through an **‘Email’** as well as **‘Form Notification – Dialog’.**

**User 2** will be able to see an alert as both **‘Pop-up’** and **‘Form Notification – Dialog’.**

#### Steps to set User Preference

* Set individual user preferences for an alert. **Admin – No preference.**

![](<../../.gitbook/assets/Set Pref2\_1.png>)

**User 1 – Email Notification.**

![](<../../.gitbook/assets/Set Pref2\_2.png>)

**User 2 – Pop-up.**

![](<../../.gitbook/assets/Set Pref2\_3.png>)

* Configure the alert message.

![](<../../.gitbook/assets/Set Pref2\_4 (1).png>)

* Once the message is activated; **Admin** will be able to see an alert only as a **Form Dialog**.

![](<../../.gitbook/assets/Set Pref2\_5.png>)

**User 1** will be notified through both **Email** as well as **Form Dialog.**

**As Email Notification:**

![](<../../.gitbook/assets/Set Pref2\_6.png>)

**As Form Dialog:**

![](<../../.gitbook/assets/Set Pref2\_7.png>)

**User 2** will be able to see an alert both as **Pop-up** and **Form Dialog.**

**As Pop up:**

![](<../../.gitbook/assets/Set Pref2\_8.png>)

**As Form Dialog:**

![](<../../.gitbook/assets/Set Pref2\_9.png>)

{% hint style="info" %}
**Note: - User preference and Email notification cannot be used together.**
{% endhint %}

![](<../../.gitbook/assets/Set Pref2\_10.png>)

**Reason:** User is required to create a workflow for alert as **‘Email Notification’** where they will decide which of the users to be picked as an audience of this email notification. In addition to this, no separate notification is created for an alert as **‘Email Notification’**, it would be sent directly as email.

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
