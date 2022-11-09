# Advanced Configuration Steps

Here are the steps for Advanced Configuration:

* Go to **'Map My Relationships'** app --> **Entity Configuration** --> Click on **New**.

![](../../../.gitbook/assets/Adv\_Config\_1.png)

* Fill the following fields --> Click on **Save**.
  * **Name:** Enter user friendly name for the record. This name will be used in the value for **‘Map My Relationships Control Configuration’** field property.
  * **Entity:** Select the entity from the list of entity.&#x20;
  * **Set As Default:** Select **'Yes'** or **'No'** (depending upon which of the entity relationships user would like to further drill through).
  * **Entity Node Image:** Choose which image needs to displayed on the node of the primary entity record.&#x20;
    * **Entity Image:** The image of the entity that we see for the entity in the sitemap.&#x20;
    * **Record Image:** The image of the  record that we see on the record. If image is not present for record then Entity image will be displayed.&#x20;
    * **Image URL:** A field will be visible upon selection of this option. Enter the external or internal image URL.&#x20;
  * **Allowed Actions:** A list of activities present in the system. Select multiple activities from the list. The selected activities will be available for the user to create activities against the related record.

![](../../../.gitbook/assets/Adv\_Config\_3.png)

* Now, go to **Entity Relationships** --> Select **'New Entity Relationships'**.

![](../../../.gitbook/assets/Adv\_Config\_4.png)

![](<../../../.gitbook/assets/MMR filter\_1.png>)

*   &#x20;Fill the following fields.

    * **Relationship Type:** Choose which type of relationship you want to add. Options are ‘One-to-Many’, ‘Many-to-One’ and ‘Many-to-Many’.&#x20;
    * **Relationship:** Select the relationship from the list of relationship. This get filtered based on the option selected in the ‘Relationship Type’ field.&#x20;
    * **Relationship Node Image:** Choose which image needs to displayed on the node of the primary entity record, same as above **(Entity Image, Record Image or Image URL)**.
    * **Default View Filter:** Choose the default view for the relationship map.



![](<../../../.gitbook/assets/MMR filter\_3.1.png>)

* **Allowed Actions:** A list of activities present in the system. Select multiple activities from the list. The selected activities will be available for the user to create activities against the related record.
* **View to show fields on Tooltip:** A list of fields of the related entity selected as a Relationship. Select multiple fields. The selected fields will be displayed as a tool-tip on the nodes of the related records. On hovering over the entity record in the relationship view, all those columns that belong to the selected view are shown as a tooltip.

**Columns present under 'Active Invoices' view:**

![](<../../../.gitbook/assets/Tooltip\_2 (1).png>)

**Information shown on hovering over the respective entity record:**

![](../../../.gitbook/assets/Rel\_3.png)

* **Continuing....**
  * **Child Configuration:** A list of Entity Configurations will be available. Select one such configuration to further drill down through the relationship and see associated entity records.&#x20;
  * **Group By:** A list of optionset type of fields of the related entity selected as a relationship. Select a single field. The Map My Relationships view will group the records based on the selected field. For example, as shown below, grouping can be done on the basis of **gender:**

![Grouping based on Gender](../../../.gitbook/assets/Grouping\_1.png)

* **Continuing....**
  * **Measure and Aggregate Type:** A list of fields of the related entity. Select a field and the selected field will be displayed as a tooltip of the grouped node with aggregation. This will measure the selected field in the relationship configuration and calculate the value based on the option chosen as an aggregate type. Consider a scenario where there are total 4 contacts with the following credit limit values.&#x20;
    * Contact 1 (Female) – Rs. 1,000&#x20;
    * Contact 2 (Female) – Rs. 1,500&#x20;
    * Contact 3 (Male) – Rs. 500&#x20;
    * Contact 4 (Male) – Rs. 2,000

Let’s set the values to **'Measure'** and **'Aggregate Type'** in the relationship configuration as shown below:



![](<../../../.gitbook/assets/Mea & Agg\_3.png>)

On hovering over the group node, it will show the **sum of Credit limit**:

![](<../../../.gitbook/assets/Mea & Agg\_1 (1).png>)

![](<../../../.gitbook/assets/Mea & Agg\_2 (1).png>)

* After filling all the respective fields, click on **Save**.

![](<../../../.gitbook/assets/MMR filter\_5.png>)

![](<../../../.gitbook/assets/MMR filter\_6.png>)

* Next, perform the steps to [add Map My Relationships control on the form](https://docs.inogic.com/map-my-relationships/configuration/add-map-my-relationships-control-on-the-form) --> Go to **Controls** --> Select **Map My Relationships** control.

![](<../../../.gitbook/assets/Basic\_0 (2).png>)

* Go to **'Map My Relationships Control Configuration'** --> Enter the **'Entity Configuration'** record name.

![](../../../.gitbook/assets/Adv\_6.png)

![](../../../.gitbook/assets/Adv\_7.png)

* **Save and Publish** the customization.

![](../../../.gitbook/assets/Adv\_8.png)
