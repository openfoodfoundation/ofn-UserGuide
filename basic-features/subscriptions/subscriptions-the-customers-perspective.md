# Subscriptions - the customer's perspective

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

This page details what a customer with a subscription can expect. It also highlights some things that shops offering subscriptions should be aware of.

## Anmeldung bei OFN

Customers must have an account with OFN before you can process subscription orders for them.

To create an account, direct the customer to the local Open Food Network home page and 'Login' at the top right hand corner.  They'll be guided through registering with OFN. _**Customers must have an active email address to register**_.

After signing up they'll be sent a confirmation email. Once they click on the link in this email their account will be confirmed and they will be able to login.&#x20;

{% hint style="info" %}
Due to over zealous email filters (designed to ward off spam) sometimes customers won't receive their confirmation email from us (or it will be directed to their junk folder).  If this occurs ask them to add open food network to their 'safe' list in their email account settings.
{% endhint %}

## Speichern von Kreditkarten und Autorisierung von Gebühren

Customer who want to pay for their subscription orders via automated charges onto their credit/debit card (Stripe) need to a) save their preferred card in their OFN account and b) grant the shop permission to charge that card.&#x20;

### Speichern der Kreditkartendaten im Kundenkonto

The Customer's Account page can be accessed after logging into OFN by the top right hand 'Profile' button:

![](../../.gitbook/assets/subcard1.jpg)

Your customer can save one or more cards in their account, in the **credit cards** tab.

![](../../.gitbook/assets/subcard2.jpg)

If a customer registers more than one debit/credit card, then the card which is denoted as 'default' will be the one which is charged automatically by Stripe (if they have a subscription with Stripe as the chosen payment method).&#x20;

{% hint style="danger" %}
If none of their cards are selected as 'default' their credit card payments won't be processed.
{% endhint %}

![](<../../.gitbook/assets/image (26).png>)

If your customer saves credit cards in their account, they'll also be able to quickly select these when they shop in your shop at checkout.

![](<../../.gitbook/assets/image (4).png>)

### Einem Geschäft die Genehmigung erteilen, seine Standardkarte zu belasten

**You should add your customers to your** [**Customer List**](../shopfront/customer-management-and-conditional-displays-prices/customers.md) **before you ask them to save their credit card details and authorise your shop to bill their card. The customer will not see your enterprise under the 'Authorised Shops' list on the right if you have not done so.**

For the Stripe payment method to work for a subscription the customer has with your enterprise they must check the 'Allow Charges' box:

![](../../.gitbook/assets/subcard2.jpg)
