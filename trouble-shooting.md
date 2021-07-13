# Trouble shooting

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

{% hint style="success" %}
Always save or update at the end of every change you make. Changes will be lost if you move to a different page without saving.  Sometimes you will not be prompted to save.
{% endhint %}

## It won't 'let me' set up an order cycle

* Do you have an active [payment method](basic-features/shopfront/payment-methods.md) set up for your shop or hub?
* Do you have an active [shipping method](basic-features/shopfront/shipping-methods.md) set up for your shop or hub?
* Are all the [relevant required fields complete](basic-features/shopfront/order-cycle/)? You need to set open and closing times for the order cycle, give it a unique name, and complete the 'Ready for' field box.

## I want to sell whole chickens but don't know the weight of individual birds until day of slaughter.

* This is not a problem! Read [here](basic-features/products-1/pricing-irregular-items-kg.md) for a range of ways the OFN platform has been designed to be flexible to meet the specific needs of food producers.

## I supply 'Farmshop A' with potatoes which cost £1/kg. My potatoes are displaying for sale to customers at £1.20/kg

Farmshop A may need to generate extra revenue from every sale to cover their overhead costs.  They can do this in a number of ways:

* If you set up an [enterprise permission](basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) whereby your business permits Farmshop A to add your products to their inventory then they can modify the prices a customer pays for your products that way. 
* Farmshop A may add an [enterprise fee](basic-features/shopfront/enterprise-fees.md) to your cost price for the potatoes. If this is the case then customers purchasing the items will be able to see a break down of the price they pay by clicking on the pie chart icon to the right of the product price on the shop front.

Good working relationships are key to any sustainable food network. Chat to Farmshop A about how they have organised their sales of your produce \(either in person, over the phone or by email\).

Farmshop A should \(morally\) pay you £1/kg for every kg of potatoes you supply to meet their sales.  Payment of goods \(from distributor to supplier\) is a private arrangement organised outside of the OFN platform.

## I've added new products but they aren't displaying on the shopfront.

Newly added products must be added to an active order cycle before they are visible on a shopfront for customers to purchase.

