# Orders

You can interact with orders via two pages within the OFN, the Lisitng Orders page, and the Bulk Order Managment page. The features of these two pages will be discussed below.

## Listing orders

The listing order page shows a list view of all orders placed through your shop\(s\). From here you can access details of individual orders, edit orders and track the status of their payment and shipping. For details of how to create a new order see [here](/create-an-order.md).

The page has filters which allow you to select which orders you want to view. You can filter by date, status or the email and name of the customer.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Listing-Orders1.png "Listing orders page")

**Distributor:**This is the enterprise whose shop the order was placed through

**Completed at:**This is the date that the order was placed.

**Number:**This is an arbitrarily assigned order number. An exclamation mark symbol will show if the customer included a note with their order at checkout. Hover you mouse above the exclamation mark to view the note.

**State:**

* Complete- the customer has finished checkout
* Cancelled- if admin edits the order and chooses to ‘cancel it’
* Cart- The customer is in the process of shopping, but hasn’t checked out

**Payment State:**

* Balance Due- if it’s cash, or bank transfer or eftpos, then the order will be ‘balance due’ by default, until admin indicates that payment has been received.
* Paid- If paying by paypal or pin payment then this will automatically update to ‘paid’ after payment. If payment has been manually indicated as having occurred, state will also be ‘paid’.
* Credit Owed- If someone has paid for their order, but then you edit their order, and remove an item, the cost of that item becomes ‘credit owed’.

**Shipment state:**

* Pending- When the payment state is ‘balance due’ the shipping state will be pending, meaning that until payment is received, shipping should not commence.
* Ready- When payment has been received \(paid, or credit owed status\) the shipping state becomes ‘ready’.
* Shipped- When the product has been edited and the ‘ship’ button clicked, the status becomes shipped.

_Note: You cannot set an order to ‘shipped’ unless that order’s Payment State is ‘Paid’._

**Customer email:**The customer’s contact email. A full list of customer emails can be extracted in the ‘mailing list’[report](/reports.md).

**Total:**The total value of the customer’s order

##### Changing the payment and shipping state of an order

On the right hand side of the listing view you can update the payment/shipping state of an order.

Click on the tick icon to indicate that payment has been received \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Tick.png "paid")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Tick.png)\).  
Click on the road icon to indicate that the order has been shipped \(![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Shipped.png "Shipped button")\).  
Click on the edit icon \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Edit-order.png "Edit order button")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Edit-order.png)\) to edit an order and view more detailed information about it \(discussed below\).

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/tracking-orders.png "Tracking and editing orders")

##### Editing an order

After clicking the edit button on the right hand side of an order \(see image above\) you’ll be taken to a detailed view of the order \(below\). Functionalities within this page will be discussed below.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/View-Order.png "View Order")

**Adding and removing products from an order**

You can select a product to add to the order. To remove a product click the rubbish bin icon on the right hand side of a product. You can also change the quantity ordered. Remember to click the **update and recalculate fees **button to save changes.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Order-actions.png "Order actions")

**Resend confirmation email**

If you make changes to a customer’s order, you might wish to resend an updated order confirmation email to the customer.

**Print Invoice**

Clicking this will give you the option to print an invoice as a PDF or by sending to a printer.

**Send invoice**

To send an invoice to the customer, click the ‘send invoice’ button. This will email the customer with an attached PDF file. Invoice layout shown below.

**Cancel an order**

Click the cancel button to cancel an order.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Invoice-example.png "Invoice example")

**Mark an order as paid**

To mark an order as paid, click the tick icon on the listing order page. Or click on ‘Payments’ in the menu on the right and then click the tick icon \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Tick.png "paid")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Tick.png)\).

**Mark an order as shipped**

After payment has been received the Ship button will be visible at the top of the page \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Ship.png "Ship")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Ship.png)\). Click this to record that shipment has occurred.

**View customer details**

Clicking on customer details \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Customer-details.png "customer details")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Customer-details.png)\) in the right hand menu will take you to a complete view of the customer’s details.

**Add or subtract from the order balance**

Clicking on adjustments \([![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Adjustments.png "Adjustments")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Adjustments.png)\). From here you can remove fees that are already on an order, or add/subtract from the order total by clicking on + New Adjustment. You also have the capacity to select the tax setting of the adjustment. Remember, for a fee to include tax, the enterprise must be set to charge tax in its profile settings.

##### Customer’s View

Your customers can view a list of their orders when they login to the OFN, and click on their account \(see below\).

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Account-login.png "Customer account login")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Account-login.png)

Here your customers will be able to see the past orders and payments as well as a running balance at your shop. This should be kept up to date so customers can view an accurate balance.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Orders.png "Customer Account")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Orders.png)

## Bulk order management

