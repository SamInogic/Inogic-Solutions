# Convert Opportunity/Quote/Order to Subscription Schedule

Subscription and Recurring Billing Management gives provision to users to convert their Opportunities, Quotes and Orders to Subscription Schedules on a single click.&#x20;

To convert an Opportunity to a Subscription Schedule, we need to create an Opportunity with the required details by following the steps given below:

* Navigate to **Subscription and Recurring Billing Management app --> Billing --> Opportunities --> Click on ’New’ button.**
* Enter the necessary details --> Click on **Save.**
  * **Bill To Customer:** The Customer to whom the invoice is sent and is responsible for paying the invoice. This could be the Reseller, the Customer, or a third party if they are being billed directly. If you bill the Customer directly, the Bill To Customer and Ship to Customer will be the same. This will appear as the **Bill To** on the Sales Invoice.&#x20;
  * **Ship To Customer:** The End Customer who would be actually using the product.&#x20;
  * **Margin Schedule:** This field will be populated based on ‘Bill To Customer’. If Margin schedule is defined on Bill To Customer, then that will be set on opportunity as well.&#x20;
  * **Margin Percentage:** This field is populated on the basis of Margin Schedule. Margin Percentage will be taken from the Margin schedule and this field is editable only by the user having the Security Role **'System Administrator'** or **'Subscription Management Admin'**.

![](<../../.gitbook/assets/Use case\_1.png>)

* If you wish to set the **Start Date** of your Subscription when you convert your opportunity to Subscription Schedule to any date other than the today’s date, you can do that by setting the value in the **'Start Date'** field in the **Subscription Management** tab on your Opportunity/Quote/Order.&#x20;
* If the Start Date is a date older than today’s date, then the field **'Create Transaction for this Billing Cycle'** is visible.&#x20;
* If the value of this field is set to **No** then after converting the Opportunity to Subscription Schedule the next transaction date on the Subscription Schedule is set to the **next billing cycle**. E.g., If start date on opportunity is **1st May 2021** and today is **26th May 2021**, then on converting to Subscription Schedule the next transaction date there will be set as **1st June 2021.**

![](<../../.gitbook/assets/Use case\_2.png>)

* If the value of this field is set to **Yes** then after converting the Opportunity to Subscription Schedule the next transaction date on the Subscription Schedule is set to the **current billing cycle**. E.g., If start date on opportunity is **1st May 2021** and today is **26th May 2021**, then on converting to subscription schedule the next transaction date there will be set as **1st May 2021.**
* Now add a product line to the opportunity --> Enter the necessary details given below:
  * **Existing Product.**&#x20;
  * **Show Subscription Fields:** Set the value in the **'Show Subscription'** field to **Yes** to view the other fields related to the subscription management.&#x20;
  * **Plan:** Select the plan as you want the pricing to be calculated.&#x20;
  * **Commitment Period:** Enter the commitment period to define the tenure for which you want to subscribe the product.&#x20;
  * **Subscriber Count:** Number of users who are going to use the product. This field is automatically set to **1** and locked if the plan selected is **Flat Fee**.&#x20;
  * **Price Per Billing Period/Price Per Unit:** This is the OOB Price Per Unit field renamed on the main form where the amount gets auto populated based on the plan selected and the value in the subscriber count.
  * **Convert to Subscription:** This line is added in the Subscription Schedule only if this field is set to **Yes** otherwise it is not included.&#x20;
  * **Is Taxable/ Tax Schedule:** If Tax Calculation Type on the configuration record is set as Standard, and the country selected is USA then **Is Taxable** field is visible or else **Tax Schedule** field is visible. These fields determine how the tax needs to be calculated.
* Click on **Save & Close.**

![](<../../.gitbook/assets/Use case\_3.png>)

* Next, add Add-Ons if required. On the line grid after selecting the product you can see the **'Add Add-Ons'** button. On click of this button below pop up is seen where the list of add-ons is seen associated with the product.&#x20;
* Now chose an appropriate plan for the add-on you wish to add.

{% hint style="info" %}
**Note: In the list of plans you can only see the plans having the billing frequency same as the one in the parent line.**
{% endhint %}

* Click on **'Add To List'** to add the add-on(s) to the opportunity.

![](<../../.gitbook/assets/Use case\_4.png>)

* Once the Opportunity is won, the **‘Convert to Subscription Schedule’** button becomes visible on the ribbon.

{% hint style="info" %}
**Note: When you are on Quote record the button is only visible after Activating the quote. And on Order record the button is always visible.**
{% endhint %}

* Next, click on **‘Convert to Subscription Schedule’** button on the ribbon.

![](<../../.gitbook/assets/Use case\_5.png>)

* A new Subscription Schedule is instantly created.

![](<../../.gitbook/assets/Use case\_6.png>)

{% hint style="info" %}
Note:&#x20;

* If there are two products in Product Line Items with different period of subscription such as monthly and yearly then two different Subscription Schedules will be created.&#x20;
* If different products with same Bill Every & commitment are added then only one schedule is created.&#x20;
* Write-in products are not carried over to Subscription Schedule.&#x20;
* Discount on the header is not carried forward to Subscription Schedule. If you want the discount to be carried over to Subscription Schedules then you will have to use the Margin Schedule.&#x20;
* Manual Discount on lines gets divided with the commitment period while being carried over to the Subscription Schedule.
* Once ‘Convert to Subscription’ button is clicked for any Quote or Order then the associated Opportunity or Quote records will be closed as ‘Won’.
{% endhint %}

### Price Breakdown

While adding products to your Opportunity/Quote/Order/Subscription Schedule it is imperative to select plans. The plans selected can be of different pricing models. Now one of the pricing models is Tiered for which the amount calculation is a bit complex as compared to others. So, to identify how we reached to an amount based on the subscriber count for a tiered pricing we have the entity **Price Breakdown** which is associated to **Opportunity Product/Quote Product/ Order Product/ Subscription Lines**.&#x20;

And for every product line as the name of the entity suggests we create the break down records which gives the details of the amount charged for a set of subscriber count based on the tier it falls in.

![](<../../.gitbook/assets/Use case\_7.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

