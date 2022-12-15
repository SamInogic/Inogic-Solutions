# Add Map My Connections control on the form

Map My Connections control allows user to configure the connection control for a particular entity for which the user wishes to create, update and delete the connection record(s).

### Parameters of Map My Connections control

1. **Allowed Role Categories:** Allows user to state the role categories for which the user want to create a connection record. For example, Sales Team, Business, Family, etc.&#x20;
2. **Allowed Entities:** Allows user to put the entities of user’s choice to create a connection record of a chosen entity.&#x20;
3. **Default Control:** Allows user to decide the default view of the connection control.&#x20;
4. **Map My Relationships Control Configuration:** Allows user to enter a name of the Map My Relationships entity configuration in order to be able to see and create a connection record through relationship view.&#x20;
5. **Allow to connect using Relationships map:** Allows user to be able to create a connection record by searching a record through the relationship view.

### Components of Map My Connection control

1. **Grid/Relationships View:** To allow user to see the data in grid as well as in relationship view.
2. **Expand relationship view:** To view the connection control in enlarged screen mode.
3. **Grid Refresh:** To refresh the connection control
4.  **New connection creation:** These are the necessary fields to successfully create new connection - &#x20;

    a) **Role:** All those roles that fall under the selected role category will be listed under this drop-down.

    b) **Select Entity:** The entities that user puts in while binding the connection control will be listed here.

    c) **Selection Type:** This allows user to search a record either through a look up field or through relationship view.

    d) **Selected Record:** Allows user to select a record for creating a connection.

    e) **Description:** User can add any description for the connection record.
5. **Update connection:** Allows user to update the connection with any of the above fields
6. **Delete connection:** Allows user to delete the connection record easily

### Steps to configure the connection control

Consider a scenario where user wants to connect a few records to the Opportunity entity record.

For this, first we will start with configuring the connection control for the **Opportunity** entity.

1\) Go to **Advanced Settings --> Settings --> Customizations --> Customize the System.**

![](../../.gitbook/assets/MMC\_1.png)

![](../../.gitbook/assets/MMC\_2.png)

![](../../.gitbook/assets/MMC\_3.png)

2\) **** Next, under **‘Default Solution’** select **Opportunity --> Forms --> Main Form**.

![](../../.gitbook/assets/MMC\_4.png)

3\) Now add a sub-grid on the form (You can add a sub-grid with one column for a better view).

![](../../.gitbook/assets/MMC\_5.png)

4\) Set the properties of sub-grid as shown below:

![](../../.gitbook/assets/MMC\_6.png)

5\) Now go to **‘Controls’** and add **‘Map My Connections’** control.

![](../../.gitbook/assets/MMC\_7.png)

![](../../.gitbook/assets/MMC\_8.png)

6\) Enable the control so that you can see it on all three: **Web, Phone and Tablet.**

![](../../.gitbook/assets/MMC\_9.png)

7\) Next, let’s set the parameters for the control.

**Allowed Role Categories:** Here, you will have to manually enter the role categories for which you want to create a connection of. For example, if you put **‘Sales Team’**, it will show you **‘Sales Team’** category under **‘Connect’** option with its further connection roles later on when you are creating a connection for an opportunity through connection control.

{% hint style="info" %}
**Note: These are the categories that you could find through the connection roles in business management.**
{% endhint %}

![](../../.gitbook/assets/MMC\_10.png)

You can further sort it by category.

![](../../.gitbook/assets/MMC\_11.png)

In this instance, we will put the categories as - **Sales Team,Business,Family** (**do not** add any space in between the commas **“,”** as the configuration is likely to crash because of that).

![](../../.gitbook/assets/MMC\_12.png)

![](../../.gitbook/assets/MMC\_13.png)

**Allowed Entities:** The entities that you put here will list out under **‘Select Entity’** on the **‘Create Connection’** form while adding a connection to the opportunity. This will allow user to connect the record of only these mentioned entities to the opportunity. You will need to make sure to enter the logical name of an entity into the field.

