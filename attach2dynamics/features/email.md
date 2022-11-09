# Email

Users also have an option to send an email for both Non-activity and Activity entities.&#x20;

### For Non-activity Entity:

There are two options for this – send as Link or Attachment.

* **Links:** On selecting this option you can insert the file’s/folder’s link in the email body. The below window opens on choosing the option ‘Link’ with link of file in email body.
* **Attach Documents:** On selecting this option you can attach the file itself in the email body. The below window opens with file as attachment by choosing ‘Attach.’

<figure><img src="../../.gitbook/assets/Email files as an attachment or share the link to the files- slide 17.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Email files as an attachment or share the link to the files- slide 17 image 2.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Email files as an attachment or share the link to the files- slide 17 image 3.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note: Email can be sent only with files and not folders. Also, multiple files can be sent in a single mail.**
{% endhint %}

### For Activity Entity (Email):

To directly send an email with multiple attachments, please follow the steps given below:

* First, create the Connector record in Attach2Dynamics App. Please follow this [link](https://docs.inogic.com/attach2dynamics/configuration/connector-configuration/sharepoint) for directions.
* Next, create an entity configuration record for the **Email** entity.
* Now you have to create an entity configuration record for the entity which will be selected in the **Regarding field** of **** the **Email**. Follow [this link](https://docs.inogic.com/attach2dynamics/configuration/entity-configuration) for directions to create entity configuration.
* Navigate to the Email form --> Set the entity record that you want to view in Attach2Dynamics UI in the **Regarding** field --> Click on the **Attach2Dynamics** button.
* You will be able to see the files and folders present in the SharePoint site of the record present in the **Regarding** field as shown below:

![](<../../.gitbook/assets/Image1 (1).png>)

![](<../../.gitbook/assets/Image2 (1).png>)

* Select the file --> Click on the **Email** button to attach the file as an **attachment** or as a **link** in the email.

![](<../../.gitbook/assets/Image3 (1).png>)

* In the case of **Attach Documents**, the file will be added as an attachment in the email attachment section.

![](<../../.gitbook/assets/Image4 (1).png>)

* In the case of **Links**, the link of the SharePoint folder location of the selected file will be added as a link in the email body.

![](<../../.gitbook/assets/Image5 (1).png>)

