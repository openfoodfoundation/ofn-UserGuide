# Open your Shop on 'Preview'

{% hint style="info" %}
This functionality is best achieved using the [Tags and Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) feature of the platform.
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

![](<../../.gitbook/assets/preview 3.jpg>)

* Visit your [Order Cycles](https://openfoodnetwork.org.uk/admin/order\_cycles) page. &#x20;
* Set up your next [order cycle](../../basic-features/shopfront/order-cycle/order-cycles-for-hubs.md). Set the opening time as ‘now’ and the closing time your usual closing time.
* On page 3 (‘Outgoing Products’) add ‘preview’ into the tag section:

![](<../../.gitbook/assets/preview 4.jpg>)

* Visit your **Enterprise -> Settings** page and select ‘[Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-order-cycles-at-my-shopfront)’ from the left hand menu.  Set up the following Tag rules:\
  Default: Order Cycles tagged ‘preview’ are not visible.\
  For Customers tagged ‘producer’, Order Cycles tagged ‘preview’ are visible.

![](<../../.gitbook/assets/preview 2.jpg>)

**Bingo!  Your order cycle is now open for your producers to view their products on your shop front but general customers will not be able to view (or shop).**

{% hint style="warning" %}
Producers/suppliers can make purchases during this time
{% endhint %}

### Step Two

* **Set a reminder on your phone/calendar to edit your order cycles at the time and day you wish shopping to commence.**
* At this time visit your [order cycles](https://openfoodnetwork.org.uk/admin/order\_cycles) and select ‘Edit’ next to the one you wish to make ‘live’ to customers:

![](<../../.gitbook/assets/preview 5.jpg>)

* Visit ‘Outgoing Products’ section on page 3 and remove the tag:

![](<../../.gitbook/assets/preview 6.jpg>)

**All your customers will be able to view your shop and make purchases now!**

###
