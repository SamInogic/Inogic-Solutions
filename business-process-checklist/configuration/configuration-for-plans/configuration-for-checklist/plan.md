# Plan

To create a Checklist-Type plan, you need to create a plan first. Plans consist of multiple tasks/plan steps that are needed to be performed to complete a business process successfully.

Below are the steps for creating a Checklist-Type plan:

* Navigate to **Business Process Checklist App** **--> Plans --> New Plan**

<figure><img src="../../../../.gitbook/assets/Configuration entity _1.png" alt=""><figcaption></figcaption></figure>

* Click on the **'New plan'** button and select **Checklist.**

<figure><img src="../../../../.gitbook/assets/Configuration entity checklist _2.png" alt=""><figcaption></figcaption></figure>

* This will open a **'New Plan',** page where you need to fill in the details.
  * **Name:** Provide a unique name for the plan.
  * **Description:** Provide a short description of the plan.
  * **Record Type:** Select the **Record Type** for which the plan will be created. (E.g. Lead, Opportunity, Case, or Custom record type etc.)
  * **Plan Type:** Select Plan Type **** as **Checklist**.
  * **Priority Order:** Users can attach multiple plans to a single record, for which it is necessary to define which plan needs to be connected to the record first. To do this, you can set the priority order against the plan (if the criteria are matching with three different plans, then the plan that has to be followed, we need to set the priority order number respectively). Any value less than 1 or repeated numbers are invalid for this priority order field.
  * **Set criteria for the execution of the plan (Optional):** Set the criteria against the plan (the plan will automatically attach against those for which the criteria match). Select either **Simple** or **Advanced**.
    * **Simple:** Execute plans based on the chosen View of an entity.
    * **Advanced:** Execute plans **** based on filter criteria or conditions (conditions defined in Fetch XML).
* **Plan for (Optional)**: Users can create plans for **Business Process Flow** or **Custom Groups.** (If neither business process nor custom groups are selected, then the plan will be automatically created for the record type selected.)
  * **Business Process Flow:** Select **Business Process Flow** to create a Checklist-Type plan for Custom or OOB [Business Process Flows.](https://docs.inogic.com/business-process-checklist/features/manage-plans/create-plan-for-business-process-flow/checklist-type-plan-for-business-process-flow) &#x20;
  * **Custom Groups:** Select **Custom Groups** to create a Checklist-Type plan for [Custom Groups.](https://docs.inogic.com/business-process-checklist/features/manage-plans/create-plan-for-custom-groups/checklist-type-plan-for-custom-groups)

{% hint style="info" %}
**Note: If either business process or custom groups are selected, then the plan will be created for the record by default.**
{% endhint %}

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/Plan_4 (1).png" alt=""><figcaption></figcaption></figure>

* The new plan will be created and can be seen on **Plans**.

<figure><img src="../../../../.gitbook/assets/Publish checklist.png" alt=""><figcaption></figcaption></figure>

Now that we have created a plan, let’s add [plan steps](https://docs.inogic.com/business-process-checklist/features/manage-plans/create-plan/create-checklist-type-plan/plan-step) to the plan.

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
