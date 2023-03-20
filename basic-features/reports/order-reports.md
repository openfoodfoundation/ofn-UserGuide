# Order Reports

## Orders and Distributors Report

{% hint style="success" %}
This report is a useful way to view customer orders as they are placed in more detail than on the [Order](../orders/view-orders.md) list.
{% endhint %}

The Data fields you can see in this report are:

* Date & time the order was placed along with order ID
* Shipping method (and cost), payment method, customer notes
* Customer name, email, phone number, city (but not full address)
* For each product within an order, there is the name of the product, variant name, quantity (and Max quantity for bulk order items), cost
* Hub (distributor) address

![Orders and Distributors Report](<../../.gitbook/assets/orders and distributors.jpg>)

{% hint style="info" %}
Filter by date and time to enable swift download.
{% endhint %}

## Orders and Fulfillment Reports

Under the Orders and Fulfillment Reports you will find four options: Order Cycle Supplier Totals, Order Cycle Supplier Totals by Distributor, Order Cycle Distributor Totals by Supplier and Order Cycle Customer Totals.

### Order Cycle Supplier Totals&#x20;

{% hint style="success" %}
As a **producer who supplies one or more hubs** these three reports are a great way to keep track of orders of your products which coming in **while an order cycle is open.**&#x20;
{% endhint %}

Unless you are also the coordinator or distributor of the order cycle these orders will not appear in your list of [Orders](../orders/view-orders.md) but you may want to start planning your baking/picking before you receive the [supplier notification email](../shopfront/order-cycle/order-cycles-for-hubs.md#notify-producers-button) from the distributing hub.

A summary of the data found in each report is below:

| Report            | OC Sup Tots | OC Sup Tot by Dist | OC Dist Tot by Sup |
| ----------------- | ----------- | ------------------ | ------------------ |
| Producer          | Y           | Y                  | Y                  |
| Hub               | N           | Y                  | Y                  |
| Product           | Y           | Y                  | Y                  |
| Variant           | Y           | Y                  | Y                  |
| Amount            | Y           | Y                  | Y                  |
| Tot Units         | Y           | N                  | N                  |
| Current unit Cost | Y           | Y                  | Y                  |
| Total Cost        | Y           | Y                  | Y                  |
| Status            | Y           | N                  | N                  |
| Shipping Method   | Y           | Y                  | Y                  |
| Tot shipping cost | N           | N                  | Y                  |

{% hint style="warning" %}
Note that the Total Cost is not a simple multiple of Current cost per unit and amount. &#x20;

* The current cost per unit may vary over the time frame selected. &#x20;
* The value recorded in these reports is the current cost per unit at the time of the last order.
* The Total Cost is a sum of product costs at the time when each item was purchased.
{% endhint %}

![Order Cycle Supplier Totals](<../../.gitbook/assets/OC supplier totals.jpg>)

![Order Cycle Supplier Totals by Distributor](<../../.gitbook/assets/OC supplier totals by distributor.jpg>)

![Order Cycle Distributor Totals by Supplier](<../../.gitbook/assets/OC distributor totals by supplier.jpg>)

{% hint style="success" %}
These reports are handy for calculating the amount to reimburse a producer for items supplied
{% endhint %}

### Order Cycle Customer Totals

{% hint style="success" %}
Useful for:

* Fulfilling orders on a individual basis&#x20;
* Preparing individual orders in bulk
{% endhint %}

This report which contains the most data:

* Date & time the order was placed along with order ID
* Customer name, email, phone number, billing and shipping addresses
* For each product within an order, there is the name of the product, variant name, quantity, cost, price paid by the customer (item cost + fees), a break down of fees (Enterprise, payment method and shipping method fee associated with each product), producer
* Hub name.
* Payment Method and status (ie. paid, unpaid)
* Shipping Method, Delivery or Pick up

{% hint style="info" %}
The Shipping Address displayed for an order where the chosen shipping method is 'pick up' will be the address of the distributing hub.
{% endhint %}

The screenshot below shows the information contained in an Order Cycle Customer Totals report.&#x20;

![Order Cycle Customer Totals](<../../.gitbook/assets/OC customer totals.jpg>)
