# Service Scheduling

InoLink application runs as a service. The services in InoLink are designed to handle the sync operations between Dynamics 365 CRM and QuickBooks. These services run in the background without interrupting your on-going activities. In this section, we will discuss these services in detail.

![](<../../.gitbook/assets/QB to CRM\_1 - Copy.png>)

Using **Service Scheduling** option you **** can enable the feature to start the services for **QuickBooks** to **Dynamics 365 CRM Data Synchronization.** After clicking on **Service Scheduling,** you will get the below displayed window.

![](<../../.gitbook/assets/QB to CRM\_SS\_1.png>)

After clicking on **Save** button user will get the below message where the user needs to contact us i.e. **Inogic** to start the **QuickBooks** to **Dynamics 365 CRM** services. The services will be started within 2**4 hours** after the request is been placed.

![](<../../.gitbook/assets/QB to CRM\_SS\_2.png>)

In case the user tries to start the services and save them while we processing user’s provision request then they will get the below error message.

![](<../../.gitbook/assets/QB to CRM\_SS\_3.png>)

Inogic will then enable the QuickBooks to Dynamics 365 CRM services and Dynamics 365 CRM to QuickBooks bulk data synchronization service and send the email to intimate the user. User then needs to start the services by navigating back to **Service Scheduling.**

![](<../../.gitbook/assets/QB to CRM\_SS\_4.png>)

### **1)** InoLink High Priority Service&#x20;

This service is used to move **Customers, Products, Transaction history, Current balance, Total balance,** from QuickBooks to Dynamics 365 CRM. You need to follow the below steps to setup the service:

* **Toggle:** Click on the toggle button to switch on/off the service.&#x20;
* **Days:** Indicates on which days your service will run. The service will trigger only on the selected days.&#x20;
* **Time:** Indicates the time when your service will run. The service will trigger from the specified time. If you want your service to run in your business hours i.e. **8 AM to 5 PM**, then select the **Start Time**, and **End Time** accordingly and the service will trigger in your business hours only.&#x20;
* **Poll Interval (In minutes):** Indicates the triggering interval of the service in the specified time i.e. if the poll interval has been set as 30 minutes, then your service will run trigger after **every 30 minutes,** starting from **8 AM till 5 PM.**

![](<../../.gitbook/assets/QB to CRM\_SS\_5.png>)

This service is scheduled to run at an interval of **30 minutes** between **8AM to 5PM** on Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, and Sunday. You can modify the days, time, and interval to your choice. We recommend the users to set the minimum time of **15 minutes.**

### 2) InoLink Low Priority Service

This service will move data like **Aging details (30, 60, 90)** from QuickBooks to Dynamics 365 CRM. You need to follow the below steps to setup the service:

* **Toggle:** Click on the toggle button to switch on/off the service.&#x20;
* **Days:** Indicates on which days your service will run. The service will trigger only on the selected days.&#x20;
* **Poll Interval (In hours):** Indicates the triggering interval of the service in the specified time. Here, the poll interval is set in hours, and the options to choose are **6 hours, 12 hours,** and **24 hours.** If you select **6 hours,** then your service will trigger after every **6 hours** starting from **midnight** on the given day.

![](<../../.gitbook/assets/QB to CRM\_SS\_6.png>)

This service is scheduled to run once a day on Monday, Tuesday, Wednesday, Thursday, Friday, and Saturday. Once again the interval, and days can be modified but we recommend having this set as a once a day update since it will read through all the synced customer and product records and update them all and is usually a long running and resource consuming process.

### 3) InoLink CRM to QuickBooks Services

This service will help you to **move multiple records** that are promoted in bulk from Dynamics 365 CRM to QuickBooks or else it will remain in queued status if this service is disabled. You need to do the following to setup the service:

* **Toggle:** Click on the toggle button to switch on/off the service.&#x20;
* **Days:** Indicates on which days your service will run. The service will trigger only on the selected days.&#x20;
* **Poll Interval (In minutes):** Indicates the triggering interval of the service in the specified time i.e. if the poll interval has been set as 60 minutes, then your service will run after every 60 minutes (1 hour), starting from 12 midnight, till 23:59 PM.

![](<../../.gitbook/assets/QB to CRM\_SS\_7.png>)

This service is scheduled to run at an interval of **60 minutes** on Monday, Tuesday, Wednesday, Thursday, Friday, and Saturday from **12 AM to 23:59 PM**. You can modify the days, time, and interval to your choice. We recommend the users to set the minimum time of **30 minutes.**

Before you start the services, ensure that all the **Preferences** have been set and the **mappings** have been completed for a successful transfer of data between systems.

**Currency Settings:** If you use **Multi-Currency,** ensure that you have created/enabled all the currencies used in both systems.

{% hint style="info" %}
**Note: During Sync, the program tries to match all fields using their text value so ensure that both systems use the same labels for Picklists and lookups.**
{% endhint %}

