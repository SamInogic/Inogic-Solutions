# Copy references of records

The next step is copying references of records on both **source** and **target** entities under **advanced configuration**.

Now to add these source and target lookup fields please follow the steps given below:

* Navigate to **Settings** --> **Customizations**.

![](../../../.gitbook/assets/Clone1\_2.1.png)

* Click on **Customize the System**.

![](../../../.gitbook/assets/Clone1\_2.2.png)

* Go to **Entities** --> **Order** --> **Fields** --> **Add new field**.

![](../../../.gitbook/assets/Clone1\_2.3.png)

* Add a **source lookup** field --> Click on **Save** & **close it**. (Note down the name of the field, we will need this name later while setting the reference against the target entity field under advanced configuration.)

![](../../../.gitbook/assets/Clone1\_2.4.png)

* Add a **target lookup** field --> Click on **Save & Close**. (Note down the name of the field, we will need this name later while setting the reference against the source entity field under advanced configuration.)

![](../../../.gitbook/assets/Clone1\_2.5.png)

* Go to **Forms** --> **Main form**.

![](../../../.gitbook/assets/Clone1\_2.6.png)

* Add a **source record field** to the form. (This is the source lookup field that we added earlier.)

![](../../../.gitbook/assets/Clone1\_2.7.png)

* Same way add a **target field** to the form. (This is a target lookup field that we added earlier.)

![](../../../.gitbook/assets/Clone1\_2.8.png)

* Once the both the fields are added, click on **'Save'** and then click on **'Publish'.**

![](../../../.gitbook/assets/Clone1\_2.9.png)

* Close the window and click on **'Publish All Customization'**.

![](../../../.gitbook/assets/Clone1\_2.10.png)

* Navigate back to **Click2Clone Templates** --> **Advanced Configuration** --> **Set the references**. Set the **target** lookup field against **'Source Entity'** and **source** lookup field against **'Target Entity'**. Enter the names of both these look fields into respective fields. (These are names that we have noted down while creating the fields through customization.)

![](../../../.gitbook/assets/Clone1\_2.11.png)

Once you have completed all the steps, you will be able to:

* [Clone single record](https://docs.inogic.com/click2clone/features/clone-single-record)
* [Clone multiple records](https://docs.inogic.com/click2clone/features/clone-multiple-records)
* [Create multiple copies of a record](https://docs.inogic.com/click2clone/features/multiple-copies-of-a-record)
