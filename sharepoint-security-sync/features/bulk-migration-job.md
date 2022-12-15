# Bulk Migration Job

**Bulk Migration Job** Entity enables users to configure the bulk movement of the attachments from CRM to SharePoint and also it shows the details and status of the migrating **Emails, Notes and Sales Literature Attachments.**

{% hint style="info" %}
**Note:**&#x20;

* **Users are advised to do the migration during off business hours for minimum interruption as there may be bulk of data to be moved.**
* **Only the Entities where the Attachment Action is defined as Move or Copy in the Entity Configuration will be considered for Bulk Migration.**
{% endhint %}

To configure **Bulk Migration Job**, go to **SharePoint Security Sync App --> Bulk Migration Jobs --> Click on '+New' --> Fill the respective fields.**

### **General:**

This section is where you define the period and Email/Note/Sales Literature attachment we are moving to SharePoint.

<figure><img src="../../.gitbook/assets/Bulk migration slide 34.png" alt=""><figcaption></figcaption></figure>

* **For?:** This specifies whether we are doing Bulk Migration for Emails, Notes or Sales Literature.&#x20;
* **Connector:** In this field we specify the connector support i.e. SharePoint.&#x20;
* **Schedule Date:** Scheduled date keeps track of the date from which the migration job will start.
* **Attachment Action:** In this field we specify the action i**.**e. Copy or Move.
* **Select Duration Criteria:** In this field we specify the period for which we have to migrate Note/Email Attachment/Sales Literature Attachments to SharePoint. Here, X represents  Numeric Value. For e.g. Last 10 days, Last 3 weeks, etc. where the number 10 and 3 specify the Value.&#x20;
  * **Last X Days:** Specify data of how many(X) days have to be migrated to SharePoint.
  * **Last X Weeks:** Specify data of how many(X) weeks have to migrate to SharePoint.
  * **Last X Months:** Specifies data of how many(X) months have to be migrated to SharePoint.
  * **Last X Years:** Specifies data of how many(X) years has to be migrated to SharePoint.
  * **Older Than:** This moves all the Notes/Email attachments prior and inclusive of the date SharePoint.
  * **Custom:** This specifies the period Process From date to Process Till date between which the data is to be moved to SharePoint.

{% hint style="info" %}
**Note: The Notes and Sales Literature Attachments will be moved to their corresponding record folder and Email attachments will move to a common folder named Email Attachment or Regarding Folder.**
{% endhint %}

### Information:

The next tab is Information that comprises the details of processed records.

<figure><img src="../../.gitbook/assets/Bulk migration slide 34 image 2.png" alt=""><figcaption></figcaption></figure>

* **Total Records Processed:** Total number of Emails/Notes/Sales Literature attachment that are processed.
* **Total Succeeded Records:** Total number of records that have successfully migrated to SharePoint.
* **Total Ignored Records:** Number of records that were ignored.
* **Total Failed Records:** Total number of records that failed in the process of migration.
* **Total Succeeded Size (KB):** The size of records that were moved to SharePoint. This tells the Dynamics 365 CRM user how much space he has freed from the CRM.
* **Total Ignored Size (KB):** This is the size of files that were ignored while migrating to SharePoint.
* **Total Failed Size (KB):** Size of failed files while uploading to SharePoint.

{% hint style="success" %}
For further queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}





