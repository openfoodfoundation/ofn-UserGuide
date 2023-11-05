# Konfiguration

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Aktivieren von Abonnements

Um die Abonnementfunktion für Ihr Unternehmen zu aktivieren, gehen Sie zu Unternehmen-> Einstellungen-> [Shop-Einstellungen](../enterprise-profile/enterprise-settings.md#shop-einstellungen).

Ändern Sie unten auf der Seite Abonnements auf "aktiviert".

![](../../.gitbook/assets/subscriptions1.jpg)

**Gastbestellungen:** Für Unternehmen mit aktivierten Abonnements empfehlen wir, dass sich alle Kunden anmelden müssen, bevor sie bei Ihnen einkaufen können. Dadurch wird sichergestellt, dass jeder Kunde mit einem Abonnement sich anmeldet und seine bestehende Abonnementbestellung sieht und nicht versehentlich eine Doppelbestellung aufgibt.

**Aufträge ändern:** Für Kunden mit einem regelmäßig wiederkehrenden Auftrag von Ihrem Unternehmen im Abonnement, dann gelten die folgenden Optionen:

* _Erteilte Aufträge können nicht geändert/storniert werden:_ Der Kunde muss sich mit Ihnen in Verbindung setzen, um seine reguläre Bestellung zu ändern (Änderung der Mengen der einzelnen gewünschten Produkte oder Stornierung der Bestellung).
* _Kunden können Bestellungen ändern/stornieren, während der Bestellzyklus offen ist:_ Der Kunde kann die Menge der Produkte, die er in seinem Abonnement wünscht, ändern und/oder die gesamte Bestellung stornieren.

{% hint style="info" %}
Wenn ein Kunde mit einer Abonnementbestellung ein Produkt kaufen möchte, das nicht Teil seiner regulären Bestellung ist, muss er in jedem Fall einen zweiten Warenkorb anlegen und zur Kasse gehen. **Weder Sie noch der Kunde können neue Produkte zu seiner Abonnementbestellung hinzufügen, sobald der Bestellzyklus geöffnet ist.**
{% endhint %}

## Versand- und Zahlungsarten für Abonnements

Wenn Sie das Abonnement des Kunden erstellen, müssen Sie die Versandart und die Zahlungsmethode auswählen, mit der der Kunde bezahlt werden soll. Dies gilt dann für alle folgenden Bestellungen, die in ihrem Namen über die Abonnements aufgegeben werden

### Versandmethoden

You can apply any [shipping/delivery method](../shopfront/shipping-methods.md) to a subscription.&#x20;

### Zahlungsmöglichkeiten

You can only assign two types of [payment methods](../shopfront/payment-methods.md) to subscriptions.

1. **Manual payment methods:** Cash, cheque, bank transfer (ie. any method which does not involve automatic validation online by the OFN platform).
2. **Stripe:** Stripe is a payment gateway that takes payment with credit cards.  Details on how to configure Stripe payments for your enterprise can be found [here](../shopfront/payment-methods.md#integrated-payment-providers).&#x20;

{% hint style="info" %}
With each order automatically placed by a subscription, the customer's bank card will be debited for the order (on closure of the associated order cycle). The amount debited will reflect any modifications made by you or them to the order.\
Customers will not be charged if they cancel their subscription order.
{% endhint %}

{% hint style="warning" %}
For the customer to be debited correctly, it is necessary for them to have an account on the Open Food Network platform.  To their OFN account they must have registered a default credit card and given their authorisation for your enterprise to debit from that card.  More information can be found [here](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authorising-charges). &#x20;
{% endhint %}

{% hint style="success" %}
If you use Stripe as the payment method for subscriptions it is helpful to the customer if you add a clear, detailed explanation of how the payment will be processed, should they choose this option.\
\
For example, rather than calling the [payment method](../shopfront/payment-methods.md) 'Credit card' you might like to call it 'automated credit card billing for subscriptions'. A possible description could be 'Your default credit card saved in your OFN account will be charged when your subscription order is confirmed on Wednesday nights'. This name and description will show on the email confirmation to subscription customers (see example below), so it's good to make it details so the customer knows what to expect.
{% endhint %}

![](<../../.gitbook/assets/image (15).png>)

## Sammeln Sie Informationen von Ihren Kunden

To setup a subscription for a customer you'll need to get some information from them, as detailed below:

**Name**, **phone number** and **email address:** Remember that any customer wishing to have an automated regular order (subscription) with your enterprise MUST have a registered and confirmed user account on the OFN platform.  Customers with subscriptions must be on your enterprise [Customer List](../shopfront/customer-management-and-conditional-displays-prices/customers.md). See [below](subscriptions-configuration.md#add-your-subscribers-to-your-customer-list) for more details.

**Billing and shipping address**

**Products:** Which items do they want to include in their subscription?

**Shipping/Delivery method**: You need to assign a shipping/delivery/collection method to their subscription order.  How would they prefer to receive the goods?

**Payment method**: Customers can select from your manual payment methods (e.g. cash, bank transfer), or paying with their credit card through your shop's Stripe account. If the customer wishes to pay for their subscription orders by Stripe then they will need to add a default payment card and give authorisation. See [here](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authorising-charges) for more details.

**Start and End Dates for their subscription orders:** Remember, for a subscription order to be created for a given order cycle it must have a start date either before or after the order cycle opening date, and the subscription end date must be after the order cycle close date.

## Fügen Sie Ihre Abonnenten zu Ihrer Kundenliste hinzu

Before you can setup a subscription order for a customer they need to be added to your [Customers list](../shopfront/customer-management-and-conditional-displays-prices/customers.md).&#x20;

**After you've added your customers to your customer list email them** and [ask them to sign up for an account on OFN](subscriptions-the-customers-perspective.md#signing-up-to-ofn).  If you plan to bill customers using Stripe, you need to also request that they follow the additional steps outlined [here](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authorising-charges) for adding a default credit/debit card to their OFN user account and giving your enterprise authorisation to take payments.

{% hint style="info" %}
You can add customers to your Customer list before or after they've signed up for an account with OFN. However, before a subscription order can be successfully setup the customer must have confirmed the email address to which their OFN account is registered.
{% endhint %}

{% hint style="warning" %}
If you wish to debit a customer for their subscription order by Stripe then they must be added to your [Customer list](../shopfront/customer-management-and-conditional-displays-prices/customers.md) BEFORE they can [authorise your enterprise to take payments ](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authorising-charges)from their credit/debit card.\
Hence we recommend the following procedure:

1. Contact the customer and obtain all the info you require (see [above](subscriptions-configuration.md#gather-information-from-your-customers))
2. Add them to your [customer list](../shopfront/customer-management-and-conditional-displays-prices/customers.md).
3. Email the customer, asking them to [register with OFN](subscriptions-the-customers-perspective.md#signing-up-to-ofn) for an account and [add their credit/debit card details](subscriptions-the-customers-perspective.md#saving-credit-cards-and-authorising-charges) to that account.
4. [Create the subscription](subscriptions-creating-and-managing-orders.md).
{% endhint %}

## Zeitpläne

{% hint style="info" %}
If you are new to OFN we encourage you to get familiar with setting up [order cycles](../shopfront/order-cycle/) before setting up schedules and subscriptions
{% endhint %}

### Über Zeitpläne

Subscriptions are setup so that every time an enterprise opens an order cycle, orders can be automatically generated for customers who have a subscription with that shop.  The frequency with which a subscription order is placed for a particular customer (ie which of your active order cycles triggers their subscription) is controlled by a facility called '**Schedules**'. &#x20;

Schedules are groups that order cycle can be assigned to. Once a schedule has been created, customer subscriptions are applied to the schedule, so that an order for their subscription will only be generated for new order cycles in that schedule. &#x20;

{% hint style="info" %}
You may have some customers who would like a regular order every week, in which case you would add their subscriptions to a schedule which includes all of your weekly order cycles. For other groups of customers, desiring their orders only fortnightly/monthly you can create additional schedules which only include alternate/one-in-four of your weekly order cycles.
{% endhint %}

{% hint style="success" %}
There's lots of flexibility in this arrangement and so feel free to experiment to come up with the order cycle-schedule combination which works best for your enterprise.  For example you may wish to have 'odd week' and 'even week' schedules, 'wholesale' schedules, 'monthly meat' schedules....
{% endhint %}

### Einen Zeitplan erstellen

Having completed all the steps outlined above, the **+New Schedule** button will appear at the top of your Order Cycles menu:

![](<../../.gitbook/assets/ordercycle1 (2) (2).jpg>)

{% hint style="warning" %}
You must have at least one open or due to open order cycle to be able to create a new schedule.
{% endhint %}

![](../../.gitbook/assets/new-schedule.bin)

**Name:** Give the schedule a logical name which describes this group of order cycles. E.g. ‘weekly’, ‘monthly’, ‘Tuesday Deliveries’, ‘wholesale’ or ‘retail’. This name is not visible to customers.

{% hint style="info" %}
If you manage several OFN enterprises, with subscriptions being enabled in more than one, then naming your schedules clearly is essential eg. weekly\_hubA, weekly\_hubB, fortnightly\_hubA, fortnightly\_hubB.\
Each enterprise will need a different schedule but when you create a subscription for a customer the schedules for all your enterprises will be visible. Hence, the descriptive name will help you make sure the subscription is created for the correct enterprise for that particular customer.
{% endhint %}

You can add existing order cycles into and out of the new schedule by clicking the < and > buttons.

Click **create** when you are finished.

### Bearbeiten oder Löschen eines Zeitplans

Um einen Zeitplan zu bearbeiten oder zu löschen, klicken Sie auf den Namen des Zeitplans neben dem entsprechenden Auftragszyklus in der Spalte "Zeitpläne". (Möglicherweise müssen Sie die Spalte "Zeitpläne" sichtbar machen, indem Sie sie im Dropdown-Spaltenmenü oben rechts anklicken).

![](../../.gitbook/assets/show-schedules.bin)

Sie können den Namen des Zeitplans ändern, Auftragszyklen hinzufügen/entfernen oder den Zeitplan löschen.

![](../../.gitbook/assets/delete-schedule.bin)

{% hint style="danger" %}
Sie können einen Zeitplan nicht löschen, wenn er mit Abonnements verbunden ist.
{% endhint %}

### Hinzufügen oder Entfernen von Auftragszyklen aus Zeitplänen

You can add and remove order cycles from schedules by either editing the schedule ([above](subscriptions-configuration.md#edit-or-delete-a-schedule)), or by editing the order cycle and adding/removing the schedule in the ‘schedules’ field:

![](../../.gitbook/assets/ordercycle3.jpg)

{% hint style="success" %}
Auftragszyklen können in mehr als einem Zeitplan enthalten sein. Wenn Ihre Auftragszyklen beispielsweise wöchentlich sind, Sie aber drei Zeitpläne haben (wöchentlich, vierzehntägig-ungerade Wochen und vierzehntägig-gerade Wochen), dann kann ein Auftragszyklus sowohl mit dem "wöchentlichen" als auch mit dem "vierzehntägig-ungeraden" Wochenzeitplan verbunden sein.
{% endhint %}

