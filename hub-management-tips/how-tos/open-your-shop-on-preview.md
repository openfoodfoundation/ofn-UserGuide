# Öffnen Sie Ihren Shop auf 'Vorschau'.

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Introduction

As a hub manager you may often be asked by your suppliers to see what their products look like on your shop front before the order cycle goes 'live' to customers.  Suppliers may wish to tweak their listings- change a photo or add to their product descriptions for example.  This is especially common in the early days (weeks and months) of a new hub.

The process below outlines how to implement a 'Preview' Order Cycle. It draws on the highly flexible feature of Tag and Tag Rules on the OFN platform.

{% hint style="info" %}
Your enterprise will need to be listed as a Hub on the OFN platform to add a tag to order cycles.
{% endhint %}

## Process

{% hint style="warning" %}
This is a **TWO** step process:&#x20;

1. Opening an Order Cycle which only you and suppliers can view.
2. Removing the tag which facilitates (1) when the order cycle goes 'live' to customers.
{% endhint %}

### Step one

* Login to your business OFN account and visit [Customers](https://openfoodnetwork.org.uk/admin/customers) page.
* Click **+ New Customer** and add the email addresses of your suppliers. (If they have placed an order with your shop/hub in the past then they will already be a customer of your enterprise and so this step is not necessary.)
* In the ‘tags’ column type in ‘producer’ for that customer.

![](https://lh3.googleusercontent.com/azVPv6QfS6nyjTC5QnHE3ATsDnrZxYO1bttYGxkAvYH1BItAuYpj1cT73ZYjipftqUH2zWcYP2VU4kgD9l9npPe6wDjfuSteCmJUSwFvauK1mFIEwlDK6cAaE7rJgXQ19ycdCHwx)

* Visit your [Order Cycles](https://openfoodnetwork.org.uk/admin/order\_cycles) page. &#x20;
* Set up your next [order cycle](../../basic-features/shopfront/order-cycle/order-cycles-for-hubs.md). Set the opening time as ‘now’ and the closing time your usual closing time.
* On page 3 (‘Outgoing Products’) add ‘preview’ into the tag section:

![](../../.gitbook/assets/previewtagoc.jpg)

* Visit your **Enterprise -> Settings** page and select ‘[Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-order-cycles-at-my-shopfront)’ from the left hand menu.  Set up the following Tag rules:\
  Default: Order Cycles tagged ‘preview’ are not visible.\
  For Customers tagged ‘producer’, Order Cycles tagged ‘preview’ are visible.

![](../../.gitbook/assets/previewtags.jpg)

**Bingo!  Your order cycle is now open for your producers to view their products on your shop front but general customers will not be able to view (or shop).**

{% hint style="warning" %}
Producers/suppliers can make purchases during this time
{% endhint %}

### Step Two

* **Set a reminder on your phone/calendar to edit your order cycles at the time and day you wish shopping to commence.**
* At this time visit your [order cycles](https://openfoodnetwork.org.uk/admin/order\_cycles) and select ‘Edit’ next to the one you wish to make ‘live’ to customers:

![](../../.gitbook/assets/previewocedit.jpg)

* Visit ‘Outgoing Products’ section on page 3 and remove the tag:

![](https://lh6.googleusercontent.com/dMsKV7a4YiCbY5NwxB7ijwgZVZCT8uHvzTrEgjzkJzfePixGehUtZA3vIyel0knRI8c5nThtPCn50-3bUEgrb\_o9zJbp7uV5HqeGdOimAmj08UMOhgAxqWsQy4UePE8-xksAS9DO)

**All your customers will be able to view your shop and make purchases now!**

###
