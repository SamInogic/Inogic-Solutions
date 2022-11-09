# Custom Plan

With this feature, you can create both **Process** and **Checklist-type** plans against **Custom Flows** to do the same user has to follow the simple steps given below:

### **Custom Plan-Process:**

* Enable entity configuration for this situation select  **‘Lead’** entity.&#x20;

<figure><img src="../../../../.gitbook/assets/1 (79).png" alt=""><figcaption></figcaption></figure>

* Navigate to **BPC Settings** **--> Plans --> New Plan.**

<figure><img src="../../../../.gitbook/assets/Custom process_2.png" alt=""><figcaption></figcaption></figure>

* Click on Create **New plan** button and select **Process.**

<figure><img src="../../../../.gitbook/assets/Custom process_3 (1).png" alt=""><figcaption></figcaption></figure>

* This will open the **'New Plan'** page. Here, you can fill in the details and set the conditions for Plan-Process based on which plan will be executed.

<figure><img src="../../../../.gitbook/assets/Custom process_5.png" alt=""><figcaption></figcaption></figure>

* Fill in the following fields:&#x20;
* **Name:** Give an appropriate name to the plan.
* **Description:** Give a short description of the plan.
* **Plan detail settings:** set the priority order and select the plan type.
  * **Plan Type:** Select Plan Type **** as **Process**.
  * **Priority Order:** Set the execution order against the plan (If the criteria is matching with three different plans, then which plan has to be followed, for that we need to set the priority order number) Any value less than 1 or repeated numbers are invalid for this priority order field. ****&#x20;
* **Record Type:** Select the **Record Type** to which the plan will be attached, here we are selecting the '**Lead' entity**.
* This will set the fields with values as shown below:

<figure><img src="../../../../.gitbook/assets/Custom process_6.png" alt=""><figcaption></figcaption></figure>

* **Set criteria for the execution of Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will run against those for which the criteria matches.) Select either **Simple** or **Advanced**.
  * **Simple: Execute plans** based on the View of an entity.
  * **Advanced: Execute Plans** based on filter criteria or conditions (conditions defined in Fetch XML).

<figure><img src="../../../../.gitbook/assets/Custom process_7.png" alt=""><figcaption></figcaption></figure>

* Select **'Custom Groups'.**

<figure><img src="../../../../.gitbook/assets/Custom process_8.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/Custom process_9.png" alt=""><figcaption></figcaption></figure>

* Click on **'New Plan'.**

<figure><img src="../../../../.gitbook/assets/Custom process_10.png" alt=""><figcaption></figcaption></figure>

* Fill in the Plan Details and Click **'Save'**:
  * **Name:** Give an appropriate name to the plan.
  * **Description:** Give a short description of the plan.
  * **Priority Order:** Set the execution order against the plan.

<figure><img src="../../../../.gitbook/assets/Custom process_11.png" alt=""><figcaption></figcaption></figure>

* Navigate to **Plan Details** **-->** **Manage Steps**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_1.png" alt=""><figcaption></figcaption></figure>

* Click on the **New Plan Step** button.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_2.png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create: Plan Step’** form. Here, you can fill in the details and add a waiting period for this plan step to execute**.**
  * **Name:** Give an appropriate name to the Plan Step.
  * **Description:** Give a short description of the Plan Step.
  * **Add waiting period for this step:**
    * **Days:** Add the desired waiting period for this step to be performed in **Days**.
    * **Hours:** Add the desired waiting period for this step to be performed in **Hours.**

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_3.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_4.png" alt=""><figcaption></figcaption></figure>

* Your plan step will be added to the plan and will appear here.

<figure><img src="../../../../.gitbook/assets/Custom process PLAN STEP_5.png" alt=""><figcaption></figcaption></figure>

* Click on **ellipses (the three small dots) --> '+ Create Action'** to Add an action.

<figure><img src="../../../../.gitbook/assets/Custom process plan step action_1.png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create: Plan Step Action’** form. Here, you can fill in the details and set the criteria for the execution of plan step actions.
  * **Title:** Your plan step action title is the same as your plan step name but you can modify the Plan Step Action title as you feel appropriate.&#x20;
  * **Description:** Give a short description of the plan step action
  * **Action Display Name:** Choose a display name for the action from the dropdown.
  * **Action Logical Name:** Choose a logical name for the action from the dropdown.
  * **Select the Email template:** you will see this option for the records that support email activity and have an email field present on the entity form.
    * **Auto Send Email:** Select **Yes** or **No** to send or not send email automatically.
    * **Email Template:** If you want to send an email select an appropriate Email Template from the drop-down.
  * **Set criteria for the execution of Plan Step Action:**
    * **Execution Order:** Enter the execution order number of the Plan Step Action, in which execution order the Plan Step Action should be Executed.
    * **Criteria Mode:** Defines the criteria of the records on which the Plan Step Action will be applicable and executed. Select either Simple or Advanced.
      * **Simple:** Here you can select any ‘View’ from the dropdown.
      * **Advanced:** Here, you can further define and set criteria for records through fetch XML.

