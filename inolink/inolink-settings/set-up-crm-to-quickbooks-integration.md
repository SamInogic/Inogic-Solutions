# Set up CRM to QuickBooks integration

With the help of this section, the user can enable the required feature namely Dynamics 365 CRM's customers (Contact/Account), Product, Quote, Order, Invoices that needs to be synced with QuickBooks companies.&#x20;

As shown in below image you need to select the required Company in the Companies tab for which you want to configure the settings.

![](<../../.gitbook/assets/CRM to QB\_1 (2).png>)

### Customer - (Account/Contact)

Using this option you can enable the feature to sync the details from Dynamics 365 CRM **Accounts/Contacts** to **** QuickBooks. After clicking on **Customer** you will get the below displayed window:

![](<../../.gitbook/assets/CRM to QB\_Cust\_1.png>)

Here, you need to enable the feature by switching **ON** the button at top right corner which will then turn **** green.

#### **Name Matching Criteria:**&#x20;

You have two options here:-

* **Exact** – It will look for an exact name match.&#x20;
* **Pattern** – It will perform a pattern match to cover for any typos in data entry in the two systems. E.g. **InfoMedia** and **IfnoMedia** will be treated as the same record and updated instead of creating duplicates.

#### **Deadlock Win:**&#x20;

You have two options here i.e. **CRM** or **QuickBooks.**

If you have configured a two-way sync, use this property to define the application that will hold the last change, in case changes are made in both systems to the same record.

#### **Allow Primary contact to sync:**

Set this as '**Allow'** if you would like the **Primary Contact** field from **Dynamics 365 CRM** to be synced to **Contact** field in **QuickBooks.**

Given that Accounting Contact may be different from the Business Contact stored in Dynamics 365 CRM, you may not want to override the Primary contact set in QuickBooks from Dynamics 365 CRM and vice versa. In that case, set this option as ‘**Do not Allow**’.

After clicking on **Save** button you will get below success message**:**

![](<../../.gitbook/assets/CRM to QB\_Cust\_2.png>)

### **Product**

Using this option you **** can enable the feature to move the **Products** from Dynamics 365 CRM to QuickBooks. After clicking on **Product** you will get the below-displayed window:

**Product feature Setting For US QuickBooks Company**

![](<../../.gitbook/assets/CRM to QB\_Prod\_1.png>)

Here**,** you need to enable the feature by switching **ON** the button at top right corner which will then turn green.

#### **Name matching criteria:**

You have two options here**:-**

* **Exact** – It will look for an exact name match.&#x20;
* **Pattern** – It will perform a pattern match to cover for any typos in data entry in the two systems.

#### **Deadlock Win:**

You have two options here i.e. **CRM** or **QuickBooks.**

If you have configured a two-way sync, use this property to define the application that will hold the last change, in case changes are made in both systems to the same record.

#### **Base Price List:**

In Base Price List you need to set the required **Base Price List** to be selected while syncing the Products from Dynamics CRM to QuickBooks.

{% hint style="info" %}
**Note: While selecting the Base Price List user needs to verify if the currency of the price list to be matched with the country of QuickBooks. If user selects different price list then they will get below error message.**
{% endhint %}

![](<../../.gitbook/assets/CRM to QB\_Prod\_2.png>)

#### **Product Mappings:**

In this section, you need to select the type of **products** along with the **Account** type that is to be selected for Product sync feature.

#### **Asset Account / Income Account / Expense Account:**

All type of Product in QuickBooks – **Inventory, Non-Inventory, Service** needs to have the following accounts provided for correct handling of the accounting transactions against these products.

* **Asset Account**&#x20;
* **Income Account**&#x20;
* **Expense Account**

You can look for these accounts in **Chart of Accounts** in QuickBooks.

![](<../../.gitbook/assets/CRM to QB\_Prod\_3.png>)

When a Product is moved from Dynamics 365 CRM to QuickBooks it will set above Accounts as follows:

![](<../../.gitbook/assets/CRM to QB\_Prod\_4.jpg>)

After selecting all the values in Product Mapping feature and clicking on **Save** button you will get below success message:

![](<../../.gitbook/assets/CRM to QB\_Prod\_5.png>)

### Quote

Using this option you can enable the feature to move the **Quotes** from Dynamics 365 CRM to QuickBooks. After clicking on Quotes you will get the below displayed window.

![](<../../.gitbook/assets/CRM to QB\_Quote\_1.png>)

Here, you need to enable the feature by switching **ON** the button at top right corner which will then turn green.

![](<../../.gitbook/assets/CRM to QB\_Quote\_2.png>)

#### Auto Create Missing Customer:

Set this option to **Yes** if you would like to **automatically** create a **missing customer** in **QuickBooks** when a transaction is promoted from Dynamics 365 CRM to QuickBooks.

Set this option to **No**, if you would like to manually control the customer records being created in QuickBooks. In this case, the transaction would not be created in QuickBooks if associated customer record is not found in QuickBooks.

In case if you have **not saved the Transaction Settings** then after clicking on **Save** button you will get the below message.

![](<../../.gitbook/assets/CRM to QB\_Quote\_3.png>)

### Transaction Settings&#x20;

Then, you to first save the **Transaction Settings** by selecting the **Transaction Settings feature** option. You will get to see the following options displayed as shown below.

![](<../../.gitbook/assets/CRM to QB\_Tran\_1.png>)

QuickBooks and Dynamics 365 CRM handle some accounting concepts like **Discounts, Write-In Products,** and **Shipping Product** differently. To allow for **error-free syncing** between Dynamics 365 CRM and QuickBooks, we ask to set up the products that need to be used for specific accounting features, namely, **Write-In, Line Discount,** and **Shipping Product.**

