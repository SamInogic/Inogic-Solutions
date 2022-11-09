# Subscription Lines

The Subscription Line entity is used to enter the information for the Products related to the Subscription Schedule and track the quantity and the amount to be billed. You must have at least one Subscription Line on a Subscription Schedule. The Subscription Lines will be carried over to the Invoice as the Invoice Lines.

### How to Create Subscription Lines:

* Navigate to **Subscription and Recurring Billing Management App --> Schedules --> Subscription Schedules -->** Open the **Subscription Schedule** for which you wish to add the Subscription Lines.&#x20;
* Go to **‘Subscription Lines’** tab --> Click on the button **‘New Billing Line’** to add a new line.

![](<../../../.gitbook/assets/Sub Sch\_5.png>)

* Enter details in the required information and any optional fields you wish to include.
  * **Name:** The name of the Subscription Line is auto populated and is made up from the Product concatenated with the Customer.&#x20;
  * **Subscription Schedule:** The parent Subscription Schedule associated with the Subscription Line. This field is required as a Subscription Line cannot exist without a Subscription Schedule. This is prefilled with the Subscription Schedule from where you are adding the Subscription Lines.&#x20;
  * **Product:** Product that needs to be added in the Invoice line.&#x20;
  * **Plan:** Select plan as you want the pricing to be calculated&#x20;
  * **Subscriber Count:** The quantity to bill on the Subscription Line. This is at the line level as each line could have a different quantity. If left blank, it will default to 1.&#x20;
  * **Price Per Billing Period:** Charges which are going to be billed as per the interval. E.g.: If the plan selected is on Monthly basis, then the price will be set per month.&#x20;
  * **Discount:** If you wish to add any Discount to the line that can be added here.&#x20;
  * **Extended Amount:** This field is auto-calculated.&#x20;
  * **Tax Processing:** This section is visible only if tax calculation is enabled on Configuration record. If Tax Calculation Type on the configuration record is set as Standard, and the country selected is USA then Is Taxable field is visible or else Tax Schedule field is visible. These fields determine how the tax needs to be calculated.

![](<../../../.gitbook/assets/Sub Sch\_6.png>)

![](<../../../.gitbook/assets/Sub Sch\_7.png>)

If the product has an Add-On and if you wish to add it in the Subscription Schedule you can add it by clicking on the **‘Add Add-Ons’** button either on the **Subscription Line** form **Ribbon** or on the **Subscription Line** **Subgrid** on the Subscription Schedule Form.

![](<../../../.gitbook/assets/Sub Sch\_8.png>)

![](<../../../.gitbook/assets/Sub Sch\_9.png>)
