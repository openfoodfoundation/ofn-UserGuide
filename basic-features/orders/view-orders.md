# Manage Orders

Within the admin interface there are two places where orders can be viewed and modified (if necessary):

1. the [Orders](view-orders.md#listing-orders) page itself,
2. the [Bulk Order Management](view-orders.md#bulk-order-management) page.

The features of both these two pages are discussed below.

## Listing orders

The listing orders page shows a list view of all orders placed through your shop(s). From here you can access details of individual orders, edit orders and track the status of their payment and shipping. For details of how to create a new order manually for your customer see [here](create-orders-manually.md).

The page has filters which allow you to select which orders you want to view. You can filter by date, status or the email and name of the customer.

![](<../../.gitbook/assets/listing orders.jpg>)

**Distributor:** This is the enterprise through who's shop the order was placed.

**Completed at:** This is the date that the order was placed.

**Number:** This is an arbitrarily assigned order number. An exclamation mark symbol with with word 'Note' to the left of it will show if the customer included a comment with their order at checkout. Hover your mouse above the exclamation mark to view the comment.

**State:**

* Complete: The customer has finished checkout.
* Cancelled: If a manager of an enterprise or a customer chose to ‘cancel' it.
* Cart: The customer is in the process of shopping, but hasn’t checked out yet.

**Payment State:**

* Balance Due: If it’s cash, or bank transfer or eftpos (i.e. all non automated payments), then the order will be ‘balance due’ by default, until admin members of the distributing enterprise manually mark that the payment has been received, at which point the payment state will change to 'paid'.

![](<../../.gitbook/assets/balance due.jpg>)

* Paid: For automated payments (PayPal, Stripe SCA, PIN for instance), the payment portal will automatically mark an order as 'paid' when it has been processed. \
  Non-automated payments (cash, bank transfer etc.) will also be marked as 'paid' when the payment has been marked as captured manually (see [Changing the Payment and Shipment state of an order](view-orders.md#payment-and-shipment-state)).&#x20;
* Credit Owed: If someone has paid for their order, but then you edit their order, and remove an item, the cost of that item becomes ‘credit owed’.

![](<../../.gitbook/assets/credit owed.jpg>)

**Shipment state:**

* Pending: When the payment state is ‘balance due’ the shipping state will be pending, meaning that until payment is received, shipping should not commence.
* Ready: When payment has been received ('paid', or 'credit owed' status) the shipping state becomes ‘ready’.
* Shipped: After delivery or collection, an order can be manually marked as 'shipped' by the manager of the enterprise (see [Changing the Payment and Shipment state of an order](view-orders.md#payment-and-shipment-state)).

{% hint style="warning" %}
You can ONLY manually update an order to 'shipped' if the payment state is 'paid' or 'credit owed'.
{% endhint %}

**Customer email:** The customer’s contact email.&#x20;

**Customer name:** written in the format of 'Surname-comma-first name'

**Total:** The total value of the customer’s order.

### **Changing the Payment and Shipment state of an order** <a href="#payment-and-shipment-state" id="payment-and-shipment-state"></a>

Next to each order in the Order list are two icons. Clicking on the edit icon (a pencil and paper symbol) will open up details of the order so that you can review or edit the order details. Below the edit icon will be one of two icons. These icons show the payment and shipment status, and can be clicked to change the status. If a payment has not been received, the icon will show a tick which can be clicked to capture the payment. If payment has been received, the icon will be a road, which can be clicked to mark the order as delivered.

* Clicking on the tick icon (highlighted in red below) will change the Payment State to **Paid**.&#x20;
* Clicking on the road icon (highlighted in green below) will change the Shipment state to **Shipped**.

![](<../../.gitbook/assets/orders capture.jpg>)

{% hint style="info" %}
The payment and shipping status of an order can also be updated when editing the order (see [below](view-orders.md#editing-an-order)).
{% endhint %}

#### Capturing a Payment

Capturing a payment will mark it as received. This is helpful if customers do not pay when they order. When you receive cash or a bank transfer from the customer, you can then go in to the Order Listing and capture the payment. To quickly capture a payment as received, or mark that an order has been shipped, you can click on the tick or road icons to the right of the order in the Order List. &#x20;

Note that this will capture the full amount of the order as paid. if you want to review the order details before capturing a payment, you can select the edit icon to the right of the Order you wish to review. In the Order Details screen, click on Payments to see the Balance owing and Payment Status for this order. From here you can click on the tick to capture the payment. Once captured, the Payment Status will change to Completed.

![](<../../.gitbook/assets/payments capt.jpg>)

&#x20;&#x20;

{% hint style="danger" %}
When a shop or hub manager updates the 'Shipment state' to 'shipped' _**this will automatically send the customer an email**_ to say that their products have been shipped, irrespective of the shipping method. Hence it can cause confusion for orders due to be collected (rather than shipped).\
Another source of potential confusion to be aware of is when customers pay for an order on collection. Updating the payment (and then shipping) status of the order after the goods have been collected will send an email to the customer, even though they have their goods in practice.
{% endhint %}

### **Editing an order**

To the right of an order you will see a pen and paper icon.  Click on this to access the order management page where you can edit, modify and cancel an order.

This is what the order management page looks like:

![](<../../.gitbook/assets/edit order.jpg>)

#### **Adding and removing products from an order**

You can add a product to the order by selecting the variant you require from a drop down list of those available (at least 3 letters must be typed in to the field box 'Select Variant' for list of options to appear). To remove a product from an order click the rubbish bin icon on the right hand side of the product. You can also change the quantity of each item ordered. Remember to click the **update and recalculate fees** button to save changes (this will also update enterprise, shipping and payment method fees accordingly, where appropriate).

**Changing the Shipping Method**

A customer may contact you and ask to have their groceries delivered rather than collect. You can edit the shipping method assigned to the order by selecting the edit symbol to the right of the shipping method:

![](<../../.gitbook/assets/edit shipping 1.jpg>)

You then have access to all available shipping methods. Select the one your customer wishes to change to. &#x20;

![](<../../.gitbook/assets/edit shipping 2.jpg>)

To save changes select the 'tick' icon to the right hand side. To discard, select the 'cross'.

**Adding tracking or a note to an order**

If the order will be sent by courier and you have tracking details then you can add them to the order by selecting the 'pen and paper' symbol to the right of 'Tracking details' (highlighted in red below).

Customers may add notes to orders at checkout, such as where to leave a parcel if they are not going to be home. From time to time they may forget to add the note at checkout and then contact you later with this type of information. You can add the note in retrospect by selecting the pen and paper symbol to the right of Notes (highlighted in green below).

<figure><img src="../../.gitbook/assets/tracking or note.jpg" alt=""><figcaption></figcaption></figure>

### **Additional options available under 'Actions'**

![](<../../.gitbook/assets/actions (1).jpg>)

* **Resend Confirmation**: If you have edited a customer's order, you may wish to resend them an updated order confirmation email.
* **Send Invoice**: This will automatically send the customer an [invoice](../reports/view-orders.md) (in .pdf format) by email. Sending an invoice is purely for record keeping purposes, and does not facilitate payment.&#x20;
* **Print Invoice:** This will generate the[ invoice](../reports/view-orders.md) in the form of a pdf for printing.
* **Cancel Order:** Cancel the order. It is important to process any refunds or adjustments to an order before cancelling it. **A cancelled order can not be edited or refunded.**

{% hint style="info" %}
More information can be found about OFN [invoices](../reports/view-orders.md) here.
{% endhint %}

#### **View customer details**

Customer information (email, billing, shipping addresses and phone numbers) are accessible from the menu on the right of the page:

![](<../../.gitbook/assets/customer details.jpg>)

#### **Modify an Order or Record Partial Payment**

Click on 'Adjustments' in the right hand menu (screen shot above).  On this page you can add or subtract from the order total by selecting the **+ New Adjustment button**.

![](<../../.gitbook/assets/adjustments 1 (1).jpg>)

You may wish to use this functionality to:

* grant a discount on an order if a product is damaged
* deduct credit owed to the customer from their total balance
* refund a customer&#x20;
* record a partial payment
* see [Refunding and Adjusting Payments](refunds-and-adjusting-payments.md) for more information about making adjustments to orders

<figure><img src="../../.gitbook/assets/adjustments 2.jpg" alt=""><figcaption></figcaption></figure>

## Bulk order management

We have learned above that the [Listing Orders](view-orders.md#listing-orders) tab presents a table of the **orders per customer**. The Bulk Order Management page, on the other hand, details all the products that were purchased in your orders. This functionality is useful for modifying multiple orders at once that may contain the same product (quantity change, product out of stock etc). The page looks like:

![](<../../.gitbook/assets/bulk order 1.jpg>)

**Start/End Date:** You can filter to display all orders that were placed within a given window of time.

**Producer:** You can filter for a given producer. This can narrow down the display, if you’re only interested in one product, supplied by one producer.

**Shop:** You can filter according to the shop at which the order was placed.

**Order Cycle:** Perhaps the most useful filter, the order cycle filter, will display only those orders which were placed within a selected order cycle.

**Actions:** You can select the check boxes of multiple orders (left hand column), to perform the same function to all of them, such as delete.

**Columns:** You can select which fields you do or do not want to be displayed in the table:

![](<../../.gitbook/assets/bulk columns.jpg>)

{% hint style="success" %}
Rows ('Name', 'Producer', 'Product: Unit') can be sorted according to their content by clicking on the relevant column heading: one click for sorting A-Z, two clicks for the reverse (Z-A).
{% endhint %}

{% hint style="warning" %}
The **Price** column indicates price of an item including tax but excluding fees (enterprise, shipping or payment method fees).  Fees are recalculated each time an order is modified.
{% endhint %}

### Examples of using Bulk Order Management:

#### Example 1: You have a stock shortage, and must reduce customer order quantities for a certain product.

_In your current order cycle, customers placed orders for 5kg of beef tomatoes. Unfortunately there was a storm, and you were only able to harvest 2kg. You need to identify all customers who ordered tomatoes, and half their orders for tomatoes._

This can be done in bulk order management, as follows:

1. Filter according to the date range, or current order cycle.
2. Search for ‘tomatoes’. All orders for tomatoes within the date range/order cycle you selected will now display.
3. Click on the product ‘Tomatoes’ in the Product:Unit column.
4. A box will appear at the top of the page, showing the total quantity ordered (across the date range/order cycle you’ve selected).

![](<../../.gitbook/assets/beef tom.jpg>)

You can then adjust the quantity (or delete products) of each unique order in the Quantity column. The Total Quantity Ordered in the box at the top will update automatically as you adjust orders. &#x20;

{% hint style="danger" %}
No automated email will be sent to customers after you have adjusted their orders. It is good practice though, to manually do so else the customer may be disappointed on collection/delivery.
{% endhint %}

Here, the amount of tomatoes allocated to each order has been reduced to meet the total available of 2kg:

![](<../../.gitbook/assets/beef tom adjusted.jpg>)

#### Example 2: Updating the final weight of products.

When selling indivisible products such as legs of lamb, or whole pumpkins, you may not know the final weight and price of the product until after the customer has placed their order. (Read more [here](../products-1/pricing-irregular-items-kg.md).) You can use Bulk Order Management to update the item’s exact weight once you have the product in front of you.

For the example of two meat pies which are advertised to be 250g each but actually end up being 275g each for this particular batch:

1. Filter for the order cycle or date range of interest.
2. Search for the desired product
3. Make the **Weight/Volume** and **Price** columns visible.
4. Enter the actual weight of the pies that each customer will receive in the weight/volume column. The price will automatically recalculate based on this weight.
5. Click update.

![](<../../.gitbook/assets/bulk 2.jpg>)

## A **Customer’s view of their order**

Your customers can view a list of their orders when they login to the OFN, and click on their account (see below).

![](../../.gitbook/assets/account-login.png)

Here your customers will be able to see the past orders and payments as well as a running balance at your shop (and any others on OFN where they have placed an order).&#x20;

![](<../../.gitbook/assets/customer account.jpg>)

{% hint style="warning" %}
For non-automated payments (cash, cheque, bank transfer etc) the customer's 'balance' will display as 'owing' until you have [manually recorded the payment](view-orders.md#editing-an-order). \
_**If payments are not updated regularly by a shop/hub manager this can be confusing to your customers as they may have in fact paid but it won't be documented above.**_
{% endhint %}
