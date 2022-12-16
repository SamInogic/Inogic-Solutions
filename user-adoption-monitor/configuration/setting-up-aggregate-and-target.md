# Setting up Goal

### Aggregate Tracking&#x20;

Using **‘Aggregate Tracking’**, one can track the aggregations of respective numeric field(s) of the entity on which the specific user action has been defined. To understand better, let’s take an example of **‘Opportunity-win’** action.&#x20;

In order to configure ‘Aggregate Tracking’ follow the steps given below:

* Navigate to **User Adoption Monitor App --> Entity Configuration --> Click on New.**

![](<../../.gitbook/assets/Agg Trac\_1.png>)

* Fill the given fields --> Click on **Save**.
  * **Entity label:** Opportunity&#x20;
  * **Entity Schema:** opportunity&#x20;
  * **Message:** win&#x20;
  * **Period:** Select either Daily, Weekly or Monthly.

{% hint style="info" %}
**Note: If the respective entity configuration is already present, then no need to follow the above steps to recreate the same entity configuration. One can directly open the entity configuration record and follow the below procedure to define the Aggregate Configuration.**
{% endhint %}

* Once it is saved, the sub-grids to define the **Aggregate Configurations** and **Target Configurations** will be displayed.

![](<../../.gitbook/assets/Agg Trac\_2.png>)

* Now, create a new **Aggregate Configuration** as shown below:

![](<../../.gitbook/assets/Agg Trac\_3.png>)

* Fill the following fields --> Click on **Save**.
  * **Aggregate On:** Select any attribute from the dropdown on which you want to calculate the aggregation. **** Here, we will take example of **Actual Revenue.**&#x20;
  * **Aggregate Type:** Select **‘SUM**’ or **‘AVG’**. This field will calculate the aggregation as Sum or Average of the chosen field. Here, we will take example of **SUM.**

![](<../../.gitbook/assets/Agg Trac\_4.png>)

* Once this is configured, every time a user **wins** an **opportunity**, User Adoption Monitor will calculate and show the sum of the actual revenue of Opportunities won by the respective users on daily, weekly or monthly basis.

In addition to this, there is another functionality incorporated in User Adoption Monitor that gives the provision to calculate the aggregation for specific statuses of the entity record on **‘Update’** entity action.&#x20;

For better understanding, let’s consider the following business scenario:

Admin/user having **‘User Adoption Monitor Administrator’** privileges wants User Adoption Monitor to track the aggregation on updating the opportunity record only when the status of an opportunity is **‘In progress’.**&#x20;

Let’s follow the below steps to accomplish the above requirement**:**

* Navigate to **Manage Entity Action** **-->** Set the period as required for opportunity-update action (It is set to **‘Daily’** in this example) --> Click on **Save**.

![](<../../.gitbook/assets/Agg Upd\_1.png>)

* Once the above entity action is saved successfully, you will see the **‘Opportunity-update’** entity configuration created under **‘Active User Adoption Entity Configuration’.**

![](<../../.gitbook/assets/Agg Upd\_2.png>)

* Open this **‘Opportunity-update’** configuration and create a new **‘Aggregate Configuration’** as shown below:

![](<../../.gitbook/assets/Agg Upd\_3.png>)

* Select the required attribute from the list. Here, user can pick any attribute based on the business requirement. ‘**Actual Revenue’** attribute is selected in this example as we want User Adoption Monitor to calculate and track the aggregate value of this field upon updating the opportunity record.
* We are keeping the **‘Aggregate Type’** as **‘SUM’** since we want to calculate the sum of actual revenue of total number of opportunities that are won.

![](<../../.gitbook/assets/Agg Upd\_4.png>)

* Select the status as **‘Open – In Progress’**. Now, it would track the aggregation of the **Actual Revenue** field post updating the opportunity only if the status of an opportunity is **‘In Progress’**.

![](<../../.gitbook/assets/Agg Upd\_5.png>)

* Now, let’s save this aggregate configuration with the below values:&#x20;
  * **Aggregate On:** Actual Revenue
  * **Aggregate Type:** Sum&#x20;
  * **Status:** Open – In Progress
* Once saved, this configuration will appear under ‘Active User Adoption Aggregate Configurations’ as shown below:

![](<../../.gitbook/assets/Agg Upd\_6.png>)

* Next, let’s update the below opportunity. This opportunity has the actual revenue of **$10,000.**

![](<../../.gitbook/assets/Agg Upd\_7.png>)

* Any of the fields from this opportunity record can be modified. Here, **‘Budget Amount’** field is updated to **$20,000**.

![](<../../.gitbook/assets/Agg Upd\_8.png>)

* We have set the status as **‘Open – In Progress’** in aggregate configuration earlier. Since the status of the opportunity remains **‘In Progress’** when the opportunity was updated with **‘Budget Amount’,** this will be tracked and aggregate value of the field **‘Actual Revenue’** will be calculated.
* To check the track entry, navigate to **User Adoption Monitor --> Entity Configuration --> Open ‘Opportunity-update’ entity configuration.**

