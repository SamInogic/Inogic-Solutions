# Rule-Based Alert

Rule-Based Alerts are designed for specific conditions. There are two types of Rule-Based Alerts:

#### 1) Simple Alerts

Simple alerts are rule-based alerts created based on System Views related to the entity whose Entity Configuration has been selected.&#x20;

![](<../../.gitbook/assets/Rule based\_2.png>)

To know how to create Rule-Based Simple Alerts, please [click here.](https://docs.inogic.com/alerts4dynamics/configuration/record-based-alert/rule-based-alert#1-simple-alerts)

#### 2) Advanced Alerts

Alerts can be created based on conditions.&#x20;

For eg. If you want to create alerts for all the Invoices whose Total Amount is greater than or equal to 1000 then you have to enter the Fetch XML for it. Below is the Fetch XML for Total Amount in Invoices greater than or equal to 1000.

```
<fetch version="1.0" output-format="xml-platform" mapping="logical" distinct="false">
  <entity name="invoice">
    <attribute name="name" />
    <attribute name="customerid" />
    <attribute name="statuscode" />
    <attribute name="totalamount" />
    <attribute name="invoiceid" />
    <order attribute="name" descending="false" />
    <filter type="and">
      <condition attribute="totalamount" operator="ge" value="1000" />
    </filter>
  </entity>
</fetch>
```

In the same way, you can create Advanced Alerts for other records also.

![](<../../.gitbook/assets/Rule based\_1.png>)

To know how to create Rule-Based Advanced Alerts, please [click here.](https://docs.inogic.com/alerts4dynamics/configuration/record-based-alert/rule-based-alert#2-advanced-alerts)

{% hint style="success" %}
For any queries, reach out to us at [crm@inogic.com](mailto:crm@inogic.com)
{% endhint %}
