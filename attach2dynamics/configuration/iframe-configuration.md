# IFRAME Configuration

{% embed url="https://youtu.be/RFX48jHoIrc" %}

It is possible to add Attach2Dynamics tab embedded in Entity record page directly without having to open it from the Ribbon Button. Here are the steps on how to create embedded tab in the Form of a particular Entity.

* Go to **Settings --> Customizations --> Customize the System**. A Default solution will open.
* Now on the left pane go to **Components --> Entities**.

![](../../.gitbook/assets/Iframe\_1.png)

* Expand the **Entity** drop down --> Select **Forms** for the Entity you want to create embedded tab for.

![](../../.gitbook/assets/Iframe\_2.png)

* Under the **Active Forms** select any **Name** for which **Form Type** is **Main**.

![](../../.gitbook/assets/Iframe\_3.png)

* The **Forms** window will open --> Go to **Insert** tab --> Insert **One** **Column Tab** anywhere on the form framework.

![](../../.gitbook/assets/Iframe\_4.png)

![](../../.gitbook/assets/Iframe\_5.png)

* Go to **Home** --> Click on **Change Properties**.

![](../../.gitbook/assets/Iframe\_6.png)

* A tab **Properties Window** will be opened --> Enter name in **Name and Label** --> Click on **OK**.

![](../../.gitbook/assets/Iframe\_7.png)

![](../../.gitbook/assets/Iframe\_8.png)

* Go to **Insert** tab --> click on **Web Resource**.

![](../../.gitbook/assets/Iframe\_9.png)

* In **Web resource** field enter **ikl\_/Attach2Dynamics/Library/index.html** --> Enter name in **Name and Label** --> **** Scroll down and check the **Pass** **record object-type code and unique identifier as parameters** box --> Click on **OK**.

![](../../.gitbook/assets/Iframe\_10.png)

* Go to **Home** --> Click on **Save** and **Publish**.
* Now navigate to **Entity** (for which you have configured the Form) and open a record--> Scroll down and you can see your desired tab embedded in the page.

![](../../.gitbook/assets/Configuration\_Iframe\_Last.png)

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
