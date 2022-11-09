# Prerequisite

After license registration there are some steps to be taken to ensure smooth functioning of Lead Assignment and Distribution Automation app. This includes **activating** the workflows that assign Dynamics 365 CRM records as per the assignment rule set by the user. There are two types of workflows – **Classic Workflow** and **Power Automate Flow**. Now, depending upon one’s requirement these workflows can be activated or deactivated.

{% hint style="info" %}
**Note: By default, Power Automate Flow is active and Classic workflows are in draft state.**
{% endhint %}

To check whether the workflows are activated or not, follow the steps given below.

### Classic Workflow

* Navigate to **Advanced Settings.**&#x20;

![](../.gitbook/assets/Prereq\_1.png)

* Go to **Settings --> Process Center --> Processes.**&#x20;

![](../.gitbook/assets/Prereq\_2.png)

* Select the workflows --> Click on **Activate** button.

![](<../.gitbook/assets/Classic vacation workflow\_1.png>)

### Power Automate Flow

* Go to [flow.microsoft.com ](https://us.flow.microsoft.com/en-us/)--> Select the environment.&#x20;

![](../.gitbook/assets/Prereq\_4.png)

* Go to **Solutions**.&#x20;

![](../.gitbook/assets/Prereq\_5.png)

* Select **Lead Assignment and Distribution Automation** solution --> Search for workflows.&#x20;

![](<../.gitbook/assets/Power Automate vacation flow\_1.5.png>)

* Select the workflow --> By default it is kept activated so the **‘Turn Off’** button is available on the ribbon.

![](<../.gitbook/assets/Power Automate vacation flow\_1.png>)

![](<../.gitbook/assets/Power Automate vacation flow\_2.png>)

### Adding Time Zone

In **'Inogic.DailyUpdateUserStatus'** workflow it is necessary to set time zone for the workflow to function smoothly. To update time zone please follow the steps below:

* Select the workflow --> Click on **Edit**.

![](<../.gitbook/assets/Power Automate timezone\_1.png>)

* Click on the first step 'Recurrence' --> Click on **Edit.**

![](<../.gitbook/assets/Power Automate timezone\_2.png>)

* Click on **' Show advanced options'.**

![](<../.gitbook/assets/Power Automate timezone\_3.png>)

* Select the preferable time zone --> Click on **'Save'.**

![](<../.gitbook/assets/Power Automate timezone\_4.png>)



