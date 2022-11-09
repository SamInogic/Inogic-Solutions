# Products

Product entity consists of the records of products which you want to sell as subscriptions. After installing Subscription and Recurring Billing Management app, two new tabs will be added to the records of existing products and newly added products – **Tax Processing & Subscription Management.**&#x20;

### **Tax Processing**

The Tax Processing tab is seen only if the value in the **Enable Tax** field on Configuration record is set to **Yes.** It gives information about the applicability of tax on the product. It has the following field:

**Is Taxable:** It is a two option set field. If it is set to **Yes** then the product is taxable. This field is visible only if the Tax Calc Country on Configuration is set to **USA.**

![](../../.gitbook/assets/Product\_1.png)

**Default Sales Tax Option:** It is a look up to the Tax Schedule. If the **Tax Calc Country** on Configuration is set to **Others** then Tax Schedule field shows up on Product form.

![](../../.gitbook/assets/Product\_2.png)

### Subscription Management

Next, we see is the Subscription Management tab which shows information about the Plans and Add-ons applicable to the Product. It has the following fields:

* **Is Add-On:** This field simply marks if the product is itself a Parent product or an add-on product which shall be associated to one or more products.&#x20;
* **Charge Type:** This field defines how to charge the product. It is either **Recurring** or **One time** charge. Based on this information charges will be added while renewing subscriptions.

![](../../.gitbook/assets/Product\_3.png)
