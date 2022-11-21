# Data Migration

How to migrate configurations, plans, plan steps, and plan step actions from one environment to another.

The process of migrating configurations from one environment to another can be divided into two parts:

* Export configuration from one environment
* Import the same configuration in another environment

### Export configurations from one environment to another

Before exporting the configurations, create a **custom view** on **'Business Process Checklist configuration'** in the environment from which the configuration is to be moved in the following way:

* Navigate to **Settings** --> **Customizations.**

<figure><img src="../../.gitbook/assets/data migration_1.png" alt=""><figcaption></figcaption></figure>

* Click on **'Customize the System'.**

<figure><img src="../../.gitbook/assets/data migration_2.png" alt=""><figcaption></figcaption></figure>

* Navigate to **Entities** --> **Business Process Checklist** --> **Views**.

<figure><img src="../../.gitbook/assets/data migration_3.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_4.png" alt=""><figcaption></figcaption></figure>

* Click on **'New'** to create a new view.

<figure><img src="../../.gitbook/assets/data migration_5.png" alt=""><figcaption></figcaption></figure>

* Enter an appropriate name for the view and click **'Ok'** to proceed.

<figure><img src="../../.gitbook/assets/data migration_6.png" alt=""><figcaption></figcaption></figure>

* Click on **'Add Columns'.**

<figure><img src="../../.gitbook/assets/data migration_7.png" alt=""><figcaption></figcaption></figure>

* You can keep the following column names disabled -  **Created by, Created by (Delegate), Created on, Modified by, Modified by (Delegate), Modified on and Record created on.**

<figure><img src="../../.gitbook/assets/data migration_8.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_9.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_10.png" alt=""><figcaption></figcaption></figure>

* Click **'Ok'** to proceed.

<figure><img src="../../.gitbook/assets/data migration_11.png" alt=""><figcaption></figcaption></figure>

* Click **'Save/Save & Close'** icon to save this view.

<figure><img src="../../.gitbook/assets/data migration_12.png" alt=""><figcaption></figcaption></figure>

* You can see the view that has just been added.

<figure><img src="../../.gitbook/assets/data migration_13.png" alt=""><figcaption></figcaption></figure>

* Click on **'Publish All Customizations'.**

<figure><img src="../../.gitbook/assets/data migration_14.png" alt=""><figcaption></figcaption></figure>

* Go back to **Business Process Checklist** application --> Business Process Checklist **Configurations** --> Select the **Export View.**

<figure><img src="../../.gitbook/assets/data migration_16.png" alt=""><figcaption></figcaption></figure>

* Click on **'Export to Excel'.**

<figure><img src="../../.gitbook/assets/data migration_17.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_18.png" alt=""><figcaption></figcaption></figure>

* After clicking on **'Export to Excel'**, a file with an extension **'.xlsx'** will be downloaded. **Open** this file and **save** it as **.csv format** in the system.
* Click **'Ok'.**
* Once you have successfully created the .csv version of the exported file, let’s proceed to import operation.

### Import the same configuration in another environment

* Login to the other environment to which we want to import the template --> Navigate to **Business Process Checklist** application **--> BPC Settings** --> **Business Process Checklist Configurations.**

<figure><img src="../../.gitbook/assets/data migration_19.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_20.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_21.png" alt=""><figcaption></figcaption></figure>

* **Import** the same **.csv** file.

<figure><img src="../../.gitbook/assets/data migration_22.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_23.png" alt=""><figcaption></figcaption></figure>

* Browse the **.csv** file.

<figure><img src="../../.gitbook/assets/data migration_31 new.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_32 new.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/data migration_33 new.png" alt=""><figcaption></figcaption></figure>

* Click on **Review Mapping**.

<figure><img src="../../.gitbook/assets/data migration_27.png" alt=""><figcaption></figcaption></figure>

* Click **'Finish Import'** without changing any of the below fields.

<figure><img src="../../.gitbook/assets/data migration_28.png" alt=""><figcaption></figcaption></figure>

* Click on **Confirm.**

<figure><img src="../../.gitbook/assets/data migration_29.png" alt=""><figcaption></figcaption></figure>

* Click on **Done.**

<figure><img src="../../.gitbook/assets/data migration_30.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
