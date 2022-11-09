# Rule-Based Alert

Alert created with respect to specific conditions in CRM is called **Rule-Based Alert**. There are two types of Rule Based Alerts:

1. **Simple:** Create Alerts based on the View of an entity.
2. **Advanced:** Create Alerts based on filter criteria or conditions (conditions defined in Fetch XML).

### 1) Simple Alerts

Here are the steps to create Simple Alerts:

* Go to **Alerts4Dynamics App --> Alerts --> New** and fill in the following fields.
  * **Name:** Enter a suitable name for this Alert.&#x20;
  * **Alert Type:** Select the type of alert you are creating. Here you have the option to choose Rule Based or Announcement. Select Rule Based from the dropdown.&#x20;
  * **Entity Configuration:** Select the Entity Configuration.&#x20;
  * **Rule Mode:** Select **Simple**.  (This option only appears for Rule Based alerts.)

![](../../../.gitbook/assets/Rule\_1.png)

* Select the View for which Alert has to be created.

![](../../../.gitbook/assets/Rule\_2.png)

* Select the **Interval**.

<figure><img src="../../../.gitbook/assets/Simple 3.png" alt=""><figcaption></figcaption></figure>

1. **Poll Interval:** This is the duration after which the system checks if any new record has been created that satisfies the condition provided. (In above case, based on the condition of the selected view.)
   *   The workflow can run:&#x20;

       * **Only Once:** The alerts for all the records in selected view are created Only Once.&#x20;
       * **X Hour(s):** New records in the defined condition are checked for in every X Hour(s). If new records are found that satisfy the defined condition, new notifications are created for them.&#x20;
       * **X Day(s):** New records in the defined condition are checked for in every X Day(s). If new records are found that satisfy the defined condition, new notifications are created for them.&#x20;
       * **X Week(s):** New records in the defined condition are checked for in every X Week(s). If new records are found that satisfy the defined condition, new notifications are created for them.&#x20;
       * **X Month(s):** New records in the defined condition are checked for in every X Month(s). If new records are found that satisfy the defined condition, new notifications are created for them.

       ****
2. **Interval:** This is a numeric value of X in the Poll Interval.

* After entering values in the Alerts field click on Save and the alert will be created. Create new message from the Messages sub grid. To know how to Add New Message go to the [**Message** ](https://docs.inogic.com/alerts4dynamics/configuration/messages)section.

![](../../../.gitbook/assets/Rule\_4.png)

### 2) Advanced Alerts

Here are the steps to create Advanced Alerts:&#x20;

* Go to **Alerts4Dynamics App --> Alerts --> New** and fill in the following fields.
  * **Name:** Enter a suitable name for this Alert.&#x20;
  * **Alert Type:** Select the type of alert you are creating. Here you have the option to choose Rule Based or Announcement. Select Rule Based from the dropdown.&#x20;
  * **Entity Configuration:** Select the Entity Configuration.&#x20;
  * **Rule Mode:** Select **Advanced.**  (This option only appears for Rule Based alerts.)

![](../../../.gitbook/assets/Rule\_1.png)

* Enter the Fetch XML as per your conditions.

![](<../../../.gitbook/assets/Rule Ad\_1.png>)

* After creating the **Alert**, you can add a message to it. To know how to **Add New Message** go to the [**Message** ](https://docs.inogic.com/alerts4dynamics/configuration/messages)section.

![](<../../../.gitbook/assets/Rule Ad\_2.png>)
