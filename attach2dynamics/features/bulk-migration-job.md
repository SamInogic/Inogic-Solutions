# Bulk Migration Job

Bulk Migration Job Entity enables users to configure the bulk movement of the attachments **(Notes/Emails & Sales Literature)** from CRM to the configured cloud storage and also it shows the details and status of the migrating Emails, Notes and Sales Literature Attachments.

{% hint style="info" %}
**Note:**

* **Users are advised to do the migration during off business hours for minimum interruption as there may be bulk of data to be moved.**
* **Only the Entities where the Attachment Action is defined as Move or Copy in the Entity Configuration will be considered for Bulk Migration.**
{% endhint %}

You will have to fill the following details while configuring **Bulk Migration Job.**

### **General:**

In this section you will define the period and **Email/Note/Sales Literature** attachment that you are moving to cloud storage.

<figure><img src="../../.gitbook/assets/Bulk Migration- slide 22.png" alt=""><figcaption></figcaption></figure>

1. **For ?:** This specifies whether we are doing Bulk Migration for Emails, Notes or Sales Literature.&#x20;
2. **Connector:** In this field we specify the connector support i.e. SharePoint, Dropbox or Azure Blob Storage.&#x20;
3. **Schedule Date:** Scheduled date keeps track of the date from which the migration job will start.
4. **Attachment Action:** In this field we specify the action ie. Copy or Move.
5.  **Operator:** In this field we specify the period for which we have to migrate Note/Email Attachment/Sales Literature Attachments to cloud storage. Here, X repesents  Numeric Value. For e.g. Last 10 days, Last 3 weeks, etc. where the number 10 and 3 specifies the Value.&#x20;

    **a)    Last X Days:** Specify data of how many(X) days has to be migrated to cloud storage.

    **b)    Last X Weeks:** Specify data of how many(X) weeks has to migrated to cloud storage.

    **c)    Last X Months:** Specifies data of how many(X) months has to be migrated to cloud storage.

    **d)    Last X Years:** Specifies data of how many(X) years has to be migrated to cloud storage.

    **e)    Older Than:** This moves all the Notes/Email attachments prior and inclusive of the date to cloud storage. &#x20;

    **f)    Custom:** This specifies the period **Process From** date to **Process Till** date between which the data is to be moved to cloud storage.

{% hint style="info" %}
**Note: The Notes and Sales Literature Attachments will be moved to their corresponding record folder and Email attachments will move to a common folder named Email Attachment or Regarding Folder.**
{% endhint %}

### Information:

This tab comprises the details of processed records.

<figure><img src="../../.gitbook/assets/Bulk Migration- slide 22 image 2.png" alt=""><figcaption></figcaption></figure>

1. **Total Records Processed:** Total number of Emails/Notes/Sales Literatures that are processed.&#x20;
2. **Total Succeeded Records:** Total number of records that have successfully migrated to cloud storage.
3. **Total Ignored Records:** Number of records that were ignored.&#x20;
4. **Total Failed Records:** Total number of records that failed in the process of migration.&#x20;
5. **Total Succeeded Size (KB):** The size of records that were moved to cloud storage. This tells the Dynamics 365 CRM user how much space he has freed from the CRM.&#x20;
6. **Total Ignored Size (KB):** This is the size of files that were ignored while migrating to cloud storage.&#x20;
7. **Total Failed Size (KB):** Size of failed files while uploading to cloud storage.

{% hint style="info" %}
**Note: At a time only three jobs can be executed, one for Note, one for Email and one for Sales Literature Attachment. After completion other jobs can be created.**
{% endhint %}