You can see the logical name of an entity here -

![](../../.gitbook/assets/MMC\_14.png)

Here, we will enter **‘account’** entity.

![](../../.gitbook/assets/MMC\_15.png)

![](../../.gitbook/assets/MMC\_16.png)

**Default Control:** You will need to set this field as either 0 or 1.&#x20;

**0** = Default view would be **‘Grid’** view.&#x20;

**1** = Default view would be **‘Relationship’** view.&#x20;

Here, we will set this as **0.**

![](../../.gitbook/assets/MMC\_17.png)

![](../../.gitbook/assets/MMC\_18.png)

**Map My Relationship Control Configuration:** It is mandatory for user to enter the name of Map My Relationship configuration if the user wishes to see the connections in the **relationship view** through the connection control. So, despite having the Map My Relationship configuration in the system, it will show you the below error if you try to see the relationship view of connections **without** entering a name of Map My Relationship configuration.

![](../../.gitbook/assets/MMC\_19.png)

Considering that the below Map My Relationship configuration is present in the system, let’s enter its name while configuring the connection control.

**Entity configuration:–**

![](../../.gitbook/assets/MMC\_20.png)

**Relationship configuration:–**

![](../../.gitbook/assets/MMC\_21.png)

Let’s enter the name of entity configuration into **‘Map My Relationship Control Configuration’** field.

![](../../.gitbook/assets/MMC\_22.png)

![](../../.gitbook/assets/MMC\_23.png)

**Allow to connect using Relationships Map:** This parameter decides whether user can search for a record through the relationships view for adding a connection. You will have to set either 0 or 1 to this field.&#x20;

**0** = **‘Relationship View’** option would be available under **‘Selection Type’** (User would be able to pick a record through relationship view).&#x20;

**1** = **‘Relationship View’** option will **not be** available under **‘Selection Type’** (User won’t be able to search for a record through the relationship view).&#x20;

Considering, we have the Map My Relationship configuration as shown below:

**Entity configuration:-**

![](../../.gitbook/assets/MMC\_24.png)

**Few more relationships:-**

![](../../.gitbook/assets/MMC\_25.png)

**Further few relationships:-**

![](../../.gitbook/assets/MMC\_26.png)

Let’s set the value as **‘0’** for **‘Allow to connect using Relationships Map’.**

![](../../.gitbook/assets/MMC\_27.png)

![](../../.gitbook/assets/MMC\_28.png)

8\) Once done with setting up all the required parameters for the connection control, let’s **save and publish** these customizations.

![](../../.gitbook/assets/MMC\_29.png)

![](../../.gitbook/assets/MMC\_30.png)

![](../../.gitbook/assets/MMC\_31.png)

9\) Now, go back to **Opportunity** record.

![](../../.gitbook/assets/MMC\_32.png)

Let’s say this opportunity has some connection records already.

![](../../.gitbook/assets/MMC\_33.png)

10\) Now navigate to the connection control which we configured earlier above through the customizations. The connection records will show in the grid.

![](../../.gitbook/assets/MMC\_34.png)

11\) You can also switch this to relationship view.

![](../../.gitbook/assets/MMC\_35.png)

12\) It will show you the connection records in relationship view format. Switching it back to grid view will show you these connection records in grid format, this is how user can change between these two views. Here, you are seeing the records are individually categorized in **‘Account’** and **‘Contact’**, this is because we have grouped it by **‘Type (To)’** under cluster settings in the entity configuration.

![](../../.gitbook/assets/MMC\_36.png)

![](../../.gitbook/assets/MMC\_37.png)

{% hint style="info" %}
**Note: Grouping can be based on both Optionset and Lookup fields in Connections control.**
{% endhint %}

![](../../.gitbook/assets/MMC\_38.png)

