# Anonymous Link Settings

### How to create Anonymous Link

[Attach2Dynamics](https://www.inogic.com/product/productivity-pack/attach-2-dynamics-365-crm-upload-multiple-files-sharepoint-cloud-storage) integrates cloud storages like Dropbox, Azure Blob and SharePoint seamlessly within Dynamics 365 to allow easy access to files related to CRM records including drag and drop multiple files and folders feature. Files stored on these cloud storages with Attach2Dynamics can be accessed by creating anonymous shareable link.

During one of our implementation we came across a problem where users were not able to create anonymous shareable link of files on SharePoint with Attach2Dynamics in Dynamics 365 CRM. So, lets get some tips on how to resolve that.

![](<../../.gitbook/assets/Anonymous Link\_image 1.png>)

While creating an anonymous link of file on Attach2Dynamics UI in Dynamics 365 CRM as shown in the above screenshot, you may receive the following error, which may be due to insufficient permissions on SharePoint.

![](<../../.gitbook/assets/Anonymous Link\_image 2.png>)

**Solution –** To successfully create anonymous links of files on SharePoint please follow the below steps:

**1**. Sign in to [https://admin.microsoft.com](https://admin.microsoft.com/) as a global or SharePoint admin. If you see a message that **You don’t have permission to access the page**, then you don’t have Office 365 administrator permissions in your organization.

![](<../../.gitbook/assets/image (69).png>)

&#x20;**2**. In the left pane, below admin centers select SharePoint.

![](<../../.gitbook/assets/image (55).png>)

&#x20;**3**. Now, in the left pane of the new SharePoint admin center, under **Sites** select **Active sites**. (If the classic SharePoint admin center comes then select try it now to open new SharePoint admin center).

![](<../../.gitbook/assets/image (111).png>)

&#x20;**4**. Select site and then select **Sharing**.

![](<../../.gitbook/assets/image (72).png>)

&#x20;**5**. Select **Anyone** and then save it. Now, you can create anonymous shareable link of files.

![](<../../.gitbook/assets/image (68).png>)

&#x20;**6**. Now go to Attach2Dynamics pop-up and try to create an anonymous link.

![](<../../.gitbook/assets/Anonymous Link\_image 3.png>)

Anonymous shareable link is created!!

By enabling rights for a particular site you can enable creating anonymous shareable link for that site.

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
