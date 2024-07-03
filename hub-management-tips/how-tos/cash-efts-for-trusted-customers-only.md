# Cash/EFTs for trusted customers only

{% hint style="info" %}
This functionality is best achieved using the [Tags and Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) feature of the platform.
{% endhint %}

## Introduction

It’s always really disappointing if your supplier has spent time and resources to prepare goods for a customer and then they don’t arrive to collect their shopping.  This is especially a risk when payment is not taken up front for goods. &#x20;

Using [Stripe (card payment) or PayPal ](../../basic-features/shopfront/payment-methods.md)businesses can automatically collect payment from their shoppers at the time of checkout using the OFN platform.  These card payment methods may not suit all your customers though: some people are afraid of online payments, some may not have a bank account and others might use cash as a way of keeping track of their weekly budgets.

As a manager of a local food enterprise you are in tune with your customers’ needs.  You might like the majority of your customers to pay by card (less admin time for you to chase/collect payments by BACS or cash, peace of mind that you have payment upfront for goods rather than waiting for the day of collection …. etc) but allow a small selection who you know and trust to pay by cash or BACS.  You can use [Tags and Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-payment-methods) to implement this as described below.

## Process

* Set up a [Stripe](../../basic-features/shopfront/payment-methods.md#integrated-payment-providers) (or PayPal) payment method which will be your only option for the majority of shoppers. (Visit **Enterprises -> Settings -> Payment Method** and ‘**Create New Payment Method+**’. See [this guide](https://guide.openfoodnetwork.org/basic-features/shopfront/payment-methods) for more information.)
* Create a second payment method with the following settings:\
  Name: ‘Cash or BACS payment’\
  Description: provide relevant details here such as bank information required for a trusted customer to make direct payment to your bank account\
  Display: Both checkout and back office\
  Active: yes\
  **Tags: ‘trusted’**\
  Provider: Cash/EFT/etc

![](<../../.gitbook/assets/trusted 3.jpg>)

* Visit your  [Customers](https://openfoodnetwork.org.uk/admin/customers) page.
* Use the ‘Quick Search’ box to find your regular and trusted customer’s details:&#x20;

![](../../.gitbook/assets/customers.jpg)

* Add the Tag ‘trusted’ to their entry:

![](<../../.gitbook/assets/trusted 2.jpg>)

* Visit **Enterprises -> Settings -> Tag Rules** and add the following:

Default: Payment Methods tagged ‘trusted’ are NOT VISIBLE\
Rule: For Customers tagged ‘trusted’ Payment Methods tagged ‘trusted’ are visible.

![](<../../.gitbook/assets/trusted 1.jpg>)

* When you open an [order cycle](../../basic-features/shopfront/order-cycle/), on page 4 '**Checkout Options**' select at least one automatic payment method which is visable for the majority of your customers (Stripe and/or PayPal) as well as the new tagged payment method set up above 'BACS payment'.

**Bingo!  Only your trusted customers will be offered the choice of payment by cash or BACS.**&#x20;

{% hint style="success" %}
If you find a customer regularly fails to pay on collection or is repeatedly late with BACS payments then you can always remove this option by deleting the tag ‘trusted’ on their [Customer](https://openfoodnetwork.org.uk/admin/customers) record.  The shopper will then only be able to pay by card upfront, like your other customers.
{% endhint %}
