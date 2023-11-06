# Wie man Geschenkgutscheine erstellt

## Introduction

{% hint style="warning" %}
Die einfache Implementierung von Geschenkgutscheinen (Verkauf und Einlösung) ist derzeit keine Funktion der OFN-Plattform, obwohl wir hoffen, sie in Zukunft einführen zu können.
{% endhint %}

In der Zwischenzeit ist es möglich, Gutscheine mit Hilfe von Tags und Tag-Regeln zu erstellen. Der Vorgang wird im Folgenden beschrieben. Gutscheine sind zu Weihnachten und anderen saisonalen Anlässen immer sehr beliebt, und aufgrund der Komplexität der Ausstellung könnte es sich lohnen, Gutscheine nur zu bestimmten Zeiten des Jahres anzubieten.

Eine alternative "Geschenk"-Option, die Ihr Unternehmen in Betracht ziehen könnte, ist die Möglichkeit, dass ein Kunde (der Schenkende) ein [Abonnement](../../basic-features/subscriptions/) (regelmäßige Bestellung) für einen Freund oder ein Familienmitglied (den Beschenkten) abschließt. Zum Beispiel könnte der Schenkende dafür sorgen, dass der Beschenkte einen Monat lang jede Woche sein Lieblingsbrot von Ihrem Lebensmittelunternehmen geliefert bekommt (auf Kosten des Schenkenden).

Dies hätte für den Schenkenden den zusätzlichen Vorteil, dass die Kosten des Geschenks wöchentlich verteilt würden und nicht als Pauschalbetrag gezahlt werden müssten: Zu Weihnachten und in anderen Jahreszeiten ist der Geldfluss für alle knapp!

## Process

{% hint style="warning" %}
Dies ist ein mehrstufiger Prozess
{% endhint %}

### Step One

Erstellen Sie ein [Produktverzeichnis](../../basic-features/products-1/products.md) für Gutscheine. Wir schlagen vor, dass Sie es einfach halten, d.h. nur maximal drei verschiedene Gutscheinwerte (£10, £20, £50). Denken Sie daran:

* To include instructions to the customer on how they can redeem their voucher later (they will need to ask the recipient of the voucher to email your enterprise with their voucher ID number (see [step 2](how-to-create-gift-vouchers.md#step-two)) and email address ([step 5](how-to-create-gift-vouchers.md#step-five)) with which they have set up an OFN account.)

![](../../.gitbook/assets/voucher1.jpg)

* That [enterprise fees](../../basic-features/shopfront/enterprise-fees.md) are included in the price of the voucher.  The person who redeems the voucher will also have the enterprise fee added onto the products they purchase (ie. fees will be collected twice). The extra enterprise fee may be necessary to cover the added overheads of admin work, processing gift vouchers. Alternatively the product price can be adjusted so that the customer facing price (product price + fee) is the voucher’s value.

![](../../.gitbook/assets/voucher2.jpg)

### Zweiter Schritt

Email a voucher to the customer or print off a paper one. Give each voucher a unique number (perhaps use their OFN order number with post fix of a, b, c etc if more than one voucher purchased in the same transaction).

Example:

![](../../.gitbook/assets/1.png)

This voucher was made using the free online software [Canva](https://www.canva.com/).

### Dritter Schritt

Make a spreadsheet to record sales and keep track of claims: name of customer (gifter), amount, date of issue, order number/voucher ID number, name of recipient (giftee), credit remaining**.**

| Gifter email address             | Value of Voucher            | Date purchased | Voucher ID number | Giftee email address             | Credit remaining |
| -------------------------------- | --------------------------- | -------------- | ----------------- | -------------------------------- | ---------------- |
| <p>…@gmail.com<br>Joe Bloggs</p> | <p>£20</p><p>R185277652</p> | 10/10/20       | JB\_7652a         | <p>…@hotmail.com<br>Mr Baker</p> | £20              |
|                                  |                             |                |                   |                                  |                  |
|                                  |                             |                |                   |                                  |                  |

### Vierter Schritt

Customer who bought the voucher (gifter) gives it to a friend or family member at Christmas (giftee). For the giftee to redeem their voucher they need to contact your hub/shop informing you of:

* The email address associated with their OFN account (for [step 5](how-to-create-gift-vouchers.md#step-five))
* Their unique voucher ID number (for you to keep track of vouchers issued and redeemed).

### Schritt Fünf

Add the giftee to your enterprise [Customer](https://openfoodnetwork.org.uk/admin/customers) list if they have not purchased from the shop in the past. If they have brought before then they will appear on the list already. &#x20;

![](https://lh6.googleusercontent.com/kQ9p8e9MwV59o9bnXYdzS2yZCPduKmJrBr3PF0y--YxnUSCgTPlYvXgWgHVVv45T6RFCVfeuVZO32H2TggixTTkP\_zzKitwD3Q3PeR70OrCWApmCVvJRUZtzQavLaADi6hYd-wsZ)

**Add a unique tag next to the customer’s name.** Perhaps use initials-underscore-last four digits of the voucher ID number (set up a consistent way of doing this).

### Schritt Sechs

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

### Schritt Sieben

Set up a [Tag rule](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-payment-methods) (visit **Enterprises -> Settings -> Tag Rules**):

Default: Payment Methods tagged initials\_digits are not visible\
Rule: for customers tagged initials\_digits payment methods tagged initials\_digits are visible.

![](https://lh5.googleusercontent.com/XNlPg1s5bgvq42adGiNAcJ6-1u4HAGDokwbp7jainIZM0RxROZMhW\_kKrfrbGIUIjKJleibB-5glFEGySi3Dc6bbkdKctyKsJgmu6mFiskNOAxqqxEhX4JQWSSuC2TpD4HgdGiOX)

### Der Kunde (Beschenkte) nutzt den Gutschein und überschreitet den Wert des Restguthabens:&#x20;

* Delete their unique payment method, tag rule and tag associated with customer’s (giftee’s) name.
* Obtain the balance of their order by cash payment or BACS

### Der Kunde (Beschenkte) nutzt den Gutschein, gibt aber nicht den gesamten Wert aus:&#x20;

Edit their unique payment method to adjust the ‘amount’ under Fee Calculator to their remaining voucher balance (eg. if the voucher’s original value was £20, they spent £15 then the original amount would be -20 and the amount after their first transaction would need to be edited to -5)\


### Zu beachtende Punkte:

* If a customer (giftee) makes a second purchase before you have had a chance to update their remaining credit or remove the unique payment option (if all their credit has been used up) then they will have the option to claim the voucher’s value twice. This relies on the customer being honest and not doing so. This should be mentioned on the voucher and in the description of their payment method ([step 6](how-to-create-gift-vouchers.md#step-six)). As an enterprise you could cancel orders if a voucher is redeemed inappropriately- always good to notify the customer (giftee) first though!
* It is a good policy with vouchers to set an expiry date (say 12 months).
