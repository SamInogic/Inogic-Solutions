# Subscription Schedules

The Subscription Schedule is used to define a framework for billing a customer using a particular product. The Subscription Schedule determines when a transaction should be created, and what values should be set in it. The user can create as many Subscription Schedules as they need and customize them based on common billing attributes such as billing length, frequency, reminders, penalties, margins and tax.

### How to Create a Subscription Schedule:

* Navigate to **Subscription and Recurring Billing Management --> Schedules --> Subscription Schedule --> Click on ‘New’ button.**

![](../../../.gitbook/assets/Subcription\_2.png)

![](<../../../.gitbook/assets/Subcirpt Schedule\_1.png>)

*   Enter details in the required fields and any other necessary fields.

    * **Name:** A descriptive name of the Subscription Schedule. This can be manually entered but if left blank the name concatenates the **Ship to Customer** and the word **'Subscription Schedule'.**&#x20;
    * **Bill To Customer:** The Customer to whom the invoice is sent and is responsible for paying the invoice. This could be the Reseller, the Customer, or a third party if they are being billed directly. If you bill the Customer directly, the Bill To Customer and Ship to Customer will be the same. This will appear as the Bill To on the Sales Invoice.&#x20;
    * **Ship To Customer:** The End Customer who would be actually using the product.&#x20;
    * **Price List:** Select the price list for the product.
    * **Payment Terms Definition:** This field defines the payment terms that the customer has agreed to. Payment Terms if selected as **‘Net 30’** then the Invoice when generated from the Subscription Schedule will have the Invoice due date set 30 days after the document date.



![](<../../../.gitbook/assets/Sub Sch\_3.png>)

* Continuing.....
  * **Refund Mode:** This is the option set field with values as -
    * **No Refund:** When the subscription is cancelled no refund will be given to the customer. This is the default value of the field.&#x20;
    * **Issue Credit Memo:** When the subscription will be cancelled refund will be given to the customers on prorated basis.
  * **Margin Schedule:** This field will be populated based on ‘Bill to Customer’. If Margin schedule is defined on Bill to customer, then that will be set n subscription schedule&#x20;
  * **Margin Percentage:** This field is populated on the basis of Margin Schedule. Margin Percentage will be taken from the Margin schedule and this field is editable only by the user having the Security Role **'System Administrator'** or **'Subscription Management Admin'.**&#x20;
  * **Transaction Entity:** This field is auto populated from the Configuration entity record. Its default value is Invoice. It decides whether an Invoice or a Sales Order should be generated from the Subscription Schedule.
  * **Send Mail on Invoice Generation:** This field provides two options – **Yes / No**. If **‘Yes’** is selected, an email along with Invoice will be sent to the customer as and when Invoice is generated.&#x20;
  * **Send Email Rule:** This field appears when **‘Yes’** option is selected for the above mentioned field. Here, user can select the specific Reminder Rule created for this purpose.

![](<../../../.gitbook/assets/Sub Schedule.png>)

*   Continuing.....

    * **Start Date:** Date when the subscription will start.&#x20;
    *   **End Date**: The last of date of Subscription which is auto populated depending upon the Stt Date, Bill Every, Bill on X Date, Interval and Total Subscription Period.&#x20;

        For example -&#x20;

        * **Start Date - 3/23/2022 (M/DD/YYYY)**
        * **Bill Every – X Month(s)**&#x20;
        * **Interval – 1**&#x20;
        * **Bill on X Date - 17**
        * **Total Subscription Period - 2**&#x20;
        * **End Date – 5/16/2023 (M/DD/YYYYY)**&#x20;

        If the value of **Duration Option** is **No End Date**, then the **End Date** remains empty.
    * **Bill Every:** The frequency at which to generate invoices/orders for this Subscription Schedule. The following options are available:
      * X Day(s)&#x20;
      * X Week(s)&#x20;
      * X Months&#x20;
      * X Year(s)
    * **Interval:** This works in conjunction with the Bill Every field. It’s a numeric field where you can set the Interval as in like if we want to keep monthly billing cycle then in Bill Every, select **X Month(s)** and keep Interval as **1**.&#x20;
    * **Bill on X Date/Bill Date/Bill on X Day:** This field provides the option to select the date on which Invoice will be generated. It could be on a different date (past date) than the subscription start date. Depending on the option selected in **‘Bill Every’** section, this field will change accordingly. For example -&#x20;

    If **‘X Year(s)’** is selected then a new field named **‘Bill Date’** will appear in which user has to define the date, month and year.

![](<../../../.gitbook/assets/Sub Sch Bill every\_1.png>)

