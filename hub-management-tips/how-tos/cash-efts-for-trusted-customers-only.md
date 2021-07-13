# Cash/EFTs for trusted customers only

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

## Introduction

It’s always really disappointing if your supplier has spent time and resources to prepare goods for a customer and then they don’t arrive to collect their shopping.  This is especially a risk when payment is not taken up front for goods.  

Using [Stripe \(card payment\) or PayPal ](../../basic-features/shopfront/payment-methods.md)businesses can automatically collect payment from their shoppers at the time of checkout using the OFN platform.  These card payment methods may not suit all your customers though: some people are afraid of online payments, some may not have a bank account and others might use cash as a way of keeping track of their weekly budgets.

As a manager of a local food enterprise you are in tune with your customers’ needs.  You might like the majority of your customers to pay by card \(less admin time for you to chase/collect payments by BACS or cash, peace of mind that you have payment upfront for goods rather than waiting for the day of collection …. etc\) but allow a small selection who you know and trust to pay by cash or BACS.  You can use [Tags and Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-payment-methods) to implement this as described below.

## Process

* Set up a [Stripe](../../basic-features/shopfront/payment-methods.md#integrated-payment-providers) \(or PayPal\) payment method which will be your only option for the majority of shoppers. \(Visit **Enterprises -&gt; Settings -&gt; Payment Method** and ‘**Create New Payment Method+**’. See [this guide](https://guide.openfoodnetwork.org/basic-features/shopfront/payment-methods) for more information.\)
* Create a second payment method with the following settings: Name: ‘Cash or BACS payment’ Description: provide relevant details here such as bank information required for a trusted customer to make direct payment to your bank account Display: Both checkout and back office Active: yes **Tags: ‘trusted’** Provider: Cash/EFT/etc

![](https://lh6.googleusercontent.com/jybdqQT_WgpCQfNB6v6DCWrE_iMN7og0wwK43P_1H89CJknrwUuqtArffusumwVmjj9mMalf90DIfRG-3xFnnzPbiMT0EyjrxlakDAhzkvqHXxzyKmBsY7VynAYQgYCau-dsRyzC)

* Visit your  [Customers](https://openfoodnetwork.org.uk/admin/customers) page.
* Use the ‘Quick Search’ box to find your regular and trusted customer’s details: 

![](https://lh6.googleusercontent.com/DcRo1W18G7l7JKxuhHybJB4gIEzZWQIX-3kynCMX79RwtrKFpMR8b6SYI4uyoQjGOOlmrV1rv7oIbsYS55UkfeH1yfu4SJntTnO1vMPmwuTMljBhkX_kRhYLiI5fKzKjxYBR_uCO)

* Add the Tag ‘trusted’ to their entry:

![](../../.gitbook/assets/trustedcust.jpg)

* Visit **Enterprises -&gt; Settings -&gt; Tag Rules** and add the following:

Default: Payment Methods tagged ‘trusted’ are NOT VISIBLE  
Rule: For Customers tagged ‘trusted’ Payment Methods tagged ‘trusted’ are visible.

![](../../.gitbook/assets/trustedtags.jpg)

**Bingo!  Only your trusted customers will be offered the choice of payment by cash or BACS.** 

{% hint style="success" %}
If you find a customer regularly fails to pay on collection or is repeatedly late with BACS payments then you can always remove this option by deleting the tag ‘trusted’ on their [Customer](https://openfoodnetwork.org.uk/admin/customers) record.  The shopper will then only be able to pay by card upfront, like your other customers.
{% endhint %}

