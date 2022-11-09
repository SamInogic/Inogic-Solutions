# Entity Configuration

{% embed url="https://youtu.be/qKKUo1khbDY" %}

Entity configuration enables users to manage and store documents/attachments related to entity records in all three cloud storage with the help of Attach2Dynamics button.

Here are the steps to configure Entities for three different connectors.

### **SharePoint Connector:**

* Navigate to **Attach2Dynamics app --> Entity Configuration --> Click on New.**&#x20;

![](<../../.gitbook/assets/Hier - Copy.png>)

* Fill the following fields in **'General'** tab --> Click on **Save**.
  * **Connector:** Select the Connector.
  * **Entity Name:** Select the entity i.e. Account, Quote, Email, Sales Literature, etc.
  * **Attachment Action:** Select either move or copy.
    * **Copy:** If you Select Copy, the attachment will be also be copied to Cloud Storage and its cloud storage path will be copied in Dynamics CRM next to attachment’s location.&#x20;
    * **Move:** If you Select Move, the attachment will be moved/migrated to Cloud Storage and its cloud storage path will be left behind in Dynamics CRM next to attachment’s location.
    * **None Selected:** If you don’t select any option then the Attachment will not be moved to your Cloud Storage but you will be still able to use the Attach2Dynamcs document management UI for the respective entity.
  * **Override Files:** Enable the checkbox if required.
  * **Folder Structure Field:** This field appears on selection of the entity for which hierarchy structure is configured. In this field, customized entity with Account or Contact lookups will be populated. Select either of the entities.
    * **Configuring Hierarchy Structure:** Another interesting factor in Folder Structure is that Attachments/Documents of Dynamics 365 CRM records can be stored in SharePoint sites on the [basis of hierarchy](https://docs.inogic.com/attach2dynamics/how-to-guides/configuring-hierarchy-structure).

Lastly, got to **'Email Configuration'** **--> Populate the fields --> Click on Save.**

![](../../.gitbook/assets/Entity\_3.png.jpg)

#### Example:

Go to any Opportunity record -->Click on the **'Attach2Dynamics'** button.

![](<../../.gitbook/assets/Entity config example\_1.png>)

The Attach2Dynamics UI will open --> Upload file(s) --> Click on **'Open Folder'** button.

![](<../../.gitbook/assets/Entity config example\_2.png>)

You will be now directed to the SharePoint site where the file(s) is stored.

![](<../../.gitbook/assets/Entity config example\_3.png>)

#### Email Attachments

In order to move **'Email Attachments'** to cloud storage of your choice, it is necessary to create Entity Configuration for Email attachments as shown in the below screenshot:

![](<../../.gitbook/assets/Email con\_1.png>)

#### Sales Literature Attachments

Similarly, you need to create the below Entity Configuration to move **'Sales Literature Attachments'**.

![](../../.gitbook/assets/SLA\_1.png)

### **Dropbox Connector:**

* Navigate to **Attach2Dynamics app --> Entity Configuration --> Click on New --> Fill the following fields in 'General' tab --> Click on Save.**
  * **Connector:** Select the Connector.
  * **Entity Name:** Select the entity.
  * **Folder Path Schema:** To populate this field you have to fulfil the following criteria -
    * Selected field should be single line of text.&#x20;
    * Max length of field should be greater than 100.&#x20;
    * Selected field should not be primary field (we suggest custom field because we store path of record in this field).
  * **Folder Path:** This field is auto populated
  * **Attachment Action:** Select either move or copy.
  * **Override Files:** If necessary then enable the checkbox.

![](<../../.gitbook/assets/Entity DB\_1.png>)

* Now go to next tab - **'Email Configuration'** **--> Populate the fields --> Click on Save.**

![](<../../.gitbook/assets/Entity DB\_2.png>)

### **Azure Blob Storage Connector:**

* Navigate to **Attach2Dynamics app --> Entity Configuration --> Click on New --> Fill the following fields in 'General' tab --> Click on Save.**
  * **Connector:** Select the Connector.
  * **Entity Name:** Select the entity.
  * **Folder Path Schema:** To populate this field you have to follow the given criteria.
    * Selected field should be single line of text.&#x20;
    * Max length of field should be greater than 100.&#x20;
    * Selected field should not be primary field (we suggest custom field because we store path of record in this field).
  * **Folder Path:** This field is auto populated
  * **Attachment Action:** Select either move or copy.
  * **Override Files:** If necessary then enable the checkbox.

{% hint style="info" %}
**Note: In case of azure storage the override file will only work if the document content is been modified.**
{% endhint %}

![](../../.gitbook/assets/Azure\_2.png)

* Now go to next tab - **'Email Configuration'** **--> Populate the fields --> Click on Save.**

![](../../.gitbook/assets/Azure\_3.png)

### Activity Entity Configuration

To create entity configuration for Activity Entities, follow the steps given below:

* Navigate to **Attach2Dynamics** **App --> Entity Configurations**.

![](<../../.gitbook/assets/Entity Config for Activity\_1.png>)

* Click on **+New.**

![](<../../.gitbook/assets/Entity Config for Activity\_2.png>)

* Enter the required details to create Entity Configuration for **Email** --> Click on **Save.**

![](<../../.gitbook/assets/Entity Config for Activity\_3.png>)

* For example - If an Account record is set as a Regarding for an Email record then create an entity configuration for the **Account** entity as shown in the below screenshot. Make sure to select either **Copy or Move** as **** an **** attachment action while configuring the entity record.

![](<../../.gitbook/assets/Entity Config for Activity\_4.png>)

* Once the Email is **Sent or Received**, the attachments will get migrated to SharePoint and the email attachment would be uploaded inside an email folder present in the regarding record folder as shown in the below screenshot:

![](<../../.gitbook/assets/Entity Config for Activity\_5.jpg>)

* Similarly, if there are any other entity records as an email regarding then create an Entity configuration for those entities as well.

&#x20;
