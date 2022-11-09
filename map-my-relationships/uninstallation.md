# Uninstallation

Uninstalling **Map My Relationships** solution from your CRM environment is quite simple. Just follow the below process to uninstall **Map My Relationships** from your Dynamics 365 CRM.

{% hint style="info" %}
**Note: In order to uninstall Map My Relationship view, you first need to remove the dependency of Map My Relationships/Map My Connections control from the Entity Forms. If you have added the control on any entity forms then remove that control from the form. In below steps we have taken the example of Account entity.**
{% endhint %}

1\) Navigate to **Settings** ->**Customizations** ->**Customize the System.**

![](<../.gitbook/assets/21 (3).png>)

2\) From there go to **Entities** ->**Account** ->**Forms** ->Select the respective ‘Form’ for which controls are set.

![](<../.gitbook/assets/22 (1).png>)

3\) Double click on **Form** ->Click the field on which control is set.

![](../.gitbook/assets/23.png)

4\) Now go to **Controls** -> Delete **Map My Relationships** Control -> Click **OK** -> Click on **Save and Publish**.

![](../.gitbook/assets/24.png)

5\) Similarly, to remove Map My Connections control, go to **Default Solution** -> Select **Opportunity** -> **Forms** -> **Main Form**.&#x20;

![](<../.gitbook/assets/Uninstall\_1 (3).png>)

6\) Double click on **Form** -> Click the field on which control is set.

![](../.gitbook/assets/Uninstall\_2.png)

7\) Now go to **Controls** -> Delete **Map My Connections** Control -> Click **OK** -> Click on **Save and Publish**.

![](../.gitbook/assets/Uninstall\_3.png)

8\) Next, navigate to **Settings** --> **Solution** --> Select **Map My Relationships** solution.

![](<../.gitbook/assets/2 (32).png>)

9\) Click on **delete** button. A pop-up will appear asking for your confirmation. Click on **OK** and the solution will be uninstalled from your environment.

![](<../.gitbook/assets/3 (5).png>)

![](<../.gitbook/assets/uninstall\_5 - Copy (1).png>)
