# Ermäßigte/freie Lieferung für schutzbedürftige Kunden

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Introduction

Elderly or vulnerable customers may find it more difficult to reach your hub or shop collection point.  Whilst it wouldn't necessarily be possible for you to deliver goods to every customer's doorstep (due to cost, time and distances involved) you may have capacity to help a small number of local 'priority' customers.

Below is a step-by-step guide to enable selected customers to access free (or discounted) delivery.

The process uses the Customer Management feature which is described in [full here](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-shipping-methods).

## **Things to consider before starting**

* What is the maximum number of delivery slots you can offer for free/discounted rate?
* Which areas would you consider delivering to free of charge or at a discounted rate?  For instance, limit the area to a specific postcode/street/district or perhaps to streets on your way home.
* Be realistic about the number of deliveries you can make and the cost of petrol/time to make them.

## Process

* Keep a record of the customer’s name and the email address linked to their OFN account.
* Login to your business OFN account and visit [Customers](https://openfoodnetwork.org.uk/admin/customers) [page](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/customers.md).
* Use the ‘Quick Search’ box to identify if the person has shopped with you before.&#x20;

![](https://lh6.googleusercontent.com/DcRo1W18G7l7JKxuhHybJB4gIEzZWQIX-3kynCMX79RwtrKFpMR8b6SYI4uyoQjGOOlmrV1rv7oIbsYS55UkfeH1yfu4SJntTnO1vMPmwuTMljBhkX\_kRhYLiI5fKzKjxYBR\_uCO)

* If their email address doesn’t appear then click **+ New Customer** and add their address.
* Add the tag ‘free\_delivery’ to the customers entry.

![](../../.gitbook/assets/freedelivtagcust.jpg)

* Visit **Enterprises -> Settings ->** [**Shipping Methods**](../../basic-features/shopfront/shipping-methods.md) and click **+New Shipping Method**.

![](../../.gitbook/assets/freedeliv.jpg)

Name: Free local home delivery for elderly and vulnerable customers.\
Description: Free local delivery to your home address.\
Display: Both Checkout and Back Office\
Category: Delivery\
**Tags: Add the tag ‘free\_delivery’ into this space.**\
Fee Calculator: Flat Rate amount = 0.00\
Categories: Default\
Zones: UK\_VAT

* Visit your **Enterprise -> Settings** page and select ‘[Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md)’ from the left hand menu.  Set up the following Tag rules:

Default: Shipping Methods tagged ‘free\_delivery’ are not visible.\
For Customers tagged ‘free\_delivery’, Shipping Methods tagged ‘free\_delivery’ are visible.

![](../../.gitbook/assets/freedelivtags.jpg)

**Bingo!  A customer who has registered with you as elderly and lives close by will have these options at checkout:**

![Tagged customer view at checkout](https://lh3.googleusercontent.com/eq2nJ6QucE4SZCtLsrat2veXR2k8uxxdm5BPd7oyWc8EhT7wo8gMBEzKVGt07JqenrR8OOt5VmNbBotrnXEx8\_a9B8Ok3sdgOAlLWhutrgkMG42npDpiSnJl9G8xiBOIfT-MIs6d)

Everyone else will only be able to see your standard shipping methods:

![View of non-tagged customer's Shipping Options at checkout](https://lh4.googleusercontent.com/MHj98plQ6gLA6GCdl5g3p9S5wZccyaLwDb2PaHo1PVUE5iDXfcUTGlVZJrhL2TXKELmFkwdVt2iAMA2RxIFzsfv33Y60nh1OmQ4QunNfhPEYSCtvsYhkKCa511tvJrsr-UBdmww5)

{% hint style="success" %}
Add a comment to your standard delivery methods (in the ‘Description box’) to inform elderly and vulnerable customers on how to get in touch and be eligible for free delivery in the future.
{% endhint %}

## **You might also like to: Add a message to your customers on your shop Notice page.**

Don’t forget to edit your ‘[Shopfront Message](../../basic-features/enterprise-profile/enterprise-settings.md#shop-preferences)’ (found from **Enterprises -> Settings -> Shop Preferences**) to invite new elderly/vulnerable/keyworker customers to contact you so they can be prioritised.

![Admin view](https://lh5.googleusercontent.com/Wg3e\_guD-P5zbZE1oa6OFb36YU-csR35WpZD9Hxn0cT3O05jXDDihtHH2EL9CIP7atYsXXK3va9gUSvyfNka\_ovDGDtSG2uRqreA2nW4cp8IjCnL3eodEv12iZ5QkA2eRIGaCkzD)

![](../../.gitbook/assets/notices2.jpg)
