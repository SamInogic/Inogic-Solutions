# Set Game Rules

Every game has certain rules. Before creating any game, it is mandatory to set the rules based on which games will be played. In Gamifics365, you can set the game rules in **‘Gamifics365 Studio’**. It is a platform to create and manage game rules for different types of games within Dynamics 365 CRM.

To set the game rules, just follow the simple steps given below:

* Navigate to **Gamifics365 app --> Administration --> Gamifics365 Studio** --> Click on **‘+New Rule’**.

![](<../../.gitbook/assets/Game Rule\_1.png>)

* This will open the **‘Create Game Rule’** form. Here, you can set the conditions for game rules based on which game will be played.
  * **Rule Name:** Give an appropriate name to the Game Rule.
  * **Short Name:** Give a short name to the rule.
  * **Description:** Give a short description of the rule.
  * **What type of record is this?:** Select the entity to which the record belongs to.
  * **Select the event for the selected type of record:** Define the occasion for which the rule is created. For example – When a new lead record is created, when the status of a record is updated, etc.
  * **Which date should we use?:** Define which date should be used as the cut-off date for completing a certain task that will earn points for the players, i.e., the date on which a record is created, modified, or won. For example – Actual Close Date, Final Decision Date, etc.
  * **Who should get the score:** Select to whom the score should be given. In this field, multiple options can be selected.
  * **Calculate score by:** There are two options available – Actual field value or Fixed points.
    * **Actual field value:** The actual value will be considered here, such as Actual Revenue, Budget Amount, etc. You can select the appropriate value from the dropdown list. For example – In a game of two players ‘Actual Revenue’ is selected for the actual field value. Now, player A has closed a deal worth $10,000.00 and player B has closed a deal worth $7500.00 then the score of player A will be 10,000 and score of player B will be 7500. Here the winner is player A.
    * **Fixed points:** Here, a fixed point is defined for each deal closed by the player like 100, 200, 500, etc. For example – Suppose for each deal closed by the player will be awarded 100 points then as per the above example both player A and player B will score 100 points each for closing the sales deal. Here, it will be a tie between two players.
  * **Choose how to filter the record further:** Defines the criteria of the records on which the game rule will be applicable. Select either Simple or Advanced.
    * **Simple:** Here you can select any ‘View’ from the dropdown. All the records coming under this view will be considered while playing the game
    * **Advanced:** Here, you can further define and set criteria for records through fetch XML. This will restrict the rule to select few records instead of all records under a single view. For example – In a game between two sales reps, each sales rep is given a target to achieve total sales of $5000 in a month. But a condition is given that only a sales deal worth $500 or more will be considered. So, even if the sales rep closes a deal worth $450, it will not be counted.

![](<../../.gitbook/assets/Game Rule\_2.png>)

* Once the required fields are filled, click on **‘Create Rule’**.

![](<../../.gitbook/assets/Game Rule\_3.png>)

* The new rule will be created and can be seen on Gamifics365 Studio.

![](<../../.gitbook/assets/Game Rule\_4.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}



