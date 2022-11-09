# SSRS Template

This section will guide you through the process of creating **CRM Report Template** for **SSRS Reports**.

* Open **Click2Export App** and then select **Reports.**

![](../../../.gitbook/assets/SSRS\_1.png)

* Select the reports that need to be used for quick export using **Click2Export** then click on **Create Template Record** button from the ribbon.

![](../../../.gitbook/assets/SSRS\_2.png)

* A confirmation dialog box will appear --> Click on **OK.**

![](../../../.gitbook/assets/SSRS\_3.png)

* The **'Create Template Records'** submits a background job to create records. This allows you to continue with your work till all the templates have been created. Once it is done the following message would be displayed the following message. Click on **OK.**

![](../../../.gitbook/assets/SSRS\_4.png)

* You can check the report templates created in the **CRM Report Templates Area** added in **Click2Export App --> CRM Report Templates.**

![](../../../.gitbook/assets/SSRS\_5.png)

* All the details in the template would be pre-populated based off the template selected at the time of CRM Report Template creation.

### General:

<figure><img src="../../../.gitbook/assets/29.1 (1).png" alt=""><figcaption></figcaption></figure>

**Template Type:** Report Template. This cannot be changed for SSRS Report Template.

**Template Name:** By default, this is set to the corresponding report name but is customizable and can be changed. This name is displayed for Report selection in the Click2Export Window. Hence, it should be unique and easy to identify with, especially when you have multiple templates for the same report.

**Default File Format:** **PDF, Excel, Word, CSV and TIFF** are the options. By default, with the solution it is set as **PDF**. With this option you can decide the default format in which the report would be exported.

**Export File Name:** This is the name that would be provided to the file generated upon export. You could provide a static name or dynamic name (based on a field of the record).

**For e.g. Template Name – {customerid} – {today}**

It will create a file name as: **Sample Click2Export Quote Report - Wayne Industries - Friday, 26 March 2021**

You can use any field name including custom field from the record type provided & today, to get today’s date.

**DateTime Field Format:** This field decides in what format Date & Time should be represented while exporting the report if Export File Name contains a DateTime field. It should have a valid DateTime format for e.g. - **mm/dd/yyyy for 03/23/2021**, **mm/dd/yyyy h:mm tt for 03/23/2021 5:50 AM**. It will reflect the Date & Time field format as Logged-In user’s settings if this field is left blank.

**Auto Send Email:** If enabled, it sends email automatically with the attached exported file, while performing the action from **Click2Export UI** or else it’ll open up the **Email Window** with all the necessary details populated and then you can hit send manually.

**Default Email Template:** The email would be created based on the default email template specified in that section. If left blank, the Email body would be empty.

**Default Filter:** It contains the default fetch XML of template.

### Email Configuration:

The next section is **'Email Configuration'.** To know more about this section, please click [here](https://docs.inogic.com/click2export/configuration/email-configuration).&#x20;

![](<../../../.gitbook/assets/Advance Email Config\_Report.png>)

### CRM Report Parameters:

This will list down all the parameters that needs to be supplied for the report to render.
