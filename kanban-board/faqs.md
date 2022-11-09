# FAQs

## 1) Does it support custom entity?

Yes, it supports OOB as well as custom entities.

## 2) Does it work on tablet and mobile phones(iOS and Android)?

It works on tablets and mobile of both iOS and Android OS.

## 3) Does it work on On-Premise?

No, Kanban Board works only on Online environment.

## 4) How to use BPF in Kanban Board?

BPF is by default enabled on Kanban Board. To select a BPF you can choose it from the drop down on the Kanban Board.

![](<../.gitbook/assets/BPF FAQ5.png>)

## 5) Can I create custom activity against a record?

Yes, by adding the logical name of that entity in Activity Section while configuring the Kanban Board.

## 6) Kanban Board is not visible to a user?

User should have a security role of **'System Administrator'** or any of the **two roles** highlighted below to see Kanban Board.

![](../.gitbook/assets/FAQ5\_1.png)

## 7) We have done a sandbox copy of the production environment to a TEST environment and would like to work with 'Kanban Board' solution in this new instance. What should we do?

For this, you need to delete the **Inogic License Details** record from your sandbox environment. After deleting, the next step would be to [activate the license](https://docs.inogic.com/kanban-board/getting-started/license-activation).

To delete the **Kanban Board** license follow the steps given below:

* Navigate to **Advanced Find.**

![](<../.gitbook/assets/FAQ\_1 (2).png>)

* Select **Inogic License Details** in **‘Look for’** --> Click on **Results** button.

![](<../.gitbook/assets/FAQ\_2 (2).png>)

* Select the **Kanban Board** record and **delete** it.

![](<../.gitbook/assets/FAQ\_3 (1).png>)

## 8) After importing the solution of Kanban Board from website all the Processes of Kanban Board is in a 'Draft/Deactivated' state. What to do?

Once the solution is imported, please follow the below steps to activate all the processes of Kanban Board.

* Click on the **gear icon** --> Select **Advanced Settings**.&#x20;

![](../.gitbook/assets/A4D\_1.png)

* Next, select **Processes**.

![](../.gitbook/assets/A4D\_2.png)

* From **'All Process'** View activate the process shown in the below screenshot:

![](<../.gitbook/assets/Kanban FAQ\_7.png>)

## 9) Can I use Kanban Board if I have only Power Apps environment and no Dynamics 365 CRM?

Kanban Board works on Dataverse and Customer Engagement environments. In Power Apps, it will only work for Model Driven Apps where we have Entity Views. Also, Kanban Board can be installed on an environment that does not have Dynamics 365 CRM subscription i.e. Dataverse (CDS) environment.

## **10) Which type of fields can be used in Lane and Row filter criteria?**

You can use the following types of fields in Lane and Row Filter Criteria:

* Currency&#x20;
* FP (Floating Point)&#x20;
* Decimal&#x20;
* SingleLine.Email&#x20;
* SingleLine.Phone&#x20;
* SingleLine.Text&#x20;
* SingleLine.Ticker&#x20;
* SingleLine.URL&#x20;
* OptionSet&#x20;
* TwoOptions&#x20;
* Whole.None&#x20;
* Lookup.Simple
* Lookup.Owner

## 11) The title of the card is not fully visible in Kanban View. Is there a way to view the full length of the card title?

Yes, there is a way to view the full length of the card title. While [configuring](https://docs.inogic.com/kanban-board/configuration/configuration-for-entity) Kanban View for an entity, you can add the field name in **Body Text 3** as highlighted in the below image. The length of the **Body Text 3** is maximized, hence you can view the whole text.

![](../.gitbook/assets/FAQ\_10.jpg)
