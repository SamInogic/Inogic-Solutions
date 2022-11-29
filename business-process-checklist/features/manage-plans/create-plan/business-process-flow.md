# Process-Type Plan for Business Process Flow

Sometimes, users need to have a plan for Business Process Flow where order of tasks in the plan matters to complete a business process effectively, in this case manager can create a Process-Type plan for Business Process Flow.

This is useful for creating plans for Business Process Flow where you want your salesperson to follow the guidelines in a predefined order and not randomly.

To create a Process-Type plan for Business Process Flow, follow the steps given below:&#x20;

* **Fill in the following plan details:** Name, Description, Plan Type, Priority Order, Record Type.
* **Priority Order:** A **** waiting period can be added to define when the plan step should be performed. Once the waiting period is over the plan step actions within the plan step can be performed to eventually complete a plan step. For example, if there is a plan step for getting the lead details and the waiting period for it is set as 2 hours then the plan step actions within the plan step can only be performed after the waiting period ends.
* **Set criteria for the execution of the Plan (Optional):** Set the criteria against the plan (the plan will automatically attach against those for which the criteria match). Select either **Simple** or **Advanced.**
  * **Simple:** Execute plans based on the chosen View of an entity.
  * **Advanced:** Execute plans based on filter criteria or conditions (conditions defined in Fetch XML).

{% hint style="info" %}
Note: This step is the same for checklist and process - type plans.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/BPF new 2.png" alt=""><figcaption></figcaption></figure>

#### **1)    Simple**&#x20;

Simple criteria can be set on Views of the Record Type.

<figure><img src="../../../../.gitbook/assets/BPF new 3.png" alt=""><figcaption></figcaption></figure>

#### 2) Advanced&#x20;

Plans can be attached based on conditions.&#x20;

For eg. If you want to attach a plan for upcoming leads with the lead source as **"Web"** then you have to enter the Fetch XML for it. Below is the Fetch XML for the same.

<pre><code>&#x3C;fetch version="1.0" output-format="xml-platform" mapping="logical" no-lock="false" distinct="true">
&#x3C;entity name="lead">
&#x3C;attribute name="entityimage_url"/>
&#x3C;attribute name="fullname"/>
&#x3C;order attribute="fullname" descending="false"/>
&#x3C;attribute name="statuscode"/>
&#x3C;attribute name="createdon"/>
&#x3C;attribute name="subject"/>
<strong>&#x3C;attribute name="leadid"/>
</strong>&#x3C;filter type="and">
&#x3C;condition attribute="statecode" operator="eq" value="0"/>
&#x3C;condition attribute="leadsourcecode" operator="eq" value="8"/>
&#x3C;/filter>
&#x3C;/entity>
&#x3C;/fetch></code></pre>

In the same way, you can set Advanced criteria for other plan records as well.

<figure><img src="../../../../.gitbook/assets/BPF new 4.png" alt=""><figcaption></figcaption></figure>

* Select **'Business Process Flow'.**
* Select Business Process Flow to which the plan will be attached.

<figure><img src="../../../../.gitbook/assets/BPF new 6.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/BPF new 8 (1).png" alt=""><figcaption></figcaption></figure>

Your Process-Type plan for Business Process Flow is created and now you can add the Plan Steps inside the various stages of the selected Business Process Flow. To do the same, follow the steps given below:

* Navigate to **Manage Steps**.
* Here, as per the Business Process Flow selected by the manager, various stages of the selected Business Process Flow will be displayed. The manager now selects the desired stages and creates the plan step and plan step action inside the stages.
* **For example:** Here we have selected the Business process flow of the **Lead to Opportunity Sales Process,** and the stages are Qualify, Develop, Propose, and Close of the **Lead to Opportunity Sales Process** which **** will **** automatically be displayed as shown below.
* Now, select the required BPF stage, for example, select the **Qualify** stage.
* Click on the **'Create Plan Step'** Button.

<figure><img src="../../../../.gitbook/assets/BPF steps 1 (1).png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create Form: Plan Step’,** where we need to fill in the details**.**
  * **Name:** Provide an appropriate name for the Plan Step.
  * **Description (Optional):** Provide a short description of the Plan Step.
  * **Add a waiting period for this step (Optional):** Waiting period can be added to define when the plan step should be performed. Once the waiting period is over the plan step actions within the plan step can be performed to eventually complete a plan step. For example, if there is a plan step for getting the lead details and the waiting period for it is set as 2 hours then the plan step actions within the plan step can only be performed after the waiting period ends.
    * **Days:** Add the desired waiting period for this step to be performed after **'X'** **Days**.
    * **Hours:** Add the desired waiting period for this step to be performed after **'X'** **Hours.**

<figure><img src="../../../../.gitbook/assets/BPF step 3 (1) (1).png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/BPF step 3.png" alt=""><figcaption></figcaption></figure>

* Your plan step will be added to the process and will appear on plan steps.

<figure><img src="../../../../.gitbook/assets/BPF step 4 (1).png" alt=""><figcaption></figcaption></figure>

* And now you can add the actions inside the plan step created for the selected stage.

<figure><img src="../../../../.gitbook/assets/BPF_ 14.png" alt=""><figcaption></figcaption></figure>

* To create Plan Step Actions [click here](https://docs.inogic.com/business-process-checklist/configuration/configuration-for-plans-process/plan-step-action).

In this way, Process-Type plans for Business Process Flow can be created with plan steps and plan step actions.

You can also create a [Checklist-Type](https://docs.inogic.com/business-process-checklist/features/manage-plans/create-plan-for-business-process-flow/checklist-type-plan-for-business-process-flow) plan for Business Process Flow.

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
