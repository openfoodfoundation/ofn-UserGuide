---
description: Payment Reports, Tax reports, Xero
---

# Payment and Tax Reports

## Payment Reports

{% hint style="success" %}
The three Payment reports are good for keeping track of total incoming and outgoing revenue for your food hub within a time frame.
{% endhint %}

### Payment by Type

The simplest payment report. This documents the total of paid, balance due and credit owing for each different type of payment a hub may employ (ie. a total for Stripe payments, a total for cash/EFT payments and one for PayPal).

![Payment by Type](../../.gitbook/assets/payment-by-type.jpg)

### Itemised Payment Totals

Listed by payment status (paid, balance due, credit owing) rather than payment provider, this report gives a breakdown of revenue (product costs, shipping fees) as well as the total.  The Outstanding balance column will be 0.0 for the payment status of 'paid'

![Itemised Payment Totals](../../.gitbook/assets/itemizedpayment.jpg)

### Payment Totals

In addition to the Itemised Payment Totals this report states revenue coming from EFT (cash or bank transfer) and Paypal separately.

![Payment Totals](../../.gitbook/assets/payment-totals.jpg)

## Sales Tax

There are two sales tax reports: Tax Types and Tax Rates.

{% hint style="success" %}
The **Tax Type** report is useful for separating total tax per order into its different component elements: tax on products, tax on shipping method fee and tax on fees- enterprise and/or payment method fees.
{% endhint %}

![Tax type report](<../../.gitbook/assets/tax types report.jpg>)

The **tax rate** report gives an **order-by-order break down** of tax by it's tax rate (full, reduced or zero-rated PRODUCTS and tax from delivery fees).  Order totals inclusive and exclusive of tax are also given.

![Tax rate report](<../../.gitbook/assets/tax rates report.jpg>)

## Xero Invoices

This report creates CSV files which can be imported into the accounting package ‘Xero’ to generate invoices for customers.

### Generating the report

![Xero Report Fields](../../.gitbook/assets/xero-report.png)

**Date range:** You can filter orders by the date the order was placed.

**Report type:** You can select to download a ‘detailed’ report, which includes a line item for each item the customer purchased, including any fees and adjustments to their order.

**Hub and order cycle:** You can specify which Hub and Order Cycle, the orders were placed through.

**Initial invoice number:** To ensure compatibility with your Xero invoice numbering system, enter the first invoice number you would like new invoices to be allocated. All subsequent invoices will be numbered from this point.

**Invoice date:** You can select the date that you want the invoices to be marked with in Xero. This is editable once you have the invoice in Xero, but doing it here allows you to batch date all the invoices in a single report.&#x20;

**Due date:** You can select the due date to be marked on Xero invoices. Again this is editable in Xero.

**Account code:** If you place a Xero account code here, all items in the invoice will be assigned to this account. This it editable in Xero.

**Download as CSV:** When you are ready to download the file for import check the box and click **search**.

### Data Available

* Customer name, email, billing address (no phone number)
* Invoice number and date of purchase. Due date is one month after invoice date.  Reference number is the same as invoice number.
* Product name, quantity, cost, tax rate, SKU, fee
* Payment status (paid or balance due)
* currency of transaction.

### Importing the report into Xero

In Xero go to **Accounts**, **Sales** and click Import.

![Xero Import](../../.gitbook/assets/xero-import.png)

Next you will select your downloaded OFN Xero report for upload. The settings you should select are shown below.

![Xero Import Steps](../../.gitbook/assets/xero-import-steps.png)

Selecting **Ignore contact address detail**s will ensure your Xero customer data is unaltered.&#x20;

Selecting **Tax Exclusive** will ensure that products you have set to include tax in the Open Food Network will include tax, but your tax free items will remain tax free.
