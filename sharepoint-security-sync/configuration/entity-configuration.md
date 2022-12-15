# Entity Configuration

Given below are the steps for Entity configuration in SharePoint Security Sync.

For **‘Entity Configuration’** go to **SharePoint Security Sync --> Entity Configuration**.

![](<../../.gitbook/assets/Entity\_1 (2).png>)

Entity Configurations can be created from the Connector form too, just click on **Entity Configuration** **Tab** on Connector page and click on '**+ New** ' button.

![](<../../.gitbook/assets/Create Cust Fold\_0.png>)

![](<../../.gitbook/assets/Create Cust Fold\_1.png>)

### General:

* In the **General** tab, populate the following fields:
  * **Connector:** Select the Connector for which you want to configure the Entity.
  * **Entity Name:** Mention the Entity for which you are configuring.
  * **Attachment Action:** You can either Copy or Move the attachment.
    * **Copy:** If you select **Copy**, the attachment will be copied to SharePoint and its cloud storage path will be stored against the record.
    * **Move:** If you select **Move**, the attachment will be moved/migrated to SharePoint and its cloud storage path will be stored against the record.
    * **None Selected:** If you don’t select any option then the Attachment will not be moved to your Cloud Storage but you will be still able to use the Attach2Dynamcs document management UI for the respective entity.
  * **Override files:** If checked, means trying to upload file with same name will be overridden. If unchecked, then a new file with number appended is created and uploaded in SharePoint.
  * **Auto Create Folder:** By default **‘No’** is selected for this field. If **‘Yes’** is selected then folder will be created in SharePoint for the respective entity automatically.

### Create Custom Folder Structure:

SharePoint Security Sync gives provision to create your own folder structure within SharePoint for storing documents/attachments. With this tab, you can customize both the library structure as well as the record folder structure in SharePoint site. This tab is divided into two sections – **Create Library Structure** and **Create Record Folder Structure**.

The **‘Create Library Structure’** section can be set as follows:

**Library Structure:** This is an optionset field with following options – **By Period, By Starting Character** and **Custom.** Select either one of these options. Based on the option selected, further fields will be made available.

*   **By Period:** If this option is selected then the document library structure will be created based on certain period. To be precise, the period is based on ‘createdon’ date of record. In order to define the period additional fields are required to be populated. These fields include:

    * **Period Type:** This is yet another optionset field with the following options - **Daily, Weekly, Monthly, Quarterly, Yearly, X Month and X Year.**&#x20;
    * **Duration:** This is a numerical field. It appears when **‘X Month’** or **‘X Year’** option is selected in **‘Period Type’**.&#x20;
    * **Select Date Format:** This is also optionset field with numerous options. Select any one format for the date.

    For example, suppose if user has set **‘Period type’** to **‘X Month’** and **‘Duration’** to **‘6’.** Now based on this setting a half yearly document library will be created in SharePoint for whichever record created for that particular period.

![](<../../.gitbook/assets/Create Cust Fold Feat\_10.png>)

![](<../../.gitbook/assets/Create Cust Fold Feat\_11.png>)

* **By Starting Character:** If this option is selected then the document library structure will be created based on the starting character of the chosen field name. Once this option is selected, the following additional field needs to be populated:
  * **Document Library Format:** Here, logical name of the field is to be entered within brace brackets **{}**. And the field type should be either **Single.Text, Optionset** or **Lookup**.

![](<../../.gitbook/assets/Create Cust Fold\_3 (1).png>)

* **Custom:** With this option, you can create document library structure based on the full name of any chosen field. Once this option is selected, the following additional field needs to be populated:
  * **Document Library Format:** Here, logical name of the field is to be entered within brace brackets **{}**. And the field type should be either **Single.Text, Optionset** or **Lookup.**

![](<../../.gitbook/assets/Create Cust Fold\_.png>)

The **‘Create Record Folder Structure’** section can be set as follows:

**Folder Format:** Here, you can either use logical name or any text to name the folder. Further, you can also use combination of both logical name and text.

For example, suppose if user has used combination of logical and text for **‘Folder Format’** like **‘{name} KP.’** Now based on this setting the following record folder structure will be created in SharePoint.

![](<../../.gitbook/assets/Create Cust Fold Feat\_12.png>)

![](<../../.gitbook/assets/Create Cust Fold Feat\_13.png>)

### Email Configuration:

Next is the **Email Configuration** tab from which you can send the documents as attachments/links through email to the required recipients.&#x20;

