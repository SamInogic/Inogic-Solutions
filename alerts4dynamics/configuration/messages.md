# Messages

Every Alert can have multiple messages attached to it. Once an Alert is created, messages can be added to it. For example, multiple messages can be added for a **Holiday Alert**, such as **Holiday on 30th June**, **Holiday on 20th July**, etc.

<figure><img src="../../.gitbook/assets/Message 1.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note: Message cannot exist independently without an Alert.**
{% endhint %}

Given below are the steps to add multiple messages to an existing Alert.

* Click on **'+ New message'** and a New Message page will open.

![](../../.gitbook/assets/Message\_2.png)

*   Enter the value in the following Fields:

    * **Name:** This is the name of the message you are trying to create.&#x20;
    * **Alert:** This is the Alert for which you are creating the message.&#x20;
    * **Message Text:** Enter the message you would like to display in the notification or send to the users as email. Users can also pass dynamic values here for e.g. Account {name} has been created, where {name} stands for Account’s name.&#x20;
    * **Alert Level:** This can be categorized as **Information, Warning** and **Critical**. This determines the severity level of the Alert you are trying to create.&#x20;
    *   **Alert As:** This is the mode of notifying your users. It can be done as:&#x20;

        * **Pop-Up:** The notification with message will pop-up post clicking the global notification bell button.&#x20;
        * **Form Notification:** Choosing an alert as **'Form Notification'** will show up the **‘Display As’** field. Under this field, you can select either **‘Dialog’** or **‘Bar’**. If you select **‘Dialog’** then alert will be shown as a dialog sliding out from the right of the screen immediately after opening the record and if you choose **‘Bar’** then the notification will be displayed under the ribbon in the form of a bar.
        * **Email Notification:** The message will be sent to the users through email.
        * **User Preference:** Gives a provision to set the preference to receive an alert.


    * **Is Dismissible:** Gives provision to configure the alert as either dismissible or non dismissible. If **‘Yes’** is selected, alert becomes dismissible and if **‘No’** is selected then alerts cannot be dismissed. **(Note: Is applicable to all type of alerts)**.
    * **Auto Dismissible:** Gives provision to configure the alerts as auto-dismissible/non auto-dismissible. If **‘Yes’** is selected then alerts will be automatically dismissed once the defined condition is no more satisfied. If **‘No’** is selected then alerts cannot be dismissed automatically even if it moves out of the defined condition in the alert configuration. **(Note: Is applicable to Rule-based and Event-based alerts. However, it only supports Record-based alert if the alert is configured using advanced message type.)**
    * **Email Workflow:** If the **‘Email Notification’** is selected in ‘**Alert As’** field then the user needs to create an OOB workflow for sending an email. We can send email notification to not only the CRM users but also the customers as well.



![](../../.gitbook/assets/Message\_3.png)

![](../../.gitbook/assets/Message\_4.png)

![](../../.gitbook/assets/Message\_5.png)

* Next is setting the start and end date for the message.
  * **Process Start Date:** Process Start Date is a mandatory field. It is the date from when the notifications start getting created. This date cannot be prior to the date when the message is created. If you enter a previous date you will get the error message - **Process Start Date should be greater than or equal to current date.**&#x20;
  * **Process End Date:** This is the date when notifications stop getting created. If you leave this field blank the notifications will continue getting created indefinitely. Process end date cannot be before Process Start Date, in case such a value is entered following error comes - **Process End Date should be greater than or equal to Process Start Date.**&#x20;
  * **Display Until:** It defines for how much period the notification should be displayed. If user hasn’t dismissed the notification.&#x20;
  * **Language:** Alert messages can be created in multiple languages.

![](../../.gitbook/assets/Message\_6.png)

{% hint style="info" %}
**Note: Languages need to be enabled for creating messages in multiple languages. If the created Notification Message (language) is in English then the notification will be displayed only for users whose User Interface language is English.**
{% endhint %}

* Next is the notification audience section. Here, you have to fill the following fields:
  * **Include Users:** If you specify the set of users here, alerts will be shown to only these users.
  * **Exclude Users:** If you specify the set of users here, alerts will be shown to every user in organization except for these users.&#x20;
  * **Security Roles:** If you select security roles here, alerts will be shown to these security roles.
  * **Teams:** If you select Teams here, alerts will be shown to these teams.

{% hint style="info" %}
**Note:**

* **If Include Users/Exclude Users/Security Roles are left blank, then the notifications will be shown to everyone.**&#x20;
* **Include Users/Exclude Users have priority over Security Roles.**
{% endhint %}

These fields allow you to select your viewing audience for alert message. Dynamics values as well as static values can be selected in these fields.&#x20;

For example, in below image we can see in **Include Users** field **Owning User** and **Owning User Manager** are selected which are dynamic values and in **Exclude Users** field **‘Scott Hamells’** (CRM User) is selected.

![](../../.gitbook/assets/Message\_7.png)

* After creating a message, save it and click on **Activate** to make it live.

![](../../.gitbook/assets/Message\_8.png)

* To edit a message click on **Draft.**&#x20;

![](../../.gitbook/assets/Message\_9.png)

{% hint style="info" %}
**Note: You can set state as Draft or edit a message only before Process Start Date. You cannot set the state to Draft or edit that message after the process of creating notifications has started because it becomes Read Only.**
{% endhint %}

![](../../.gitbook/assets/Message\_10.png)



### Message Type

There are two **Message Types** in Alerts4Dynamics:

* Simple (Default)
* Advanced

#### 1) Simple Message:

In Simple mode, user can configure the notifications like Message Text, specifying notification audience which can be dynamic users, teams and security roles as well.&#x20;

For **Notification** and **Email Audiences** we can select user type lookup fields which are available on the entity form will be shown in the **Include Users, Exclude Users** dropdown and for **Teams**, similarly to user we can select team lookups fields.

<figure><img src="../../.gitbook/assets/simple message.png" alt=""><figcaption></figcaption></figure>

#### 2) Advanced Message:

In Advanced mode, consider a scenario in which the alert is configured for Invoice but we want the notification to be shown on related Account record.&#x20;

Similarly, we want the Notification and Email Audiences related to the account like **‘One to Many’** and **‘Many to Many’** relationship.

<figure><img src="../../.gitbook/assets/advance message.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/advance message 2.png" alt=""><figcaption></figcaption></figure>

