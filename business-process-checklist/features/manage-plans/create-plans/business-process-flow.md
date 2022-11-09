# Business Process Flow

With this feature, you can create both **Process** and **Checklist-type** plans against **Business Process Flow.**

For example, if a user wants to create a plan against the **Lead to Opportunity Sales process** to set the best practices for **Lead Nurturing**. **** In order to achieve this, the user has to follow the steps given below:

### Business Process Flow - Process:

* **Fill in the following details:** Name, Description, Plan Type, Priority Order, Record Type.

<figure><img src="../../../../.gitbook/assets/BPF_5 (1).png" alt=""><figcaption></figcaption></figure>

* **Set criteria for the execution of the Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will run against those for which the criteria matches.) Select either **Simple** or **Advanced**.
  * **Simple:** Execute plans based on the View of an entity.
  * **Advanced:** Execute Plans **** based on filter criteria or conditions (conditions defined in Fetch XML).

{% hint style="info" %}
Note: This step is the same for checklist and process-type plans.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/BPF_6 (1).png" alt=""><figcaption></figcaption></figure>

#### **1)    Simple**&#x20;

Simple criteria can be set on System Views of the Record Type.

<figure><img src="../../../../.gitbook/assets/BPF_7 (1).png" alt=""><figcaption></figcaption></figure>

#### 2) Advance&#x20;

Plans can be attached based on conditions.&#x20;

For eg. If you want to attach a plan to open leads with lead source as web then you have to enter the Fetch XML for it. Below is the Fetch XML for the open lead where the lead source is the web.

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

In the same way, you can set Advance criteria for other plan records as well.

<figure><img src="../../../../.gitbook/assets/Bpf_8.png" alt=""><figcaption></figcaption></figure>

* Select **'Business Process'.**

<figure><img src="../../../../.gitbook/assets/Bpf_9.png" alt=""><figcaption></figcaption></figure>

* Select Business Process Flow to which the plan will be attached.

<figure><img src="../../../../.gitbook/assets/BPF_10.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/BPF_11 (1).png" alt=""><figcaption></figcaption></figure>

* Click on **'New Plan'.**

<figure><img src="../../../../.gitbook/assets/BPF_12.png" alt=""><figcaption></figcaption></figure>

* Fill in the Plan Details and Click **'Save'**:

<figure><img src="../../../../.gitbook/assets/BPF_13.png" alt=""><figcaption></figcaption></figure>

* To create Plan Step Actions [click here](https://docs.inogic.com/business-process-checklist/configuration/configuration-for-plans-process/plan-step-action).

### Business Process Flow - Checklist:

* Enable entity configuration for this situation select the **‘Lead’** entity.&#x20;

<figure><img src="../../../../.gitbook/assets/BPF_1 (1).png" alt=""><figcaption></figcaption></figure>

* Navigate to **BPC Settings** **--> Plans --> New Plan.**

<figure><img src="../../../../.gitbook/assets/BPF_2 (3).png" alt=""><figcaption></figcaption></figure>

* Click on Create **New plan** button and select **Checklist.**

<figure><img src="../../../../.gitbook/assets/BPF_2 (2).png" alt=""><figcaption></figcaption></figure>

* This will open the **'New Plan'** page. Here, you can fill in the details and set the conditions for Plan-Checklist based on which plan will be executed.

<figure><img src="../../../../.gitbook/assets/BPF_4 (1).png" alt=""><figcaption></figcaption></figure>

* Fill in the following fields:&#x20;
* **Name:** Give an appropriate name to the plan.
* **Description:** Give a short description of the plan.
* **Plan detail settings:** set the priority order and select the plan type.
  * **Plan Type:** Select Plan Type **** as **Checklist**.
  * **Priority Order:** Set the execution order against the plan (If the criteria is matching with three different plans, then which plan has to be followed, for that we need to set the priority order number) Any value less than 1 or repeated numbers are invalid for this priority order field. ****&#x20;
* **Record Type:** Select the **Record Type** to which the plan will be attached, here we are selecting the '**Lead' entity**.
* This will set the fields with values as shown below:

<figure><img src="../../../../.gitbook/assets/BPF_5 (3).png" alt=""><figcaption></figcaption></figure>

**Set criteria for the execution of Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will run against those for which the criteria matches.) Select either **Simple** or **Advanced**.

* **Simple: Execute plans** based on the View of an entity.
* **Advanced: Execute Plans** based on filter criteria or conditions (conditions defined in Fetch XML).

<figure><img src="../../../../.gitbook/assets/BPF_6.png" alt=""><figcaption></figcaption></figure>

* Select **'Business Process'.**

<figure><img src="../../../../.gitbook/assets/BPF_7 (3).png" alt=""><figcaption></figcaption></figure>

* Select Business Process Flow to which the plan will be attached.

<figure><img src="../../../../.gitbook/assets/BPF_8.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/BPF_9.png" alt=""><figcaption></figcaption></figure>

* Click on **'New Plan'.**

<figure><img src="../../../../.gitbook/assets/BPF_10 (1).png" alt=""><figcaption></figcaption></figure>

* Fill in the Plan Details and Click **'Save'**:
  * **Name:** Give an appropriate name to the plan.
  * **Description:** Give a short description of the plan.

<figure><img src="../../../../.gitbook/assets/BPF_11.png" alt=""><figcaption></figcaption></figure>

* To know how to create Plan Steps please[ click here](https://docs.inogic.com/business-process-checklist/configuration/configuration-for-plans-checklist/plan-step).
