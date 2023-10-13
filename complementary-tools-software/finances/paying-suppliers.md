# Bezahlung von Lieferanten mit ABA-Dateien (Australien)

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

Users who operate a shop with multiple suppliers (hub users) often ask us for the quickest way to forward payments that they receive from customers, to their suppliers. For example, you may stock products from 20 producers in your hub shop. After you receive customer orders and payments, you want a quick way to work out how much you need to transfer to each supplier and then quickly make payment.

This page describes a couple of ways that users can pay their suppliers.

## **Working out how much you owe your suppliers**

You can use [Reports ](../../basic-features/reports/)to get a breakdown of the value of goods sold from each supplier. The [Order Cycle Supplier Totals](../../basic-features/reports/#order-cycle-supplier-totals) report gives the total value of goods sold from each supplier. Alternatively you can download the Order Cycle Customer Totals report and create some pivot tables to extract the data you need.

## **Paying suppliers**

Once you have the dollar values that you need to pay to each supplier, the next step is often to enter these amounts into your online banking system, to do a bank transfer to each supplier. This can be time consuming for those with numerous suppliers.

At the moment OFN doesn't have an automated system for calculating what is owed to suppliers and automatically forwarding payments to them.&#x20;

### Paying multiple suppliers quickly with an ABA file

{% hint style="info" %}
Note: The ABA file is an Australian banking file format, so this option is only relevant to Australian users.&#x20;
{% endhint %}

An alternative for Australian users is to create an ABA file. An ABA file is an file type like an excel spreadsheet, which can be uploaded into most Australian bank's online banking systems, as a way to pay multiple people without entering their individual payments manually.

There's a couple of ways to create an ABA file.

**1) Use your accounting package to generate an ABA file**

If you use an accounting package such as MYOB, Quickbooks or Xero, it's likely that the package will have an 'ABA generation' tool. These tools vary, but generally they'll allow you to enter the amounts you wish to pay each supplier, along with their banking details (BSB, account number, name etc) and then the ABA file will be generated. You can then upload this file into your bank and the payments will be made en mass.&#x20;

{% hint style="info" %}
You may need to contact your bank so they can enable the ABA file upload too. It may also depend on the type of bank account you have with them, so check that they offer this first.
{% endhint %}

**2) Use an online ABA file generator**&#x20;

Cemtaxaba is an online ABA file generator which can turn an excel file into an ABA file. There are fees associated with the tool, check their website for details - [https://www.cemtexaba.com/](https://www.cemtexaba.com/)

The process for using this tool is as follows.

1\) Download the CemtexABA template CSV file.&#x20;

2\) Enter details into the correct columns.They ask for the bank details of the payee and the amount you want to transfer.&#x20;

3\) Upload the CSV into the Cemtexaba website. They'll ask you for your bank details (the 'payer' information), and then they'll provide you with an ABA file

4\) Upload the ABA file into your online banking system to do the bulk payment.
