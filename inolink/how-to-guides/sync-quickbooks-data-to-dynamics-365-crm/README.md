# Sync QuickBooks data to Dynamics 365 CRM

You need to make sure the **InoLink High Priority** service is set in Service Scheduling section within the QuickBooks to Dynamics CRM feature option.

![](<../../../.gitbook/assets/QB to CRM\_1 (1).png>)

This service is scheduled to poll at every 30 minutes interval from 8AM to 5PM. It would look for records modified since the last time it synced from QuickBooks to CRM and update such records in Dynamics 365 CRM.

You can modify the poll interval to an interval of your choice. However, it is advised to keep the poll interval in comparison with the volume of transactions during the interval. It is advised to not reduce the interval to less than 30 minutes if there is moderate transaction sync between the systems.

Successful update would result in a new Link Job created in Dynamics 365 CRM with the **'Success'** status and the Source would be set to **'Accounting'** to denote a successful completion of the sync job triggered from QuickBooks. In case of an error, the status of the Link Job is set to **'Error'.**

![](<../../../.gitbook/assets/QB to CRM\_2 (1).png>)
