# Process-Type Plan for Custom Groups

Sometimes, users need to have a plan for Custom Groups where order of tasks in the plan matters to complete a business process effectively, in this case manager can create a Process-Type plan for Business Process Flow.

This is useful for creating plans for Custom Groups where you want your salesperson to follow the guidelines in a predefined order and not randomly.

To create a Process-Type plan for Custom Groups, follow the steps given below:

* **Fill in the following details:** Name, Description, Plan Type, Priority Order, Record Type.
* **Priority Order:** Users can attach multiple plans to a single record, for which it is necessary to define which plan needs to be connected to the record first. To do this, you can set the priority order against the plan (if the criteria are matching with three different plans, then the plan that has to be followed, we need to set the priority order number respectively). Any value less than 1 or repeated numbers are invalid for this priority order field.
* **Set criteria for the execution of the Plan (Optional):** Set the criteria against the plan (the plan will automatically attach against those for which the criteria match). Select either **Simple** or **Advanced**.
  * **Simple:** Execute plans based on the chosen View of an entity.
  * **Advanced:** Execute plans **** based on filter criteria or conditions (conditions defined in Fetch XML).

<figure><img src="../../../../.gitbook/assets/Custom process new 1.png" alt=""><figcaption></figcaption></figure>

* Select **'Custom Groups'.**

<figure><img src="../../../../.gitbook/assets/Custom process new 1.1.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/Custom process new save plan.png" alt=""><figcaption></figcaption></figure>

Your Process-Type plan for Custom Groups is created, and now you can add the Plan Steps for the newly created plan. To do the same, follow the steps given below:

* Navigate to **Manage Steps**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_1 (1).png" alt=""><figcaption></figcaption></figure>

* Click on the **'Add New Group'** button.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_2 (1).png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create Form: Plan’,** where we need to fill in the details**.**
  * **Name:** Provide an appropriate name for the plan.
  * **Description (Optional):** Provide a short description of the plan.
  * **Priority Order:** Users can attach multiple plans to a single record, for which it is necessary to define which plan needs to be connected to the record first. To do this, you can set the priority order against the plan (if the criteria are matching with three different plans, then the plan that has to be followed, we need to set the priority order number respectively). Any value less than 1 or repeated numbers are invalid for this priority order field.
* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_3 (1).png" alt=""><figcaption></figcaption></figure>

* Click on the **'Create Plan Step'** button.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_5 (1).png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create Form: Plan Step’,** where we need to fill in the details**.**
  * **Name:** Provide an appropriate name for the Plan Step.
  * **Description (Optional):** Provide a short description of the Plan Step.
  * **Add a waiting period for this step (Optional):** A waiting period can be added to define when the plan step should be performed. Once the waiting period is over the plan step actions within the plan step can be performed to eventually complete a plan step. For example, if there is a plan step for getting the lead details and the waiting period for it is set as 2 hours then the plan step actions within the plan step can only be performed after the waiting period ends.
    * **Days:** Add the desired waiting period for this step to be performed after **'X' Days.**
    * **Hours:** Add the desired waiting period for this step to be performed after **'X' Hours.**
* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_6.png" alt=""><figcaption></figcaption></figure>

* Your plan step will be added to the plan and will appear on **Plan Steps**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_7.png" alt=""><figcaption></figcaption></figure>

* &#x20;We can add multiple steps, by clicking on the '**+'** button, as shown below.&#x20;

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_8.png" alt=""><figcaption></figcaption></figure>

* To create Plan Step Actions [click here](https://docs.inogic.com/business-process-checklist/configuration/configuration-for-plans-process/plan-step-action).

In this way, Process-Type plan for Custom Groups can be created with plan steps and plan step actions.

You can also create a [Checklist-Type](https://docs.inogic.com/business-process-checklist/features/manage-plans/create-plan-for-custom-groups/checklist-type-plan-for-custom-groups) plan for Custom Groups.

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
