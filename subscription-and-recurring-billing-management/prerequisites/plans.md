# Plans

Plans are where you define the pricing structure for your product depending on the pricing model and currency for a respective billing cycle.

### How to create a New Plan:

* Navigate to **Subscription and Recurring Billing Management app --> Products --> Plans -->** Click on **‘New’** button.
* Enter necessary details in the required fields --> Click on **Save.**
  * **Name:** Give appropriate name to the plan or it is auto populated with the combination of **Product Name + Interval + Bill Every + Pricing Model.**
  * **Product:** The product for which the plan is being created.&#x20;
  * **Currency:** The currency in which the price needs to be defined.&#x20;
  * **Pricing Model:** This field defines the pricing model based on which the pricing for the product shall be applied. It provides the following options –
    * **Flat Fee:** Price charged irrespective of number of users. For example; 199$ for 1 month subscription.&#x20;
    * **Per Unit:** Price charged for per unit. For example; If 5$ for 1 user, then for 10 users it will be – 10 x 5$ = 50$.&#x20;
    * **Tiered:** Per unit price charged on the basis of different tiers. For example; Price for tier of (1 – 10) users is 2$ and tier of (11 – 20) is 1$. Then for 15 users the cost will be – (10 x 2$) +(5 x 1$) = 25.&#x20;
    * **Volume:** Price charged on the basis of volume. For example; Price range for (1 – 10) users is 2$ and (11 – 20) is 1$. Then for 15 users the cost will be – 15 x 1$ = 15.&#x20;
    * **Stairstep:** Price charged based on different brackets. For example; Price bracket for (1 – 10) users is 20$ and (11 – 20) is 30$. Then for 15 users the cost will be – 30$.
  * **Billing Unit:** This field defines the period for which bills will be generated – **Day, Week, Month, Year**. Select any of these options.&#x20;
  * **Price Per Billing Unit:** This field appears when **‘Per Unit’** pricing model is selected. It is used to define the product pricing for per unit.

![](<../../.gitbook/assets/Plan\_1 (1).png>)

The **Details** section defines the pricing ranges for **Tiered, Volume** and **Stairstep** pricing model. Here, additional pricing ranges or new plan details can be added as and when needed.

To add a pricing range where you want to define the pricing for when the user count is greater than 500, you need to set the **Starting Range** as **501** and then set the **Ending Range** to a very larger number such as **999999** as shown below:

![](../../.gitbook/assets/Plan\_2.1.png)

### How to add New Plan Details:

* Navigate to **Subscription and Recurring Billing Management app --> Products --> Plans --> Select a plan** or you can directly navigate to **Subscription and Recurring Billing Management app --> Plans --> Select a plan.**
* Click on the button **‘New Plan Details’.**

![](<../../.gitbook/assets/Plan Details\_1.1.png>)

* Enter the details in required fields --> Click on **Save.**
  * **Name:** Name the plan detail. For example, 1 - 20.&#x20;
  * **Starting Range:** Define the starting range of the plan.&#x20;
  * **Ending Range:** Define the ending range.&#x20;
  * **Price per Billing period:** Define the price for the particular range.&#x20;
  * **Plan:** This field is pre-populated with the Plan to which this plan detail is associated.

![](<../../.gitbook/assets/Plan Details\_2.png>)

{% hint style="info" %}
**Note: Plan Details grid on Plan is an editable grid.**
{% endhint %}
