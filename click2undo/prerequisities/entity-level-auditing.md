# Entity Level Auditing

After enabling [Organization Level Auditing](https://docs.inogic.com/click2undo/prerequisities/organization-level-auditing), the next important step is to enable Entity Level Auditing. For all the entities that needs to be leveraging Click2Undo feature you need to follow below steps in order to enable Entity Level Auditing.&#x20;

{% hint style="info" %}
**Note : The below illustration is done using Account entity, but the same process can be followed for the other system or custom entities as well.**
{% endhint %}

1\) Open [https://admin.powerplatform.microsoft.com/environments](https://admin.powerplatform.microsoft.com/environments)

2\) Open Settings by selecting the correct environment.

![](<../../.gitbook/assets/image (150).png>)

3\) Search for Entity and field audit settings.

![](<../../.gitbook/assets/image (195).png>)

4\) It opens the Default Solution.

&#x20;

![](<../../.gitbook/assets/image (7).png>)

5\) Expand Entities --> Click on Account --> Enable Auditing.

![](<../../.gitbook/assets/image (205).png>)

6\) Save and Publish.

![](<../../.gitbook/assets/image (46).png>)

{% hint style="info" %}
**Note: By default, all fields for the selected entity are enabled for auditing.**
{% endhint %}

#### Disable/Enable Auditing Specific Field&#x20;

By default, Auditing is enabled for all the fields for the enabled entity. If you want, you can pick and choose which fields should be enabled/disabled for Auditing.&#x20;

To achieve this, follow the steps given below:

1\) Select Fields Tab.

![](<../../.gitbook/assets/image (158).png>)

2\) Select the field for which you would like to disable the auditing and click Edit.

![](<../../.gitbook/assets/image (27).png>)

3\) Select Disable --> Click on Save and Close.

![](<../../.gitbook/assets/image (102).png>)

4\) Publish the customizations.

**Now, let's look into alternate approach for enabling Entity Level Auditing.**

1\) Click on Advanced Settings from within Dynamics 365 CRM.

![](<../../.gitbook/assets/image (175).png>)

2\) Click on Customizations.

![](<../../.gitbook/assets/image (132).png>)

3\) Click on Customize the System.

![](<../../.gitbook/assets/image (97).png>)

4\) It opens the Default Solution.

![](<../../.gitbook/assets/image (26).png>)

5\) Expand Entities --> Click on Account --> Enable Auditing.

![](<../../.gitbook/assets/image (82).png>)

6\) Save and Publish.

![](<../../.gitbook/assets/image (197).png>)

__
