---
description: Tax reports
---

# Tax Reports

## Sales Tax

There are four sales tax reports:&#x20;

* [Tax Types](payment-and-tax-reports-1.md#tax-type-reports)&#x20;
* [Tax Rates](payment-and-tax-reports-1.md#tax-rate-reports)&#x20;
* [Sales Tax Totals by Producer](payment-and-tax-reports-1.md#sales-tax-totals-by-producer)
* [Sales Tax Totals by Order](payment-and-tax-reports-1.md#sales-tax-totals-by-order)

{% hint style="danger" %}
If your enterprise is **Tax Registered** then it is important that the correct 'Tax Zone' is selected when prompted (for example when setting up a [Shipping Method](../shopfront/shipping-methods.md) fee).
{% endhint %}

### Tax Type Reports

The **Tax Type** report is useful for separating total tax per order into its different component elements: tax on products, tax on shipping method fee and tax on fees- enterprise and/or payment method fees.

![Tax type report](<../../.gitbook/assets/tax types.jpg>)

### Tax Rate Reports

The tax rate report gives an **order-by-order break down** of tax by it's tax rate (full, reduced or zero-rated PRODUCTS and tax from delivery fees).  Order totals inclusive and exclusive of tax are also given.

![Tax rate report](<../../.gitbook/assets/tax rates.jpg>)

{% hint style="warning" %}
The exact tax rates for Full, Reduced and Zero, along with the legislation which governs which category a product belongs to, varies from instance to instance.

There are, however, three 'Tax Zones' available on the OFN platform: UK\_VAT, EU\_VAT and North America.  UK and EU tax zones operate in the same manner (prices displayed to customers are inclusive of sales tax); the North America tax zone operates differently (prices displayed to customers are exclusive of sales tax).

As a result there will be more than three possible columns for selection when you download a Tax Rate Report.
{% endhint %}

The above screen shot was taken from a UK enterprise.  The columns shown correspond to (from left to right):

* 5.0% : Reduced rate VAT on products
* 0.0% : Zero rate VAT on products
* 20.0% : Full rate VAT on products
* 20.0% : Full rate VAT on shipping methods from UK to North America
* 20.0% : Full rate VAT on shipping/collection methods within the UK

### &#x20;Sales Tax Totals by Producer

For the time period or order cycle used to filter results, this report gives the tax status of each supplier, and the total revenue they sold for each available tax rate.  (Only tax rates for which they sold produce are shown).

<figure><img src="../../.gitbook/assets/tax by producer.jpg" alt=""><figcaption><p>Sales Tax by Producer Report</p></figcaption></figure>

### Sales Tax Totals by Order

For the time period or order cycle used to filter results, this report gives the contribution of products or services in each tax rate to the overall tax paid by the customer for that order. &#x20;

<figure><img src="../../.gitbook/assets/tax by order.jpg" alt=""><figcaption><p>Sales Tax by Order</p></figcaption></figure>

