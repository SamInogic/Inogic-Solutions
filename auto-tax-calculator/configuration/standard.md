# Standard

When the **‘Standard’** option is selected for **‘Tax Calculation Type’** in Inogic Settings, tax is calculated depending upon the tax schedules added in the setting or on the Product, Customer or on Product lines.&#x20;

Following fields need to be filled for **Standard** type of tax calculation.

* **Tax Calculation Country:** This field is an option set with the following values
  * **USA:** If USA is selected then tax calculation is done depending upon the tax schedule set on the customer. This is the Default value.
  * **Other:** If Other is selected then tax calculation is done depending upon the tax schedule set on the product.
* If Tax Calculation Country is set to **USA** then below fields will be visible:
  * **Product Is taxable:** This is a 2 optionset field.
    * **No:** Here, tax will not be applicable on the value of products. There will be no tax calculated on the value of products.&#x20;
    * **Yes:** Here, tax will be applicable on the value of products. Tax will be calculated as per the rate defined in the **Tax Schedule** mentioned on the **Customer.**
  * **Write-In Product Is Taxable:** Here we can define whether the Write-in Product is taxable or not.

![](../../.gitbook/assets/Standard\_1.png)

* If Tax Calculation Country is set to **Other** then the below fields will be visible:
  * **Default Tax schedule for products:** This tax schedule will be set on the newly created product by default. It can be changed as per requirement.&#x20;
  * **Default Tax schedule for Write-in products:** This tax schedule will be set on the write-in products.

![](../../.gitbook/assets/Standard\_2.png)

A tab named **‘Tax Processing’** is added to the **Product, Account, Contact and on Product lines** form. If product already exists in the CRM before the installation of Auto Tax Calculator then user needs to **manually add** the **Tax Schedule** or **Is Taxable** field.\
Also for customers the Tax schedules need to be set. The fields in **‘Tax Processing’** tab for the newly generated records will be already populated on the basis of default values set in the Inogic Settings.