13\) Click on **‘Full View’** button on the right top corner of the control to see the data in expanded screen.

![](../../.gitbook/assets/MMC\_39.png)

**Expanded mode:-**

![](../../.gitbook/assets/MMC\_40.png)

User can also refresh the control if required.

![](../../.gitbook/assets/MMC\_41.png)

Now let’s create a **new connection record** for **this opportunity.** It will display those categories which we configured earlier while binding the connection control.

![](../../.gitbook/assets/MMC\_42.png)

![](../../.gitbook/assets/MMC\_43.png)

1\) Let’s pick **‘Sales Team’** for now. It will list out all the connection roles that fall under this role category.

![](../../.gitbook/assets/MMC\_44.png)

2\) Select **‘Sales Professional’**. This will open a quick create form where **‘Role’** would come selected as by default since we have chosen **‘Sales Professional**’ earlier.

![](../../.gitbook/assets/MMC\_45.png)

3\) You can also change the connection role from here if required.

![](../../.gitbook/assets/MMC\_46.png)

4\) Let’s keep **‘Sales Professional’** for now and select the entity. All those entities that are entered in the connection control configuration will be listed here. We currently have only **‘account’**.

![](../../.gitbook/assets/MMC\_47.png)

![](../../.gitbook/assets/MMC\_48.png)

5\) As we have set **‘0’** for **‘Allow to connect using Relationships Map’**, user will be shown both **‘Lookup**’ and **‘Relationships View’** options under **‘Selection Type’**. Setting the value as **‘1’** will show only **‘Lookup’** option in here.

![](../../.gitbook/assets/MMC\_49.png)

![](../../.gitbook/assets/MMC\_50.png)

6\) We have selected **‘Lookup’** here as we want to search for a record through lookup field. Click on **‘Select a record’.**

![](../../.gitbook/assets/MMC\_51.png)

7\) Search for a record that you want to make a connection with and click on **‘Add’.**

![](../../.gitbook/assets/MMC\_52.png)

8\) This will set the record to the field.

![](../../.gitbook/assets/MMC\_53.png)

9\) You can add description if required.

![](../../.gitbook/assets/MMC\_54.png)

10\) Click on **‘Save and Close’.**

![](../../.gitbook/assets/MMC\_55.png)

11\) You will see the below success pop-up once the connection is added.

![](../../.gitbook/assets/MMC\_56.png)

12\) Click **‘OK’** and the newly added connection will start showing up in both grid and the relationship view.

![](../../.gitbook/assets/MMC\_57.png)

![](../../.gitbook/assets/MMC\_58.png)

#### How to add a connection using relationship view?

![](../../.gitbook/assets/MMC\_59.png)

a) Select a quote record through the relationship view.

![](../../.gitbook/assets/MMC\_60.png)

b) Proceed to **‘Save and Close’.**

![](../../.gitbook/assets/MMC\_61.png)

c) Check for the newly created connection, it will appear in the grid.

![](../../.gitbook/assets/MMC\_63.png)

d) As well as in the relationship view of connections:

![](../../.gitbook/assets/MMC\_64.png)

13\) This is not where it ends, user is also given a provision to update the connection record. Click on the **connection record** that you would like to **update**.

![](../../.gitbook/assets/MMC\_65.png)

14\) Here, we will update the description (user can update any of the fields based on the requirement). Click on **‘Save and Close’**.

![](../../.gitbook/assets/MMC\_66.png)

15\) You will see the below message pop-up. Click **‘OK’**.

![](../../.gitbook/assets/MMC\_67.png)

16\) Updates will reflect into the record.

![](../../.gitbook/assets/MMC\_68.png)

17\) Along with create and update, user can also **delete** the connection record.

**Deleting from larger connection control:**

![](../../.gitbook/assets/MMC\_69.png)

**Deleting from smaller card view:**

![](../../.gitbook/assets/MMC\_70.png)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}







