# Automatic Assignment on Update

As soon as a Lead is created in the system, by default this solution assigns record to the users as per the assignment rule. Automatic assignment works only on creation of the record.

Now there could arise a situation where we may want to assign the record if some specific changes occur in the record. For example, you want to assign Lead record with status reason as **‘Not Ready’** to one set of users and when status reason changes to **‘Ready’** you want to assign the same record to some other set of users.

To enable automatic assignment on update of the record, you would need to make use of Inogic’s action called **‘Inogic.AddItemsToQueue’** action. This action first adds the work items to appropriate queue and then assigns the record to the user.

You can do this in two ways:

* [Using Power Automate Flow](https://docs.inogic.com/lead-assignment-and-distribution-automation/features/automatic-assignments/power-automate-flow)
* [Using Classic Workflow](https://docs.inogic.com/lead-assignment-and-distribution-automation/features/automatic-assignments/classic-workflow)

