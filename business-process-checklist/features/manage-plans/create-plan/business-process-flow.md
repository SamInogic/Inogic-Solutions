# Business Process Flow

With this feature, you can create both **Process** and **Checklist** - **** type plans against **Business Process Flow.**

For example, if a user wants to create a plan against the **Lead to Opportunity Sales process** to set the best practices for **Lead Nurturing**. **** In order to achieve this, the user has to follow the steps given below:

### Business Process Flow - Process:

* **Fill in the following details:** Name, Description, Plan Type, Priority Order, Record Type.
* **Priority Order:** Set the execution order against the plan (If the criteria are matching with three different plans, then which plan has to be followed, for that we need to set the priority order number) any value less than 1 or repeated numbers are invalid for this priority order field. ****&#x20;
* **Set criteria for the execution of the Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will attach against those for which the criteria matches). Select either **Simple** or **Advanced**.
  * **Simple:** Execute plans based on the View of an entity.
  * **Advanced:** Execute plans **** based on filter criteria or conditions (conditions defined in Fetch XML).

{% hint style="info" %}
Note: This step is the same for checklist and process - type plans.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/BPF new 2.png" alt=""><figcaption></figcaption></figure>

#### **1)    Simple**&#x20;

Simple criteria can be set on Views of the Record Type.

<figure><img src="../../../../.gitbook/assets/BPF new 3.png" alt=""><figcaption></figcaption></figure>

#### 2) Advanced&#x20;

Plans can be attached based on conditions.&#x20;

For eg. If you want to attach a plan for upcoming leads with lead source as **"Web"** then you have to enter the Fetch XML for it. Below is the Fetch XML for the same.

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

<figure><img src="../../../../.gitbook/assets/BPF new 5 (1).png" alt=""><figcaption></figcaption></figure>

* Select Business Process Flow to which the plan will be attached.

<figure><img src="../../../../.gitbook/assets/BPF new 6.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/BPF new 8 (1).png" alt=""><figcaption></figcaption></figure>

* Navigate to **Manage Steps**.

<figure><img src="../../../../.gitbook/assets/BPF steps 1 (1) (2).png" alt=""><figcaption></figcaption></figure>

* Here, as per the Business Process Flow selected by the manager, various stages of the selected Business Process Flow will be displayed. The manager now selects the desired stages and creates the plan step and plan step action inside the stages.&#x20;
* **For example:** Here we have selected the Business process flow of the **Lead to Opportunity Sales Process** and the stages are Qualify, Develop, Propose, and Close of the **Lead to Opportunity Sales Process** which **** will **** automatically be displayed as shown below. &#x20;
* Now, select the required BPF stage, for example, select the **Qualify** stage.
* Click on the **'Create Plan Step'** Button.

<figure><img src="../../../../.gitbook/assets/BPF steps 1 (1).png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create Form: Plan Step’,** where we need to fill in the details**.**
  * **Name:** Provide an appropriate name to the Plan Step.
  * **Description:** Provide a short description of the Plan Step.
  * **Add a waiting period for this step:**
    * **Days:** Add the desired waiting period for this step to be performed after **'X'** **Days**.
    * **Hours:** Add the desired waiting period for this step to be performed after **'X'** **Hours.**

<figure><img src="../../../../.gitbook/assets/BPF step 3 (1) (1).png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/BPF step 3.png" alt=""><figcaption></figcaption></figure>

* Your plan step will be added to the process and will appear here.

<figure><img src="../../../../.gitbook/assets/BPF step 4 (1).png" alt=""><figcaption></figcaption></figure>

* And now you can add the actions inside the selected stage.&#x20;
* To create Plan Step Actions [click here](https://docs.inogic.com/business-process-checklist/configuration/configuration-for-plans-process/plan-step-action).

### Business Process Flow - Checklist:

* **Fill in the following details:** Name, Description, Plan Type, Priority Order, Record Type.
* **Priority Order:** Set the execution order against the plan (If the criteria are matching with three different plans, then which plan has to be followed, for that we need to set the priority order number) any value less than 1 or repeated numbers are invalid for this priority order field.
* **Set criteria for the execution of the Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will attach against those for which the criteria matches). Select either **Simple** or **Advanced**.
  * **Simple:** Execute plans based on the View of an entity.
  * **Advanced:** Execute plans based on filter criteria or conditions (conditions defined in Fetch XML).
* Select **'Business Process Flow'.**

<figure><img src="../../../../.gitbook/assets/BPF new 1.png" alt=""><figcaption></figcaption></figure>

* Select Business Process Flow to which the plan will be attached.

<figure><img src="../../../../.gitbook/assets/BPF new 2 (1).png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/BPF new 3 (1).png" alt=""><figcaption></figcaption></figure>

* Navigate to **Manage Steps**.
* Here, as per the Business Process Flow selected by the manager, various stages of the selected Business Process Flow will be displayed. Manager can now select the desired stages and create the actions inside the stages.&#x20;
* **For example:** Here we have selected the Business process flow of the **Lead to Opportunity Sales Process** and the stages (Qualify, Develop, Propose, and Close) of the **Lead to Opportunity Sales Process** will **** automatically be displayed as shown below. &#x20;

<figure><img src="../../../../.gitbook/assets/MANAGE STEPS.png" alt=""><figcaption></figcaption></figure>

* Now select the required BPF stage for example select the **Qualify stage**.

<figure><img src="../../../../.gitbook/assets/MANAGE STEPS 2.png" alt=""><figcaption></figcaption></figure>

* Click on the **'Create Plan Step'** Button.
* This will open the **‘Quick Create Form: Plan Step’,** where we need to fill in the details**.**
  * **Name:** Provide an appropriate name to the Plan Step.
  * **Description:** Provide a short description of the Plan Step.
* Once the required fields are filled, click on **‘Save and Close’**.
* Your plan step will be added to the process and will appear here.

<figure><img src="../../../../.gitbook/assets/manage steps 4.png" alt=""><figcaption></figcaption></figure>