![](<../../.gitbook/assets/Agg Upd\_9.png>)

{% hint style="info" %}
**Note: The way the User Adoption Monitor works in this is, it compares the status of the opportunity against the status that we have set in the aggregate configuration and tracks the aggregation only if these statuses match with each other.**
{% endhint %}

### Target Tracking

Using **‘Target Tracking’** one can allot and keep track of targets assigned to respective users in Dynamics 365 CRM. The targets can either be assigned against the count of the actions performed or against the aggregate value. Let’s take the above example of **‘Opportunity-win’** action.

Follow the steps given below for **‘Target Configurations’**.

#### Target based on Aggregation Value

* First, create entity configuration for **‘Opportunity-win’** --> Configure **‘Aggregate Tracking’** --> Go to **‘Active User Adoption Target Configurations’** --> Click on **‘New Target Configuration’.**

![](<../../.gitbook/assets/Targ Agg\_1.png>)

* Fill the following fields --> Click on **Save**.
  * **Aggregate Configuration:** Select an **‘Aggregate Configuration’** associated to the same Entity Configuration as that on the Target Configuration form.&#x20;
  * **Target:** Set a value.&#x20;
  * **Interval:** Select either **‘Recurring’** or **‘Fixed’**.

![](<../../.gitbook/assets/Targ Agg\_2.png>)

* Next, add the user for whom the target is set --> Click on **Save & Close**. With this target for **‘Actual Revenue’** to be achieved has been set for the respective user.

![](<../../.gitbook/assets/Targ Agg\_3.png>)

* Now, one can monitor the performance of the users by comparing the target set and the total target achieved by them over a given period of time.

#### Target based on Count

In the same way one can set target based on count for users. Taking the above example as base, follow the steps given below:

* Create entity configuration for **‘Opportunity-win’** --> Configure **‘Aggregate Tracking’** --> Go to **‘Active User Adoption Target Configurations’** --> Click on **‘New Target Configuration’.**

![](<../../.gitbook/assets/Targ Cou\_1.png>)

* Fill the following fields --> Click on **Save.**
  * **Aggregate Configuration:** Keep this field empty.&#x20;
  * **Target:** Set a value.&#x20;
  * **Interval:** Select either **‘Recurring’** or **‘Fixed’**.

![](<../../.gitbook/assets/Targ Cou\_2.png>)

* Next, add the user for whom the target is set --> Click on **Save & Close**. With this the number of targets to be achieved for a given period has been set for the respective user.
* Now, one can monitor and compare the target set and the total target achieved by users for a given period of time.

#### Target defined for Fixed Interval

In the above two scenarios, we defined Targets with the Interval set as **‘Recurring’**. However, we do have another option i.e., to define the Target for a fixed period of time by setting the **Interval** as **Fixed**.

On setting the interval of the Target Configuration as fixed, two datetime fields i.e. the **Start Date** and **End Date** shows up using which one can define the period for which they want to set the target against tracking.

{% hint style="info" %}
**Note: The Start Date and End Date must be within the period of the associated Entity Configuration. For example, if the Period of the associated Entity Configuration is.**&#x20;

* **Daily:** The Start and End date must be the same date, i.e. **8th August 2020 – 8th August 2020.**
* **Weekly:** The Start and End date must be within the same week i.e. **Sunday to Saturday.**
* **Monthly:** The Start and End date must be within the same month, i.e. **1st August 2020 – 31st August 2020.**
{% endhint %}

Similar steps needed to be followed for the creation of the **Target configuration** for **fixed** interval:

* Create the respective entity configuration record if not already created. Then open that record and from the sub-grid for Target Configuration create a new Target Configuration.

![](<../../.gitbook/assets/Targ Fix\_1.png>)

* Fill the following fields --> Click on **Save.**
  * **Aggregate Configuration:** You may or may not select the aggregate configuration associated to the entity configuration.&#x20;
  * **Target:** Set a value&#x20;
  * **Interval:** Select **‘Fixed’**. On selecting the Interval as fixed, the below two Datetime fields show up to define the period.
    * **Start Date:** Set the date from when the tracking will be captured against this defined target for respective users.
    * **End Date:** Set the date till when the target tracking shall take place.

{% hint style="info" %}
**Note:**&#x20;

* **Once the start date is entered, the status reason of the target configuration record gets updated to ‘In Progress’. And only the In Progress target configurations are considered for target tracking.**
* **On the date next to the end date the status reason of the target configuration shall get updated to Complete and once the status reason gets updated to complete, no further target tracking shall happen for this specific target configuration.**
{% endhint %}

![](<../../.gitbook/assets/Targ Fix\_2.png>)

* Next, add the user for whom the target is set --> Click on **Save & Close.**
* With this, one can monitor and compare the target set and the total target achieved by users for a given fixed period of time.

![](<../../.gitbook/assets/Targ Fix\_3.png>)

![](<../../.gitbook/assets/Aggre Track.png>)

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