<figure><img src="../../../../.gitbook/assets/Custom process plan step action_2 (2).png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save and Close’**.

<figure><img src="../../../../.gitbook/assets/Custom process plan step action_3.png" alt=""><figcaption></figcaption></figure>

* Your Plan Step Action will be added to the plan step and will appear here.

<figure><img src="../../../../.gitbook/assets/Custom process plan step action_4.png" alt=""><figcaption></figcaption></figure>

### **Custom Plan-Checklist:**

* Enable entity configuration for this situation select the **‘Lead’** entity.&#x20;

<figure><img src="../../../../.gitbook/assets/custom checklist plan_1.png" alt=""><figcaption></figcaption></figure>

* Navigate to **BPC Settings** **--> Plans --> New Plan.**

<figure><img src="../../../../.gitbook/assets/custom checklist plan_2.png" alt=""><figcaption></figcaption></figure>

* Click on Create **New plan** button and select **Checklist.**

<figure><img src="../../../../.gitbook/assets/custom checklist plan_3.png" alt=""><figcaption></figcaption></figure>

* This will open the **'New Plan'** page. Here, you can fill in the details and set the conditions for Plan-Checklist based on which plan will be executed.

<figure><img src="../../../../.gitbook/assets/custom checklist plan_4.png" alt=""><figcaption></figcaption></figure>

* Fill in the following fields:&#x20;
* **Name:** Give an appropriate name to the plan.
* **Description:** Give a short description of the plan.
* **Plan detail settings:** set the priority order and select the plan type.
  * **Plan Type:** Select Plan Type **** as **Checklist**.
  * **Priority Order:** Set the execution order against the plan (If the criteria is matching with three different plans, then which plan has to be followed, for that we need to set the priority order number) Any value less than 1 or repeated numbers are invalid for this priority order field. ****&#x20;
* **Record Type:** Select the **Record Type** to which the plan will be attached, here we are selecting the '**Lead' entity**.
* This will set the fields with values as shown below:

<figure><img src="../../../../.gitbook/assets/custom checklist plan_5.png" alt=""><figcaption></figcaption></figure>

* **Set criteria for the execution of Plan:** Set the criteria against the plan (so that if the criteria satisfy then the plan will run against those for which the criteria matches.) Select either **Simple** or **Advanced**.
  * **Simple: Execute plans** based on the View of an entity.
  * **Advanced: Execute Plans** based on filter criteria or conditions (conditions defined in Fetch XML).

<figure><img src="../../../../.gitbook/assets/custom checklist plan_6.png" alt=""><figcaption></figcaption></figure>

* Select **'Custom Groups'.**

<figure><img src="../../../../.gitbook/assets/custom checklist plan_7.png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save’**.

<figure><img src="../../../../.gitbook/assets/custom checklist plan_8.png" alt=""><figcaption></figcaption></figure>

* Click on **'New Plan'.**

<figure><img src="../../../../.gitbook/assets/custom checklist plan_9.png" alt=""><figcaption></figcaption></figure>

* Fill in the Plan Details and Click **'Save'**:
  * **Name:** Give an appropriate name to the plan.
  * **Description:** Give a short description of the plan.
  * **Priority Order:** Set the execution order against the plan.

<figure><img src="../../../../.gitbook/assets/custom checklist plan_10.png" alt=""><figcaption></figcaption></figure>

* Navigate to **Plan Details** **-->** **Manage Steps**.

<figure><img src="../../../../.gitbook/assets/custom checklist plan step_1.png" alt=""><figcaption></figcaption></figure>

* Click on the **New Plan Step** button.

<figure><img src="../../../../.gitbook/assets/custom checklist plan step_2.png" alt=""><figcaption></figcaption></figure>

* This will open the **‘Quick Create: Plan Step’** form. Here, you can fill in the details and add a waiting period for this plan step to execute**.**
* **Name:** Give an appropriate name to the Plan Step.
* **Description:** Give a short description of the Plan Step.
* **Add waiting period for this step:**
  * **Days:** Add the desired waiting period for this step to be performed in **Days**.
  * **Hours:** Add the desired waiting period for this step to be performed in **Hours.**

<figure><img src="../../../../.gitbook/assets/custom checklist plan step_3 (1).png" alt=""><figcaption></figcaption></figure>

* Once the required fields are filled, click on **‘Save and Close’**

<figure><img src="../../../../.gitbook/assets/custom checklist plan step_4.png" alt=""><figcaption></figcaption></figure>

* Your plan step will be added to the plan and will appear here.

<figure><img src="../../../../.gitbook/assets/custom checklist plan step_5.png" alt=""><figcaption></figcaption></figure>

****

****
