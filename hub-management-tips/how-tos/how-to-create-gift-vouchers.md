# Wie man Geschenkgutscheine erstellt

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Introduction

{% hint style="warning" %}
Simple implementation of gift vouchers (selling and redeeming) is not a feature of the OFN platform at present, although it is something we hope to introduce in the future.
{% endhint %}

In the meantime it is possible to use tags and tag rules to create vouchers.  The process is described below.  Vouchers are always popular around Christmas and other seasonal events and owing to the complexity of issuing them it may be worth considering only offering vouchers at specific times of year.

An alternative 'gift' option which your enterprise may like to consider is to allow a customer (the gifter) to purchase a [subscription](../../basic-features/subscriptions/) (regular order) for a friend or family member (giftee).  For example the gifter could arrange for the giftee to receive their favourite handmade, local bread to be delivered to them (paid for by gifter), from your food enterprise, every week for a month.

This would have the extra advantage for the gifter that the cost of the gift would be spread weekly and not a lump payment: cash flow for everyone is tight at Christmas and other seasonal periods!

## Process

{% hint style="warning" %}
This is a multi-step process
{% endhint %}

### Step One

Create a [product listing](../../basic-features/products-1/products.md) for vouchers. We suggest that you keep it simple ie. having a maximum of three different denominations of voucher only (£10, £20, £50).\
Remember:&#x20;

* To include instructions to the customer on how they can redeem their voucher later (they will need to ask the recipient of the voucher to email your enterprise with their voucher ID number (see [step 2](how-to-create-gift-vouchers.md#step-two)) and email address ([step 5](how-to-create-gift-vouchers.md#step-five)) with which they have set up an OFN account.)

![](../../.gitbook/assets/voucher1.jpg)

* That [enterprise fees](../../basic-features/shopfront/enterprise-fees.md) are included in the price of the voucher.  The person who redeems the voucher will also have the enterprise fee added onto the products they purchase (ie. fees will be collected twice). The extra enterprise fee may be necessary to cover the added overheads of admin work, processing gift vouchers. Alternatively the product price can be adjusted so that the customer facing price (product price + fee) is the voucher’s value.

![](../../.gitbook/assets/voucher2.jpg)

### Step Two

Email a voucher to the customer or print off a paper one. Give each voucher a unique number (perhaps use their OFN order number with post fix of a, b, c etc if more than one voucher purchased in the same transaction).

Example:

![](../../.gitbook/assets/1.png)

This voucher was made using the free online software [Canva](https://www.canva.com/).

### Step Three

Make a spreadsheet to record sales and keep track of claims: name of customer (gifter), amount, date of issue, order number/voucher ID number, name of recipient (giftee), credit remaining**.**

| Gifter email address             | Value of Voucher            | Date purchased | Voucher ID number | Giftee email address             | Credit remaining |
| -------------------------------- | --------------------------- | -------------- | ----------------- | -------------------------------- | ---------------- |
| <p>…@gmail.com<br>Joe Bloggs</p> | <p>£20</p><p>R185277652</p> | 10/10/20       | JB\_7652a         | <p>…@hotmail.com<br>Mr Baker</p> | £20              |
|                                  |                             |                |                   |                                  |                  |
|                                  |                             |                |                   |                                  |                  |

### Step Four

Customer who bought the voucher (gifter) gives it to a friend or family member at Christmas (giftee). For the giftee to redeem their voucher they need to contact your hub/shop informing you of:

* The email address associated with their OFN account (for [step 5](how-to-create-gift-vouchers.md#step-five))
* Their unique voucher ID number (for you to keep track of vouchers issued and redeemed).

### Step Five

Add the giftee to your enterprise [Customer](https://openfoodnetwork.org.uk/admin/customers) list if they have not purchased from the shop in the past. If they have brought before then they will appear on the list already. &#x20;

![](https://lh6.googleusercontent.com/kQ9p8e9MwV59o9bnXYdzS2yZCPduKmJrBr3PF0y--YxnUSCgTPlYvXgWgHVVv45T6RFCVfeuVZO32H2TggixTTkP\_zzKitwD3Q3PeR70OrCWApmCVvJRUZtzQavLaADi6hYd-wsZ)

**Add a unique tag next to the customer’s name.** Perhaps use initials-underscore-last four digits of the voucher ID number (set up a consistent way of doing this).

### Step Six

Set up a NEW [payment method](../../basic-features/shopfront/payment-methods.md#setting-up-a-payment-method) which will be UNIQUE to this customer (the giftee).  Payment Methods can be found by visiting **Enterprises -> Settings -> Payment Methods +New Payment Method**.

![](https://lh3.googleusercontent.com/6ByGcLUnW\_rDqrBloGtym1i64JhDcMEVFospqUCR7BZc1vk5lbpiqZREU3LhN8iU9bqKPyM\_Wnd4YJwkkvgPWX4JIP9yHszyboX5rnZagwiaFMs0jbKage3z\_\_gVKGDG2fLFPch\_)

Description- use the description box to explain to the customer the value of the voucher they have received from their friend/family, that any balance on their order will need to be made up by cash or BACS (provide bank details on how to do this) if necessary. It is also worth explaining any terms and conditions- for example that the voucher is single use (ie. once the value has been claimed then if they use the voucher again immediately the 2nd order will be cancelled or full payment will be required) and expiry date for the voucher.\
Display = Both Checkout and Backoffice\
Active = yes\
**Add tag to payment method (same as used for the customer).**\
Provider- cash (if the customer spends more than the value of their voucher then they will need to pay the remainder by cash or BACS)

{% hint style="danger" %}
Do not use an automated payment provider (Stripe or PayPal) here as this will result in a payment being made from your enterprise into the giftee's bank account if they spend less than the voucher value.
{% endhint %}

Fee Calculator: Flat Rate\
Amount: enter the value of their voucher prefixed by a negative sign.

![](../../.gitbook/assets/christmaspmcalc.jpg)

### Step Seven

Set up a [Tag rule](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-payment-methods) (visit **Enterprises -> Settings -> Tag Rules**):

Default: Payment Methods tagged initials\_digits are not visible\
Rule: for customers tagged initials\_digits payment methods tagged initials\_digits are visible.

![](https://lh5.googleusercontent.com/XNlPg1s5bgvq42adGiNAcJ6-1u4HAGDokwbp7jainIZM0RxROZMhW\_kKrfrbGIUIjKJleibB-5glFEGySi3Dc6bbkdKctyKsJgmu6mFiskNOAxqqxEhX4JQWSSuC2TpD4HgdGiOX)

### **Customer (giftee) uses voucher and exceeds the value of credit remaining:**&#x20;

* Delete their unique payment method, tag rule and tag associated with customer’s (giftee’s) name.
* Obtain the balance of their order by cash payment or BACS

### **Customer (giftee) uses voucher but doesn’t spend its entire value:**&#x20;

Edit their unique payment method to adjust the ‘amount’ under Fee Calculator to their remaining voucher balance (eg. if the voucher’s original value was £20, they spent £15 then the original amount would be -20 and the amount after their first transaction would need to be edited to -5)\


### **Things to note:**

* If a customer (giftee) makes a second purchase before you have had a chance to update their remaining credit or remove the unique payment option (if all their credit has been used up) then they will have the option to claim the voucher’s value twice. This relies on the customer being honest and not doing so. This should be mentioned on the voucher and in the description of their payment method ([step 6](how-to-create-gift-vouchers.md#step-six)). As an enterprise you could cancel orders if a voucher is redeemed inappropriately- always good to notify the customer (giftee) first though!
* It is a good policy with vouchers to set an expiry date (say 12 months).
