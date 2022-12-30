# View Plan Items on Record

For CRM users to follow plans created by managers and complete business processes by following best practices, they can do so by seeing these plans on the records as well. To make plan items appear on associated records, follow the steps given below:

This can be done in the following two ways:

* Using Classic UI
* Using Power Apps UI

### Using Classic UI

* Navigate to **Settings** --> **Customizations.**

<figure><img src="../../.gitbook/assets/1 (35).png" alt=""><figcaption></figcaption></figure>

* Click on **'Customize the System'.**

<figure><img src="../../.gitbook/assets/2 (67).png" alt=""><figcaption></figcaption></figure>

* Navigate to **Entities** --> **Lead** --> **Forms**.

<figure><img src="../../.gitbook/assets/3 (30).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/4 (36).png" alt=""><figcaption></figcaption></figure>

* Click on Lead Entity with Form Type Main.

<figure><img src="../../.gitbook/assets/5 (30).png" alt=""><figcaption></figcaption></figure>

* Select (or Add) the section where you want Plan on Record Form.

<figure><img src="../../.gitbook/assets/6 (9).png" alt=""><figcaption></figcaption></figure>

* Click on **‘Change Properties’.**

<figure><img src="../../.gitbook/assets/7 (21).png" alt=""><figcaption></figcaption></figure>

* This will open a **'Section Properties'** form, where you can modify section’s properties.
* Once the required fields are filled, Click **‘OK’**.

<figure><img src="../../.gitbook/assets/8 (11).png" alt=""><figcaption></figcaption></figure>

* Go to **‘Insert’** Click on **Sub-Grid**.

<figure><img src="../../.gitbook/assets/9 (7).png" alt=""><figcaption></figcaption></figure>

* This will open a **'Set Properties'** form, where you need to fill in the details.
  * **Records:** Select **‘Only Related Records’.**
  * **Entity:** Select **‘Record Plans (Regarding)’.**
  * **Default View:** Select **‘All Record Plans’.**
* Go to **Controls.**

<figure><img src="../../.gitbook/assets/10 (6).png" alt=""><figcaption></figcaption></figure>

* Click on **‘Add Control’.**

<figure><img src="../../.gitbook/assets/11 (14).png" alt=""><figcaption></figcaption></figure>

* Select **‘Record Plan Items’** and click on Add.

<figure><img src="../../.gitbook/assets/12 (11).png" alt=""><figcaption></figcaption></figure>

* Select the desired options and click on **‘OK’**.

<figure><img src="../../.gitbook/assets/13 (1).png" alt=""><figcaption></figcaption></figure>

* Click on **‘Save’.**

<figure><img src="../../.gitbook/assets/14 (1).png" alt=""><figcaption></figcaption></figure>

* Click on **‘Publish’.**

<figure><img src="../../.gitbook/assets/15.png" alt=""><figcaption></figcaption></figure>

* Now plan will get displayed on the **‘Record Form’.**

<figure><img src="../../.gitbook/assets/16.png" alt=""><figcaption></figcaption></figure>

### **Using Power Apps UI**

* Go to [https://make.powerapps.com/](https://make.powerapps.com/).

<figure><img src="../../.gitbook/assets/1 (2) (1).png" alt=""><figcaption></figcaption></figure>

* Select the Environment.

<figure><img src="../../.gitbook/assets/2 (2) (2).png" alt=""><figcaption></figcaption></figure>

* Navigate to Dataverse **--> Tables**.

<figure><img src="../../.gitbook/assets/3 (2).png" alt=""><figcaption></figcaption></figure>

* Go to All and search for the required Entity.

<figure><img src="../../.gitbook/assets/4 (3).png" alt=""><figcaption></figcaption></figure>

* Click on the desired Entity.

<figure><img src="../../.gitbook/assets/5 (4).png" alt=""><figcaption></figcaption></figure>

* Click on Entity ‘Forms’.

<figure><img src="../../.gitbook/assets/6 (2).png" alt=""><figcaption></figcaption></figure>

* Click on Lead Entity with Form Type Main.

<figure><img src="../../.gitbook/assets/7 (1).png" alt=""><figcaption></figcaption></figure>

* Select (or Add) the section where you want Plan on Record Form.

<figure><img src="../../.gitbook/assets/8.png" alt=""><figcaption></figcaption></figure>

* Go to **‘Properties’.**
  * **Label:** Provide a unique name for the section label.

<figure><img src="../../.gitbook/assets/9.png" alt=""><figcaption></figcaption></figure>

* Go to **‘Components’.**

<figure><img src="../../.gitbook/assets/10 (2).png" alt=""><figcaption></figcaption></figure>

* Click on ‘Grid’.

<figure><img src="../../.gitbook/assets/11.png" alt=""><figcaption></figcaption></figure>

* Click on **‘Subgrid’.**

<figure><img src="../../.gitbook/assets/12 (2).png" alt=""><figcaption></figcaption></figure>

* This will open **'Select subgrid views'** form, where you need to fill in the details.
  * **Select ‘Show related records.**
  * **Table:** Select **‘Record Plans (Regarding)’.**
  * **Default view:** Select **‘All Record Plans’.**
* Once the required fields are filled, click on **‘Done’.**

<figure><img src="../../.gitbook/assets/13.png" alt=""><figcaption></figcaption></figure>

* Go to **‘Properties’.**
  * **Label:** Provide a unique label name for the **subgrid.**

<figure><img src="../../.gitbook/assets/14.png" alt=""><figcaption></figcaption></figure>

* Go to **Components** and click on **‘+ Components’.**

<figure><img src="../../.gitbook/assets/15 (1).png" alt=""><figcaption></figcaption></figure>

* Select **‘Record Plan Items’.**

<figure><img src="../../.gitbook/assets/16 (1).png" alt=""><figcaption></figcaption></figure>

* Select the required **"Show component on"** options and click on **‘Done’.**

<figure><img src="../../.gitbook/assets/17.png" alt=""><figcaption></figcaption></figure>

* Click on **‘Save’.**

<figure><img src="../../.gitbook/assets/18.png" alt=""><figcaption></figcaption></figure>

* Click on **‘Publish’.**

<figure><img src="../../.gitbook/assets/19.png" alt=""><figcaption></figcaption></figure>

* Now plan will get displayed on the **‘Record Form’.**

<figure><img src="../../.gitbook/assets/20.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
