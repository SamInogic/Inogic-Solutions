# Billing - Invoices/Orders

Subscription and Recurring Billing Management utilizes the Dynamics 365 Invoices/Sales Order entity to create Invoices/Orders from Subscription Schedules.&#x20;

The generation of Invoice/Order can either be automated by creating the record of [Workflow Trigger ](https://docs.inogic.com/subscription-and-recurring-billing-management/features/workflow-triggers)or we can go by the ad-hoc way by running the on-demand workflow named **'SM - Generate Document from Subscription Schedule'** on the Subscription Schedule record.

### How to generate invoices/orders on demand from Subscription Schedules:

* Navigate to **Subscription and Recurring Billing Management App --> Schedules --> Subscription Schedules --> Select a schedule.**
* Go to **Ribbon** bar --> Click on **Flow.**

![](../.gitbook/assets/Billing\_1.png)

* Click on **‘SM-Generate Document from Subscription Schedule’** workflow.

![](../.gitbook/assets/Billing\_2.png)

* A dialog box will appear --> Click on **OK.**

![](../.gitbook/assets/Billing\_3.png)

* The workflow is now triggered and the **Invoice or Sales Order** will be generated shortly.

On Invoice/Order form, you will also find some **additional fields** are added in the summary section as shown below:

![](../.gitbook/assets/Billing\_4.png)

**Document Date:** Date when the record is created.&#x20;

**Payment Terms:** Terms for making payment.&#x20;

**Due Date:** Date on which payment is due.&#x20;

**Paid Amount:** The amount that has been paid on the invoice.&#x20;

**Remaining Amount:** The amount remaining to be applied to this invoice. This amount is updated whenever the payment is made. The payment is done by creating the payment records associated to the Invoice. The payment record can be created manually. While doing so you can even select the appropriate mode of payment.

There are four modes of Payment. Select the one suitable depending on the mode using which your customer made the payment.

* Cash&#x20;
* Credit Card&#x20;
* Cheque&#x20;
* Others

![](../.gitbook/assets/Billing\_5.png)

Let’s make partial payment of the Invoice. So, we create a payment record of $9.00 with the Payment Mode as Cash. As can be seen on the below screenshot the Remaining Amount now shows $10.00.

![](../.gitbook/assets/Billing\_6.png)

Now if we go ahead and click the **Invoice Paid** button on the ribbon then another payment record will get created with the remaining amount as paid and the payment mode would be **'Others'**. And the value in the field Remaining Amount will be $0.00.

![](../.gitbook/assets/Billing\_7.png)

![](../.gitbook/assets/Billing\_8.png)

The Invoice/Order consists of a Subscription Management tab which holds the below details.

![](../.gitbook/assets/Billing\_9.png)

* **Start Date:** The Invoice/Order is valid from this date.&#x20;
* **End Date:** The Invoice/Order is valid to this date.&#x20;
* **Next Billing Date:** The date when the next Invoice/Order shall be generated.&#x20;
* **Subscription Schedule:** Subscription Schedule from which the Invoice/Order was generated.
* **Reminder Schedule:** Reminder schedule according to which the email reminders will be sent.&#x20;
* **Delayed charge Schedule:** Schedule according to which the delayed charges will be implemented.
* **Delayed charge thru date:** Date after which the delayed charges will be implemented.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

