# Proration

In simple terms, proration is adjusting a customer's bill amount to reflect any changes made to the existing plan in the middle of a billing cycle.&#x20;

Let’s understand this with a use case.&#x20;

A Datum Corporation is a customer with a current subscription for Click2Clone product. Subscription Schedule has been prepared for this customer for generating invoices.

![](../../.gitbook/assets/Proration\_1.png)

![](../../.gitbook/assets/Proration\_2.png)

Now the customer wants to increase the user count from **15** to **115** i.e., the customer wanted to add more 100 users within the same subscription period. Here, we will create a new Quote for the customer. After creating the Quote, in the **‘Subscription Management’** tab add the existing Subscription Schedule.

![](../../.gitbook/assets/Proration\_3.png)

Next, add the product line items.

![](../../.gitbook/assets/Proration\_4.png)

Now in **‘Apply Charges’** field there are three options available – I**mmediately, Immediately (Prorated), Start from Next Billing Cycle and Custom.**

**Immediately:** The first invoice was generated on 1st March and the subscription is for 3 months i.e., till May. And the user count was increased on 4th March. With this option the user count will be immediately included and a new invoice for whole 3 months will be generated and billed to the customer.&#x20;

**Immediately (Prorated):** In proration, the customer will be billed from the day user count is increased i.e., the remaining days of March (28 days) and for April & May.&#x20;

**Start from Next Billing Cycle:** Here, the increased user count will be included in the next billing cycle i.e., for April & May.

**Custom:** The new charges will be applicable from the date set in 'Billing Start Date' and the new invoice will be generated accordingly. For example, if the user count was increased on 13th March then the invoice can be generated for past date i.e. **10th March** or it can be generated for future date i.e. **15th March** and based on this date the charges will be calculated for the remaining period. Once **‘Custom’** option is selected, a new field termed **‘Billing Start Date’** will appear from where you can set the necessary date.

![](<../../.gitbook/assets/Apply Charges\_3.png>)

![](<../../.gitbook/assets/Apply Charges\_4.png>)

Now after adding the line item to increase the user count, activate the quote as the customer has given approval and then **convert** it to **Subscription Schedule** to update the existing Subscription Schedule selected on Quote.&#x20;

Once the quote is converted to Subscription Schedule, the subscriber count of the subscription line gets updated to **115** and depending upon the **Apply Charges** option selected the amount gets adjusted.

![](../../.gitbook/assets/Proration\_5.png)

Shown below are the adjustments for each Apply Charge Option:

* **Immediately:** A negative invoice for the entire amount charged previously gets created along with a positive invoice with the new amount.

![](../../.gitbook/assets/Proration\_6.png)

* **Immediately (Prorated):** A negative invoice for the prorated amount gets created along with a positive invoice with the prorated amount.

![](../../.gitbook/assets/Proration\_7.png)

* **Start from Next Billing Cycle:** No negative invoice gets created and from the next billing cycle the invoice gets generated with the updated amount and subscriber count.

![](../../.gitbook/assets/Proration\_8.png)

* **Custom:** If past date is selected then a negative invoice for the prorated amount gets created along with a positive invoice with the prorated amount. Let’s consider another example where the annual subscription of the product is from Jan 2021 to Dec 2021 and the customer has increased the subscriber count of the product from 50 to 100 on current date ( 22nd August) which will increase the subscription amount from 600 to 1200. Now, due to company policy, the invoice is generated for 20th August, which is back dated. Hence, both negative and positive invoice is generated for the remaining period i.e. from 20/08/2021 to 31/12/2021.

![](<../../.gitbook/assets/Proration Apply charges\_1.png>)

In similar scenario, if future date is selected i.e. 1st September, then the invoice will be generated with the updated amount and subscriber count on the said date.

![](<../../.gitbook/assets/Proration Apply charges\_2.png>)

{% hint style="info" %}
**Note:**&#x20;

* **While adding a product in Opportunity/Quote/Order as a part of proration the product selected can either be the product(s) from the subscription line of the selected Subscription Schedule or their respective add-ons**
* **To decrease the subscriber count you should** [**revise**](https://docs.inogic.com/subscription-and-recurring-billing-management/features/revision) **your Subscription Schedule**
{% endhint %}

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