While the listing view shows you orders, and details about who the customer is and when the order was placed etc, the bulk order management page shows you all items that were purchased in your orders. In bulk order management you can view all items ordered and make changes to the quantities of products ordered, or to delete certain products from orders. This functionality is useful for adjusting orders when there are stock shortages and you need to allocate a limited amount of stock.

Access Bulk Oder Management by clicking **Orders **in the blue horizontal menu, and **Bulk Order Management **in the horizontal green menu.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Bulk-Order-Management.png "Accessing bulk order management")

Within Bulk Order Management, you can apply filters, so that only the orders that you are interested in will display.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Filter-Bulk-order-man.png "Filtering within bulk order management")

**Start Date and End Date:** You can filter to display all orders that were placed within a given window of time.

**Producer:** You can filter for a given producer. This can narrow down the display, if you’re only interested in one product, supplied by one proudcer.

**Hub: **You can filter according to the hub at which the order was placed.

**Order Cycle:** Perhaps the most useful filter, the order cycle filter, will display only those orders which were placed within a selected order cycle.

**Quick Search:** Before or after applying filters, you can narrow your search down even further by searching for a key word. This could be a name, product, hub, producer, date, order number…

**Actions: **You can select the checkboxes of multiple orders, to perform a function to all of them, such as delete.

**Columns:** You can select which fields you do or do not want to be displayed \(see below\)

[![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Bulk-Order-Man-Columns.png "Bulk Order Management Columns")](https://openfoodnetwork.org/wp-content/uploads/2015/05/Bulk-Order-Man-Columns.png)

You can also sort the rows according to the contents of a column. For example, if you click on the Order Date column title, the table will be arranged in chronological order, according to the value in this field. Clicking the Name column heading will arrange the table in alphabetical order of the customer’s name.

\*Note: The price column lists prices exclusive of fees, but will include GST if the product is set as GST inclusive. Fees will re-calculate if you edit orders.

### Examples of using Bulk Order Management:

#### Example 1: You have a stock shortage, and must reduce customer order quantities for a certain product.

In your current order cycle, customers placed orders for 20kg of tomatoes. Unfortunately there was a storm, and you were only able to harvest 10kg. You need to identify all customers who ordered tomatoes, and half their orders for tomatoes.

This can be done in bulk order management, as follows:

1. You would filter according to the date range, or order cycle.
2. Search for ‘tomatoes’. All orders for tomatoes within the date range/order cycle you selected will now display.
3. Click on the product ‘Tomatoes’ in the Product:Unit column.
4. A box will appear at the top of the page, showing the total quantity ordered \(across the date range/order cycle you’ve selected\).

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/BOM-1.png "Bulk Order Management")

You can then adjust the quantity of each unique order in the Quantity column. The Total Quantitiy Ordered in the box at the top will update automatically as you adjust orders, in this case going down, as you reduce each order for the tomatoes.

You could also then see the emails of these customers, and send them an alert._An alert is not automatically generated when adjustments are made in bulk order management._

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/BOM-2.png "Bulk Order Management")

##### **The ‘Shared Resource’ checkbox**

In the screenshot above you will see a checkbox called ‘shared resource’ in the top right hand corner of the blue, producer order totals box. When you select this checkbox, the total displayed will be inlcusive of all product variants that fall under the master product. By not checking it, you can see the total for a single product variant. In the example below, you can see that when the shared resource box is selected, the total includes orders for both my 1kg apple variant and my 3kg apple variant. So I know that in total, I need 5kg of apples. If I just want to know how many 3kg bags to pack, I can uncheck the shared resource box, and click on the 3kg variant in the Product:Unit column.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Shared-Resource.png "Shared Resource checked")

#### Example 2: Updating the final weight of products.

When selling indivisible products such as legs of lamb, or whole pumpkins, you may not know the final weight and price of the product until after the customer has placed their order. You can use Bulk Order Management to update the item’s exact weight once you have the product in front of you.

Check out Pricing irregular, indivisible meat items for more information about pricing products such as this.

We’ll use an example of a leg of lamb to illustrate. In this case the producer charges all customers for a 2kg leg of lamb, and then adjusts their orders after slaughter, when he knows the exact weight of the product assigned to each customer. To make such adjustments the producer would do the following:

1. Filter for the order cycle or date range of interest.
2. Search for the leg of lamb product to view all customer orders for the product.
3. Make the
   **Weight/Volume**
   and
   **Price**
   columns visible.
4. Enter the actual weight of the leg of lamb that each customer will receive in the weight/volume column. The price will automatically recalculate based on this weight.
5. Click update.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Meat-BOMM.png "Bulk Order Management example")

_Have a suggestion for how we could improve this feature? Send us an email or join the conversation on our community forum._

