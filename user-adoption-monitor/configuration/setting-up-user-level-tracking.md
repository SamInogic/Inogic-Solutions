# Setting up User Level Tracking

User Adoption Monitor gives you the flexibility to control actions being tracked at the individual user level as well.

Given below are the steps to set up user level tracking:

* Navigate to **Advanced Settings --> Settings --> Security --> Users.**

![](../../.gitbook/assets/User\_Level\_1.png)

* Open a **User’s recor**d --> Click on **MANAGE USER TRACKING**.

![](../../.gitbook/assets/User\_Level\_2.png)

* It will open a pop-up as shown below:

![](../../.gitbook/assets/User\_Level\_3.png)

* The configuration UI at User Level would only list down those entities and actions which are enabled at System Level.

{% hint style="info" %}
**Note: For opportunity, we have enabled Win message/action, and since it is not available as a message/action in the UI, Opportunity will be listed here, but no options against it will be available.**
{% endhint %}

* In the UI, you are just allowed to select between two values for any action, the one which is selected at the System Level and the other as None.

{% hint style="info" %}
**Note: Customizing tracking capability of a particular user will end the synchronization with the System Level configurations. This means if you customize a user’s tracking capability, and later on, you enable tracking for an entity under Create action at System Level, then it will not take effect for that user. For a user to Sync with System-Level configurations again, you need to delete all of the modifications done for that user or you would need to customize the user’s tracking for the newly created action as well.**
{% endhint %}