#### Write-In Product:

Dynamics 365 **** CRM allows for adding a **write-in product** in **Quote, Order** and **Invoice.**

![](<../../.gitbook/assets/CRM to QB\_Tran\_2.png>)

**QuickBooks** however, does not allow entering a line item without specifying the product. To avoid this conflict we request a service type of product to be created in QuickBooks that we can use when transferring write-in lines from CRM Quote, Order and Invoice to QuickBooks. QuickBooks side user needs to create the write-in product in case of **US Company** they need to select **Is Taxable** option. If they want to calculate tax on write-in then they should select is taxable **true** while creating write-in product in QuickBooks.

![](<../../.gitbook/assets/CRM to QB\_Tran\_3.png>)

In case of **UK/Canada/Australia** based QuickBooks company, user needs to define the Tax code on QuickBooks side as shown below to bring the tax in Dynamics 365 CRM while syncing the product. Thus, based on tax code the CRM will calculate the tax for write-in product on Quote/Order/Invoice.

![](<../../.gitbook/assets/CRM to QB\_Tran\_4.png>)

After this, any **write-in line** from Dynamics 365 CRM would be carried over in QuickBooks as shown in the screenshots below:

![](<../../.gitbook/assets/CRM to QB\_Tran\_5.png>)

#### Line Discount product:

Dynamics 365 CRM allows you to specify discounts for line-items by specifying the discount amount in the **Discount** and **Volume Discount** fields on the line item form.

![](<../../.gitbook/assets/CRM to QB\_Tran\_6.png>)

QuickBooks on the other hand requires products to be created of the type **'Discount'** and add it as a separate line item in the transaction.

With the above mapping, line item discount in Dynamics 365 CRM as shown below;

![](<../../.gitbook/assets/CRM to QB\_Tran\_7.png>)

would be carried over to QuickBooks as shown below.

![](<../../.gitbook/assets/CRM to QB\_Tran\_8.png>)

#### Shipping product:

Dynamics 365 CRM allows for entering a **Shipping product** in **Quote** and **Invoice.**

![](<../../.gitbook/assets/CRM to QB\_Tran\_9.png>)

**Dynamics 365 CRM doesn’t calculate tax on freight amount.** Thus, we request a service type of product to be created in QuickBooks that we can use while transferring **Freight Amount** from Dynamics 365 CRM Quote/Order/Invoice to QuickBooks.

For **UK/Canada/Australia,** you need to create the **Shipping product** as a **service type** product in QuickBooks with the **Tax code** defined and tax as **zero rated.**

![](<../../.gitbook/assets/CRM to QB\_Tran\_10.png>)

After this, if you select the **Freight Amount** in Quotes/Orders/Invoice records of **Dynamics 365 CRM** it would be carried over in **QuickBooks** as a **Shipping amount.**

The product mappings accept the products of the following types in QuickBooks.

| **Dynamics 365 CRM**  | QuickBooks Item type |
| --------------------- | -------------------- |
| Line Discount Product | Service Product      |
| Write-In Product      | Service Product      |
| Shipping Product      | Service Product      |

After selecting the details in Transaction Settings and saving it you will be redirected to **Quote** feature.

#### Enable Tax Calculation:

With the help of this option you can select whether you want to automatically calculate the tax for Quote/Order/Invoice in Dynamics 365 CRM or not.

![](<../../.gitbook/assets/CRM to QB\_Tran\_11.png>)

![](<../../.gitbook/assets/CRM to QB\_Tran\_12.png>)

**Sync Tax** option allows you to sync the tax details automatically in case if there are changes made in tax within the QuickBooks systems or if your tax was not synced previously.

![](<../../.gitbook/assets/CRM to QB\_Tran\_13.png>)

![](<../../.gitbook/assets/CRM to QB\_Tran\_14.png>)

### Order

Using this option you can enable the feature to move the **Order** from Dynamics 365 CRM to QuickBooks. After clicking on Order you will get the below displayed window.

![](<../../.gitbook/assets/CRM to QB\_Order\_1.png>)

Here**,** you need to enable the feature by switching **ON** the button at top right corner which will then turn green.

![](<../../.gitbook/assets/CRM to QB\_Order\_2.png>)

#### Auto Create Missing Customer:

Set this option to **Yes** if you would like to automatically create **a missing customer** in **QuickBooks** when a transaction is promoted from Dynamics 365 CRM to QuickBooks.

Set this option to **No**, if you would like to manually control the customer records being created in QuickBooks. In this case, the transaction would not be created in QuickBooks if associated customer record is not found in QuickBooks.

After clicking on **Save** button you will get below success message.

![](<../../.gitbook/assets/CRM to QB\_Order\_3.png>)

### Invoice

Using this option you can enable the feature to move the **Invoice** from Dynamics 365 CRM to QuickBooks. After clicking on Invoice you will get the below displayed window.

![](<../../.gitbook/assets/CRM to QB\_Inv\_1.png>)

Here, you need to enable the feature by switching **ON** the button at top right corner which will then turn into a green button.

![](<../../.gitbook/assets/CRM to QB\_Inv\_2.png>)

#### Auto Create Missing Customer:

Set this option to **Yes** if you would like to automatically create **a missing customer** in **QuickBooks** when a transaction is promoted from Dynamics 365 CRM to QuickBooks.

Set this option to **No**, if you would like to manually control the customer records being created in QuickBooks. In this case, the transaction would not be created in QuickBooks if associated customer record is not found in QuickBooks.

After clicking on **Save** button you will get below success message.

![](<../../.gitbook/assets/CRM to QB\_Inv\_3.png>)