If **‘X Month(s)’** is selected then a new field named **‘Bill on X date’** will appear in which user has the option to select any date between 1 to 31.

![](<../../../.gitbook/assets/Sub Sch Bill every\_2.png>)

{% hint style="info" %}
**Note: While selecting a bill date one has to always consider the number of days available in the previous month since the billing period is accounted for from the previous month.**&#x20;

**For example - If the subscription starts on 24/03/2022 and 'Bill on X Date' is given as 25 then the billing period will be 25/02/2022 to 25/03/2022. But if 'Bill on X Date' is given as 30 then an error will be displayed stating that the date is un-representable. This is because February has only 28 days and the system cannot calculate the billing period from 30th Feb to 30th March.**
{% endhint %}

If **‘X Week(s)’** is selected then a new field named **‘Bill on X Day’** will appear in which user has to select any day of the week – Monday to Sunday.

![](<../../../.gitbook/assets/Sub Sch Bill every\_3.png>)

If **‘X Day(s)’** is selected then there will be no additional fields since the customer is going to be billed on daily basis.

![](<../../../.gitbook/assets/Sub Sch Bill every\_4.png>)

* **Initial Charge for:** This field defines the period for which the customer will be charged. There are two options:&#x20;
  * **Bill for full period:** Here, the customer will be charged for the full period irrespective of the date on which the Invoice is generated. For example – Suppose the start date for the subscription is 15th March 2022 but the billing date is 1st of March. Here the customer will be charged for the entire month i.e. from 1st March to 31st March 2022.
  * **Bill Pro-Rated:** Here, the customer will be charged on pro-rata basis. For example – Suppose the start date for the subscription is 15th March 2022 and the billing date is 1st March 2022. Here the customer will be charged from the remaining period on pro-rata basis from 15th March 2022 to 31st March 2022.Then the next invoice will be generated for full amount for next month i.e. on 1st April 2022.
* **Duration Option:** Define whether to bill indefinitely or a specified number of times.&#x20;
  * **No End Date –** Invoices/Orders will be created endlessly.&#x20;
  * **Bill Specified Number -** Allows you to bill for a specified number of invoices/orders.&#x20;
* **Total Subscription Period:** This field defines the number of Invoices which will be generated during the entire subscription cycle.
* **Generate When Option:** Determines if an Invoice/Order should generate when the Current record field is empty or a specified number of days before the Next transaction Date. The following options are available.
  * **Current Record is Empty –** If this option is selected then the Subscription Schedule will generate Invoice/Order if the field ‘Current Record’ is Empty. This field is empty before the first invoice/order is generated. Later it gets set with the recently generated Invoice or Order. Once the Invoice is paid or the Order is completed then the Current Record field becomes empty.&#x20;
  * **Number of Days before Next Transaction Date -** Looks at the current Next transaction Date and generates an invoice/order specified number of days prior to that Date. For example, if the Next Transaction Date is 03/23/2022 (MM/DD/YYYY) and the Number of Days before Next Transaction Date is set to 10 then the next Invoice/Order would be generated on 03/13/2022 (MM/DD/YYYY).
* **Generate Days Count:** This field defines the number of days before a Schedule is due to generate an Invoice/Order. For example, if you enter 10, the invoice/order will generate 10 days before it is due. This field is only available if the **'Generate When Option'** is set to **‘Number of Days before Next Transaction Date’.**
* **Remaining Invoices Count/Remaining Order Count:** The remaining number of invoices/orders to generate for this Subscription Schedule when the Duration Option is set to **'Bill Specified Number'.** This will continue to count down the number of invoices/orders left to generate until it reaches 0. After it reaches 0, no more invoices/orders will be generated.&#x20;
* **Delayed Charge Schedule:** The Delayed Charge Schedule assigned to the Invoice/Order generated from this Subscription Schedule. It is a penalty fee a customer must pay when the invoice/Orders are past due. It is an optional field and only used if Delayed Charge Schedules are used.&#x20;
* **Reminder Schedule:** The Reminder Schedule assigned to the Invoice/Order generated from this Subscription Schedule. A Reminder Schedule is an automated reminder sent to the customer regarding their bill and its due date. A different Reminder Schedule can be assigned to each Subscription Schedule. It is an optional field and only used if Reminder Schedules are used.&#x20;
* **Reminder Renewal Schedule:** A reminder schedule to renew subscriptions can be incorporated with the subscription schedule. Once the end date is nearby an automated reminder will be sent to the customers for subscription renewal and to the owner of the subscription schedule intimating about the same.