* If you are _**supplying the goods to a hub**_, then you must get in touch with the person who is coordinating the order cycle in question.  This has to be done externally to the OFN platform \(drop them an email or phone/speak in person\).
* If you are a **Shop**, then you must add the new products to your[ active, open order cycle](basic-features/shopfront/order-cycle/order-cycles-for-producers.md).
* If you are a **Hub**, then:
  * Make sure the new products are added to both the incoming and outgoing sections of the [active order cycle](basic-features/shopfront/order-cycle/order-cycles-for-hubs.md)
  * If the new products are not available for selection to add to either incoming/outgoing sections then check your [inventory settings](basic-features/enterprise-profile/enterprise-settings.md#inventory-settings). You may have to [add the products to your inventory](basic-features/products-1/inventory-tool.md#reviewing-new-products) before they can be added to the shop front.

{% hint style="info" %}
In all cases, check the stock level of the new products. Only items with an **In Stock?** value of 1 or greater or those marked as **Unlimited** will be visible for a customer to purchase.
{% endhint %}

## Not all of my supplier's products are available for me to add to my order cycle.

You may have your [Inventory settings](basic-features/enterprise-profile/enterprise-settings.md#inventory-settings) set to 'New products must be added to my inventory before they can be added to my shopfront'.  
In which case, you must review your product inventory, [add new/hidden products](basic-features/products-1/inventory-tool.md#managing-your-inventory-products) to the inventory for them to be available for selection in the order cycle.

If you are coordinating an order cycle involving multiple suppliers and distributors, some or all of which may use their product inventory to stock their shop fronts, double check all the relevant enterprise permissions have been granted.  Read more [here](basic-features/shopfront/order-cycle/permissions-in-multi-enterprise-order-cycles.md).

## A new Producer has started up nearby but I can't add their products to my hub shop front.

You must seek their permission before you are able to retail the goods they make or supply.  This is done formally on the OFN platform by the new producer through [Enterprise Permissions](basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es.md).

## I have a veg box scheme but would like to allow customers to add extra items, if desired, each week to their order.

**Scenario One:** _The customer purchases the veg box each week through an automated_ [_subscription_](basic-features/subscriptions/) _set up on the OFN platform:_  
Change your [Enterprise Settings](basic-features/enterprise-profile/enterprise-settings.md#shop-preferences)-&gt; Shop Preferences-&gt; Change Orders? to 'Customers can change/cancel orders while order cycle is open'.  
When the order cycle opens, the customer will be sent an automated email to say that their veg box order has been created. They then have until the order cycle closes to login to their OFN account, edit their order and add extra items from your shop front to their basket.

{% hint style="info" %}
The additional items will be processed as a separate order. The customer will be directed to the checkout to pay for these items. Payment for their subscription order will be taken at the end of the order cycle automatically.
{% endhint %}

**Scenario Two:** _The customer purchases a veg box through an external platform._  In this case, perhaps set up a [private shopfront](basic-features/shopfront/private-shopfront.md) which is only visible to customers registered to your external veg box scheme. Use external software or spreadsheets to match additional items brought through the OFN shop front to customers' veg boxes so that you only have to make deliveries once!

## There's been a crop failure and we have fewer tomatoes supplied than we need to meet everyone's order

Not a problem - happens to everyone once in a while!  Read [here](basic-features/orders/view-orders.md#example-1-you-have-a-stock-shortage-and-must-reduce-customer-order-quantities-for-a-certain-product) for steps to adjust all your customers' orders at once.

## A producer is only willing to supply my hub if their orders meet a minimum criteria 

The 'group buy' functionality described [here](basic-features/products-1/group-buy-for-bulk-ordering.md) can be used for this purpose too!

## I can't refund a customer who paid by PayPal

Currently you are not able to issue refunds to customers who purchased goods by PayPal directly through the OFN platform. You will need to visit your business PayPal account and manually make the refund to the customer there.  This is a functionality we hope to develop in the future, should user sufficient users demand it.

{% hint style="warning" %}
If none of these steps help, or there is another problem that you would like advice with, then please contact your[ local OFN support team](local-ofn-organizations-and-contacts.md), who will do their best to get back to you with solutions and help as soon as they can.
{% endhint %}

## How can my customer's edit their orders after they have been placed?

On occasion, a customer may place an order with your food enterprise and then change their mind or remember they forgot to add a few items.  There are a few scenarios:

#### Allow the customer to edit their own orders

In your Enterprise Settings, under the [Shop Preferences](basic-features/enterprise-profile/enterprise-settings.md#shop-preferences) tab, you can enable 'Change Orders'

![](.gitbook/assets/changeorders.jpg)

This will mean customers can:

* Remove items from their basket or cancel their order altogether.
* Increase the quantity of products already in their basket, provided the order was not placed by the subscription system.

{% hint style="warning" %}
Customers will not be able to add additional products to their basket. On doing so they will be taken to the checkout again to pay for these items.  The two orders will appear in your reports one after another if sorted by customer name though, so they can be packed together \(if you wish\) when you are preparing for collection.
{% endhint %}

#### Edit orders on your customer's behalf only

You can add a message to your [Shopfront Notices page](basic-features/enterprise-profile/enterprise-settings.md#shop-preferences) asking customers to contact you by email or phone if they wish to adjust their orders.  Products can be added or removed from orders using the steps outlined [here](basic-features/orders/view-orders.md#editing-an-order).

{% hint style="warning" %}
Note that adding items to an order will invoke the need for [additional payments](basic-features/orders/refunds-and-adjusting-payments.md#collecting-additional-payments) to be collected.
{% endhint %}

#### The order was placed by a subscription.

For information about editing an order placed by the subscription system see:

* [here](basic-features/subscriptions/subscriptions-faqs.md#can-i-or-the-customer-edit-an-order-which-has-been-placed-by-subscription-system) for one off orders
* [here](basic-features/subscriptions/subscriptions-faqs.md#what-if-i-change-the-subscription-while-its-open) for editing the base subscription order.

