# Subscriptions - FAQs

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

### **If I remove an Order Cycle from a schedule when it already has open subscription orders attached to it, what will happen to those orders? Will those subscriptions get deleted?**

Those orders will remain open. At the close of the order cycle the subscription orders will be processed like normal subscription orders. If you wanted to cancel all subscription orders that were attached to that order cycle you would need to [delete each subscription order individually](subscriptions-creating-and-managing-orders.md#edit-a-customers-subscription).

### **If I add a new subscription in the middle of an open order cycle, will there be a subscription generated for that customer?**

Yes, if you create a subscription while there is an open order cycle in that schedule, an order will be generated for that customer. If you don't want the subscription to apply to the current open order cycle you'll need to set the start date of the subscription to be after the close of that order cycle.

### **What if part of the stock is available but not all? Which customers get the limited stock?**

In the case that a product’s In Stock? value is not adequate to meet all subscription orders, the limited stock won’t be allocated evenly across customers, instead it will fulfill customers orders with available stock until it runs out. Some customers will receive their full order, others will receive none.

### **What if I change the subscription while it’s ‘open’?**

It is not possible to _**add items**_ to the core subscription order while an order cycle part of the subscription's schedule is open.  Any additional products will need to be added when order cycles are closed \(ie. for weekly subscriptions assigned to the schedule 'Weekly', in the period of time between order cycle A closing and order cycle B opening, where both A and B belong to the schedule 'Weekly'\).

If you edit a customer's core subscription to _**remove products**_ while an order cycle is open then this change will impact the order placed in the current order cycle. 

### **What if there’s limited stock, but then a customer cancels their order, will this stock get automatically allocated to other subscribers who wanted that product but couldn’t have it due to insufficient stock?**

No, if a customer cancels their subscription order or removes a product from it, that stock will be returned to the products's In Stock? value. It won't automatically be allocated to other customers, but you could now add this stock to another customer's order manually by [editing their order](../orders/view-orders.md#editing-an-order).

### **Can I or the customer edit an order which has been placed by subscription system?**

This depends on whether you would like to add or remove products:

* As enterprise manager you will be able to **remove products** \(or cancel an order\) which has been placed by the subscription system via the OFN admin panel in the [normal way](../orders/view-orders.md#editing-an-order).
* As enterprise manager, if you **add products** to an order placed by the subscription system via the [OFN admin panel](../orders/view-orders.md#editing-an-order) then this will [invoke a second payment](../orders/refunds-and-adjusting-payments.md#collecting-additional-payments) which will not be automatically processed at the end of the order cycle.
* If you enable customers to be able to [edit or cancel orders](../enterprise-profile/enterprise-settings.md#shop-preferences) while the order cycle is open then they will be able to remove items from their subscription order.  To add items they will need to generate a second order and visit the checkout as normal.



