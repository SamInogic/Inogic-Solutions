# Specify related records

To copy related opportunity line item to order line item, follow the steps given below:

* Navigate to **Child Templates** --> Click on **New Click2Clone Template.**

![](../../../.gitbook/assets/Clone2\_3.1.png)

* Fill in the following details --> Click on **Save**.

**Name** = Enter an appropriate name for the Child Template.&#x20;

**Source entity** = Opportunity Product (Since we want to copy related opportunity line item)&#x20;

**Target entity** = Order Product (Since we want to copy the related opportunity line item to order line item)&#x20;

**Source relationship** = Select **'product\_opportunities'** (This is **1:N relationship** between **Opportunity** and **Opportunity line** item)&#x20;

**Target relationships** = Select **'order\_details'** (This is **1:N relationship** between **Order** and **Order line** item)

It is **mandatory** that parent entity holds **1:N relationship** with the selected **child** entity.

![](../../../.gitbook/assets/Clone2\_3.2.png)

* Go to **Fields Mapping** section --> Map the fields of child records --> Click on **Save.**

![](../../../.gitbook/assets/Clone2\_3.4.png)

Once you have completed all the steps, you will be able to [copy one entity record to another](https://docs.inogic.com/click2clone/features/copy-one-record-to-another).
