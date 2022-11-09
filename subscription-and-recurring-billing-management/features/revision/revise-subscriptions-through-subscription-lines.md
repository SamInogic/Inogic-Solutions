# Revise Subscriptions through Subscription Lines

Let's consider a scenario to better understand how subscription schedules can be revised through subscription lines.

Suppose a customer has subscribed for the product at the starting of the month. Now midway through the month they want to increase the user count for the product. Since the invoice has been already generated for this subscription, the fields in Subscription Line are locked. So, the first step is to unlock these fields.&#x20;

To revise the fields in Subscription Line, follow the steps given below:

* Go to **Subscription Schedule --> Select and open the Subscription Line.**

![](../../../.gitbook/assets/Revision\_1.png)

* Now click on the **‘Revise’** button on the ribbon bar.

![](../../../.gitbook/assets/Revision\_2.png)

* After clicking on the ‘Revise’ button, all the fields will become unlocked.&#x20;
* Next, make the necessary revision to the fields. Here, we have increased the **Subscriber Count** from **10 to 20** and selected **Apply Charges** as **Immediately (Prorated).**

![](../../../.gitbook/assets/Revision\_3.png)

* On **Apply Charges,** we can select either of the **four** options. Based on this the Invoice will be generated.
  * **Immediately:** The new invoice will be generated instantly with new charges applicable including the current billing cycle.&#x20;
  * **Immediately (Prorated):** The new invoice will be generated instantly and the new charges will be calculated for the remaining days of the current billing cycle.&#x20;
  * **Start from Next Billing Cycle:** The new charges will be applicable from the next billing cycle.
  * **Custom:** The new charges will be applicable from the date set in 'Billing Start Date' and the new invoice will be generated accordingly. For example, let’s consider a scenario where the annual subscription for one of the products is set for Jan 2021 to Dec 2021. Now, the customer increased the subscriber count from **10 to 20** from mid of August, i.e. **15/08/2021**. Due to company policy, it was decided to create a back-dated invoice from 1st Aug 2021 with new subscriber count. So, for this select **‘Custom’** option and set **‘Billing Start Date’** field **** to 01/08/2021. Instantly, a negative and positive invoice for the period 01/08/2012 to 31/12/2021 will be generated. Here, negative invoice indicates the amount which needs to be refunded to the customer. On the other hand, positive invoice indicates the amount to be charged to the customer for the increased subscriber count. Similarly, if the customer wants the charges to be applied from 1st September then you can revise the schedule accordingly. Just select **‘Custom’** and set **‘Billing Start Date’** to 01/09/2021. Since this is a future date, both negative and positive invoice for the remaining period i.e. from 01/09/2021 to 31/12/2021 will be generated on 1st Sept 2021.&#x20;

![](<../../../.gitbook/assets/Apply Charges\_3 (2).png>)

![](<../../../.gitbook/assets/Apply Charges\_2.png>)

* Coming back to our current example, since we have selected **‘Immediately (Prorated)’,** a new invoice is generated which can be seen in the Invoices section. And to initiate the refund a negative invoice is created as well.

![](../../../.gitbook/assets/Revision\_5.png)

{% hint style="info" %}
**Note: On your existing Subscription Schedule you cannot add a new product. For this you will have to create a new Subscription Schedule itself.**
{% endhint %}
