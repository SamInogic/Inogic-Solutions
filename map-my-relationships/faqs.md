# FAQs

## 1) Can we show connections in Map My Relationships control?

Yes, we can show connections in Map My Relationship control. You would need to configure the control by adding a appropriate 1:N relationship name.

## 2) Is it possible to show N:N related entity records in the Map My Relationships control?

Yes, it is possible. We can show 1:N, N:1 and N:N related records in the Map My Relationships control.

## 3) After importing the solution of Map My Relationships from  website all the Processes of Map My Relationships is in a 'Draft/Deactivated' state. What to do?

Once the solution is imported, please follow the below steps to activate all the processes of Map My Relationships.

* Click on the **gear icon** --> Select **Advanced Settings**.&#x20;

![](../.gitbook/assets/A4D\_1.png)

* Next, select **Processes**.

![](../.gitbook/assets/A4D\_2.png)

* From **'All Process'** View activate the process shown in the below screenshot:

![](../.gitbook/assets/MMR\_1.png)

## 4) Can I use Map My Relationships if I have only Power Apps environment and no Dynamics 365 CRM?

Map My Relationships works on dataverse and customer engagement environments. In PowerApps, it will only work for Model Driven Apps where we have entities. Also, Map My Relationships can be installed on an environment that does not have Dynamics 365 CRM subscription i.e. CDS environment.

## 5) We have done a sandbox copy of the production environment to a TEST environment and would like to work with 'Map My Relationships' solution in this new instance. What should we do?

For this, you need to delete the **Inogic License Details** record from your sandbox environment. After deleting, the next step would be to [activate the license](https://docs.inogic.com/map-my-relationships/getting-started/license-activation).

To delete the **Map My Relationships** license follow the steps given below:

* Navigate to **Advanced Find.**

![](<../.gitbook/assets/FAQ\_1 (2).png>)

* Select **Inogic License Details** in **‘Look for’** --> Click on **Results** button.

![](<../.gitbook/assets/FAQ\_2 (3).png>)

* Select the **Map My Relationships** record and **delete** it.

![](../.gitbook/assets/FAQ\_1.png)

## 6) Can we customize the record details that we can see by hovering over the record node in the view?

Yes, we can customize the tooltip details which will be shown based on the view selected in the entity configuration for relationships map. It takes the first five columns from the selected view.

![](<../.gitbook/assets/MMR FAQ\_6.png>)
