# Create Games

Once the rules are set, the next step is to create games. In Gamifics365, you can create three different types of games at individual and team levels namely; **Challenge, Face-off** and **Race**.

* **Challenge:** In Challenge, individual players or teams will be given a task to be achieved in a limited amount of time. The one who achieves it wins the game.
* **Face-off:** In Face-off, two players will be pitted against each other to achieve a given task.
* **Race:** In Race, all the players will be given a common target and the one who achieves it first wins the game.

To create engaging games within Dynamics 365 CRM, just follow the simple steps given below:

* Navigate to **Gamifics365 app --> Administration --> Games -->** Click on **‘+New’**.

![](../../.gitbook/assets/Games\_1.png)

* OR you can directly navigate from **Gamifics365 Studio -** In **Gamifics365 Studio**, click on **Games** --> Then click on **‘Manage Games’** --> Click on **‘+New’**.

![](../../.gitbook/assets/Games\_2.png)

In the **‘New Game’** window, you can see 6 different tabs – **Game Details, Game Rules, Game Badge & Rewards, Earned Points** and **Earned Badges & Rewards.** The first tab is **‘Game Details’** which is further divided into 5 sections. To create a new game, fill in the necessary game related information in these 5 different sections and click on **Save**.

![](<../../.gitbook/assets/Config Games\_6.png>)

![](<../../.gitbook/assets/Config Games\_7.1 (1).png>)

**Section 1 – Name this game and provide description**

In this section, you have to name the game and provide a brief description of the game.

![](../../.gitbook/assets/Games\_3.png)

**Section 2 – When you want to start and end the game?**

In this section, you have to give the starting date and ending date for the game. The game will be played only for this period. And if the end date is not added then the game will go on.

![](../../.gitbook/assets/Games\_4.png)

**Section 3 – Select the type of game and type of players you want to add to this game.**

In this section, there are two fields:

*   **Select Type of Game:** Select either of the game type – **Challenge, Face-off,** or **Race**.

    * **Challenge:** For the Challenge game type **‘End Date’** is mandatory.
    * **Face-off:** In the Face-off game type, ‘**Game is between’** field will be auto-populated with the value **‘Users’**.
    * **Race:** In the Race game type, a new target section will be added to the form where you have to define the target for the players.&#x20;



![](<../../.gitbook/assets/Game type.png>)

![](../../.gitbook/assets/Games\_5.png)

* **Game Is Between:** Here you can decide whether the game will be for individual players or will be between teams. There are three options to select from – **Fantasy teams, Teams,** and **Users**.

![](../../.gitbook/assets/Games\_8.1.png)

* In Fantasy Teams, you can create a team for playing games and determine the number of players to be added to each team. For example – A sales manager can create a fantasy team of five members which can include two persons each from the Sales and Marketing department and one person the from Accounting department.

![](<../../.gitbook/assets/Games\_9 (1).png>)

* In Teams, you can create teams within sales departments such as Alpha Sales Team and Beta Sales Team, and set a common target for them to achieve.
* In the Face-off game type, ‘Users’ will be automatically selected. This is because face-off is always between two individual players.

**Section 4 – Who can join this game?**

In this section, there are two fields:

* **Behaviour of Game:** Here, you can set the behavior (mode) of the game as **Public** or **Private**. Public games will be open to all those players who are allowed to join the games. Who is allowed and who is not allowed to participate in games can be clearly defined in **‘Allowed Roles’**. Whereas, in **Private** games, only managers can add players to the game.&#x20;
* **Allowed Roles:** Here, you can define which roles are suitable for the game. This is to make sure that only a select few players holding a particular position in the organization are allowed to join the game in Public mode. If this field is kept blank then the game will be open to all the players. In Private mode, this field is not necessary.

![](<../../.gitbook/assets/Games\_11 (1).png>)

**Section 5 – Allow players to join game if the Game is in-progress?**

Select **Yes** or **No**. By default, this section is kept as **‘No’**. If yes is selected, then you can add players in between the ongoing games.

![](<../../.gitbook/assets/Config Games\_9.png>)

Once the **‘Game Details’** is saved, move on to the next tab – **Game Rules.** Here click on **‘+New Game Rule’.**

![](../../.gitbook/assets/Games\_6.png)

![](../../.gitbook/assets/Games\_7.png)

Now in the **‘Game Rule Template’** field, select the game rule for the game. Here, you can either select existing game rules from the game rule template or create new game rule on the spot.

![](../../.gitbook/assets/Games\_8.png)

Once the game rule template is selected, the rest of the fields will be auto-populated with the required details. Now click on **Save & Close**.

![](../../.gitbook/assets/Games\_9.1.png)

The next tab is – **Players.** You can add individual players or teams depending upon the game you want to create. Here, click on **‘+New Player’** to add users or teams.

**For adding individual players:**

![](../../.gitbook/assets/Players\_2.png)

**For adding teams:**

![](../../.gitbook/assets/Players\_1.png)

**For adding fantasy teams:**

![](<../../.gitbook/assets/Fantasy team.jpg>)

In the case of a team, give an appropriate name to the team and save it. After saving it, start adding players to the team by clicking on **‘+New Player’**.

![](../../.gitbook/assets/Games\_10.png)

The last tab is – **Game Badge & Rewards**. You can add Badges and Rewards that are to be conferred upon the winners of the game. Here, click on **‘+New Game Badges/Rewards’** to add them to the game.

![](../../.gitbook/assets/Games\_11.png)

Now, select the badges/rewards and define the points after earning which the player will get these badges/rewards. Click on **Save**. Once it is saved, additional sections - **Description and User Profile Description** - will automatically appear on the screen in editable format. Here, you can edit the content as per your requirement which will be automatically reflected on the mobile app. For easy understanding, the content/descriptions can be updated in any language of your choice.

![](<../../.gitbook/assets/Badges\_2 (1).png>)

![](../../.gitbook/assets/Games\_12.png)

The **‘Earn Badge Description’** will be shown under the **Game Details** screen in the Canvas app.

![](<../../.gitbook/assets/Canvas app Badges\_1.png>)

While the **‘User Profile Description’** will be shown under the **User Profile** screen in the Canvas app.

![](<../../.gitbook/assets/Canvas app User Profile\_1.png>)

Once the game configuration is completed, click on the **‘Go Live’** button on the ribbon bar.

![](<../../.gitbook/assets/Go Live new\_1.png>)

After clicking on **‘Go Live’**, if **** the **** current date is the start date of the game, then the status of the game will be changed to **‘In progress’** and if the start date is a future date then the status of the game will be changed to **‘Scheduled’**. Once the game is over, the status will be shown as **‘Completed’**.

![](../../.gitbook/assets/Games\_13.png)
