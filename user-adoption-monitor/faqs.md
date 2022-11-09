# FAQs

## 1) Last Touch Date vs Last Processed Date vs Enable Tracking Date

**Last Touch Date:** This date tells when the user was last active in CRM with any specific activity i.e. created/updated account/contact etc. User Adoption Monitor tracks the last CRM touch of the user and shows it as a 'Last Touch Date'.

**Last Processed Date:** There is a process involved in the **'systemuser-login'** entity configuration, that runs in the background depending on the polling interval defined for the **'systemuser-login'** entity configuration. For example, if the **'Preferred Start Time'** and **'Polling'** are defined as below –

![](<../.gitbook/assets/FAQ\_2 (2).png>)

Then, the process will first run at 18:18 and it will continue triggering at the interval of every 4 hours as the polling is set to **'Every 4 Hours'** as seen in the above image. Each time the process triggers, it checks for the CRM access of the respective users within that period of time (polling) and track the same.

**Enable Tracking Date:** This is the date when **'systemuser-login'** entity configuration was enabled/created.

## 2) How to send the Daily, Weekly & Monthly tracking reports automatically?

User can send the tracking data/information through excel sheet or SSRS reports provided the user has an excel template or SSRS report respectively in the system with an availability of the process to send them automatically. Moreover, we would request you to have a look at another ISV solution of ours named 'Click2Export' which actually gives you an ability to send such reports automatically. Therefore, Click2Export and User Adoption Monitor are together being used by some of our customers across the world to be able to perform such operations.

## 3) What if you see all the processes of 'User Adoption Monitor' in 'Draft/Deactivated' state after importing the User Adoption Monitor solution from the website?

Once the solution is imported, please follow the below steps to activate all the processes of User Adoption Monitor.

* Navigate to **Advanced Settings --> Settings --> Process Center --> Processes.**

![](../.gitbook/assets/FAQ\_3.1.png)

![](../.gitbook/assets/FAQ\_3.2.png)

* Under **'All Processes'** view, activate the processes as shown below:

![](../.gitbook/assets/FAQ\_3.3.png)

![](../.gitbook/assets/FAQ\_3.4.png)

## 4) Does User Adoption Monitor automatically log a user logging into CRM? Or must a user manually click the 'Log in' button to track that?

It does not automatically track the login/logout activity into CRM. You need to make sure to manually click on Login/Logout button in order for User Adoption Monitor tool to create and track the respective login/logout activity counts.&#x20;

## 5) Is there a way to see true user who created the Dashboard records?&#x20;

Follow below mentioned steps to be able to see the actual user (of record) that has performed an action.

While drilling down, select 'User' field from the list.

![](../.gitbook/assets/FAQ\_5.1.jpg)

Select the type of chart that you would like to view the data in.

![](../.gitbook/assets/FAQ\_5.2.jpg)

This will show you user-wise respective trackings.

![](../.gitbook/assets/FAQ\_5.3.jpg)

## 6) Is there a way to NOT track the usage by a specific CRM user?

Using 'Monitored Users' feature of User Adoption Monitor, you can restrict the tracking for selected user for a specific entity action however, if you want to completely restrict the tracking for any specific user irrespective of the entity action, you need to turn the User Adoption Monitor **Off** on the respective user record. You can follow the below steps for this –

* Navigate to **Advanced settings --> Settings --> Security --> Users --> Select the user.**

![](../.gitbook/assets/FAQ\_6.1.jpg)

![](../.gitbook/assets/FAQ\_6.2.jpg)

![](../.gitbook/assets/FAQ\_6.3.jpg)

* Select the user whom you don’t want to track anymore**.**

![](../.gitbook/assets/FAQ\_6.4.jpg)

* Disable the user adoption as shown below (Set it to 'No'). **** This will stop the tracking for the selected user.

![](../.gitbook/assets/FAQ\_6.5.jpg)

## 7) We have done a sandbox copy of the production environment to a TEST environment and would like to work with 'User Adoption Monitor' solution in this new instance. What should we do?

For this, you need to delete the **Inogic License Details** record from your sandbox environment. After deleting, the next step would be to [activate the license](https://docs.inogic.com/user-adoption-monitor/getting-started/license-activation).

To delete the **User Adoption Monitor** license follow the steps given below:

* Navigate to **Advanced Find.**

![](<../.gitbook/assets/FAQ\_1 (4).png>)

* Select **Inogic License Details** in **‘Look for’** --> Click on **Results** button.

![](<../.gitbook/assets/FAQ\_2 (4).png>)

* Select the **User Adoption Monitor** record and **delete** it.

![](<../.gitbook/assets/FAQ 7\_1.png>)