![](<../../.gitbook/assets/Create Cust Fold\_5.png>)

* **From** – The sender i.e. the person who sends the email.
* **To** – Recipient i.e. the person to whom the email is to be sent.
* **CC** – Carbon Copy i.e. the person to whom a copy of the email information is to be sent.
* **BCC** – Blind Carbon Copy i.e. the person you have kept in the loop and do not want the other recipients to see that particular contact.
* Types of Email addresses to select from:
  * **Users** – If you select Users then all the CRM users present in the environment will be enlisted while selecting the data.
  * **Queue** – If you select Queue then all the queues present in the environment will be enlisted while selecting the data.
  * **Team** – If you select Team then all the teams created in the environment will be enlisted while selecting the data.
  * **Dynamics** – E.g. If you have selected quote as an entity then all the lookup fields on quote which are allowed to send email will be enlisted while selecting the data.
  * **Manager** – E.g. If you have selected quote as an entity then, all the system-user lookup fields on quote entity will be enlisted while selecting the data, and recipient would be the manager of the selected data.

{% hint style="info" %}
**Note:**

1. **To use SharePoint Security Sync functionalities on an Entity it is mandatory that you create an Entity Configuration record for the same.**
2. **Attachment Actions can be enabled only for one entity with one Connector.**
3. **Connector and Entity Configuration are editable if user has SharePoint Security Sync Administrator role.**
4. **SharePoint Security Sync User can only read the Connector and Entity Configuration.**
5. **The security level privileges will start syncing once after creating entity configuration the user hits the File tab or Attach2Dynamics button.**
{% endhint %}

### Configuring Hierarchy Structure

Attachments/Documents of Dynamics 365 CRM records can be stored in SharePoint sites on the basis of hierarchy.

To achieve this, follow the steps given below:

* Go to **Advanced Settings** --> **Settings** --> **Document Management Settings**.

![](../../.gitbook/assets/Hier\_1.png)

* Select **Entities** --> Enter the **URL** of respective SharePoint site.

![](../../.gitbook/assets/Hier\_2.png)

* Enable the Checkbox **‘Based on Entity’** --> Select either of the entities - **Account or Contact**.

![](../../.gitbook/assets/Hier\_3.png)

* Next, go to **Entity Configurations** --> Click on **New**.

![](../../.gitbook/assets/Hier\_4.png)

* Populate the fields --> Click on **Save**.
  * **Connector:** Select the connector for the particular SharePoint site.
  * **Entity Name:** Select the entity.
  * **Attachment Action:** Select either move or copy.
  * **Override Files:** Enable the checkbox if required.
  * **Folder Structure Fields:** This field appears on selection of the entity for which hierarchy structure is configured. In this field, customized entity with Account or Contact lookups will be populated. Select either of the entities.

![](../../.gitbook/assets/Hier\_5.png)

* Now go to **Opportunity** --> Select an **opportunity** --> Click on **Attach2Dynamics** button --> **Drag and Drop** required file.

![](<../../.gitbook/assets/Entity Configuration 1.png>)

* Next, go to SharePoint site. Here, the respective file will be stored in the following manner - **Account > Account Name\_guid > Opportunity > Opportunity Name\_guid.**

![](<../../.gitbook/assets/Entity Configuration 2.png>)

### Activity Entity Configuration

To create entity configuration for Activity Entities, follow the steps given below:

* Navigate to **SharePoint Security Sync** **App --> Entity Configurations**.

![](<../../.gitbook/assets/Activity Entity Config\_1.jpg>)

* Click on **+New.**

![](<../../.gitbook/assets/Activity Entity Config\_2.jpg>)

* Enter the required details to create Entity Configuration for **Email** --> Click on **Save.**

![](<../../.gitbook/assets/Activity Entity Config\_3.jpg>)

* For example - If an Account record is set as a Regarding for an Email record then create an entity configuration for the **Account** entity as shown in the below screenshot. Make sure to select either **Copy or Move** as **** an **** attachment action while configuring the entity record.

![](<../../.gitbook/assets/Activity Entity Config\_4.jpg>)

* Once the Email is **Sent or Received**, the attachments will get migrated to SharePoint and the email attachment would be uploaded inside an email folder present in the regarding record folder as shown in the below screenshot:

![](<../../.gitbook/assets/Activity Entity Config\_5.jpg>)

* Similarly, if there are any other entity records as an email regarding then create an Entity configuration for those entities as well.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}

&#x20;
