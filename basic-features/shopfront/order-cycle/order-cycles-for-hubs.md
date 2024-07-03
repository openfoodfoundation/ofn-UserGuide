# Order Cycles (for Hubs)

{% hint style="warning" %}
Read on if you selected the Enterprise Profile '[Producer or Non Producer Hub](../../../your-quick-start-on-ofn-given-who-you-are.md#hub)'.&#x20;

Visit [this page](order-cycles-for-producers.md) if you registered as a '[Producer Shop](../../../your-quick-start-on-ofn-given-who-you-are.md#shop)' and want to set up an order cycle for your shop front.
{% endhint %}

You open your shop by creating an Order Cycle. When you create an order cycle you select when your shop is open (from and until), which products will go into the shop, and any fees that you'll apply.

**Why Order Cycles?**  \
Some hubs may wish to have an online store which is perpetually open and to fulfil orders on a one by one basis, as they are received. However, many hubs operate on a periodic ordering system which allows them to process orders in bulk, making their production, packing and distribution activities more efficient (and reducing associated overhead costs).&#x20;

For example, an order cycle might be open for two weeks. At the end of the fortnight, all orders will be packed and delivered at the same time on the following Wednesday. Once this batch of orders has been delivered, a new order cycle may reopen.

## Viewing Order Cycles

You can create an order cycle, and view previous order cycles by clicking on **Manage Order Cycles** on your [dashboard](../../dashboard.md).

![](<../../../.gitbook/assets/dashboard order cycle.jpg>)

Or from the horizontal menu at the top of the page.

![](<../../../.gitbook/assets/oc list.jpg>)

{% hint style="warning" %}
You will not be able to publish a live order cycle until you have at least one [payment](../payment-methods.md) and [shipping](../shipping-methods.md) method set up for your enterprise.
{% endhint %}

## Create a New Order Cycle

The first step is to select a coordinator for your order cycle. Only the enterprise who coordinates an order cycle has permission to modify and manage **all** aspects of the order cycle. \
Other enterprises involved in an order cycle (as suppliers or distributors only) will have restricted access. \
For more information on cross-enterprise management in the context of order cycles, [click here](permissions-in-multi-enterprise-order-cycles.md).

![](<../../../.gitbook/assets/oc cord.jpg>)

Once the order cycle coordinator has been chosen, the process of setting up your cycle can be broken down into four steps:

### 1) General Settings

![](<../../../.gitbook/assets/general settings Oc.jpg>)

**Name (**_**required**_**):** Give the order cycle a name which is meaningful to you. We recommend that you follow a consistent naming protocol e.g FoodHub\_Week27\_2014. We also recommend that you include the name of your hub in the order cycle name, so that OFN support can identify your order cycles if you need assistance.

**Orders Open at:** This is the date and time when your OFN store will be open, visible and able to accept orders from customers.

**Orders Close:** This is the date and time when your OFN store will close and stop accepting orders. If you intend to have an order cycle which is continuously open, select a close date well into the future.

**Add Coordinator Fee:** As a hub, the coordinator is most likely you. Here you can apply your Enterprise Fee which acts as the markup. The fee will be calculated according to the calculator selected in [Enterprise Fees](../enterprise-fees.md). You can only apply an enterprise fee which has previously been created.

### 2) Incoming Products

![](<../../../.gitbook/assets/oc incoming.jpg>)

On this page you can select the producers, and their produce, which will be available in this order cycle. In the dropdown menu you will see all producers who have granted you permission to add their produce to your order cycle (See [Enterprise Permissions](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) section). \
After selecting a supplier and clicking **Add Supplier**, all of the products associated with that supplier will be visible. Check those products you wish to add to the store, or click **select all.**&#x20;

{% hint style="info" %}
Products which are out of stock (i.e. their 'in stock' value is zero) are shown in this list but if added to an order cycle they will not appear on your shop front. It is always good to double check stock levels.
{% endhint %}

The **Receival Details** field is optional.  Information added to this field will automatically added to any email sent to producers at the end of an order cycle (after clicking 'Notify Producers').  It might be a good idea to include an exact delivery address for produce prior to distribution to customers here.

The **Add Fee** button in this section, at the end of each producer's entry in the table, allows you to add different [enterprise fees](../enterprise-fees.md) to different suppliers. For example, transporting flour or heavy goods to customers may be more expensive for a hub than salad.  Hence, a hub can, in a transparent manner, add a slightly higher enterprise fee to all goods supplied by the flour miller than the salad farmer.

Select the name of the enterprise which sets the fee in the first dropdown box, then click the name of the enterprise fee in the second dropdown box. &#x20;

![Apply enterprise fee to incoming supplier](<../../../.gitbook/assets/ent fee incoming oc.jpg>)

{% hint style="warning" %}
This fee will be applied to all of 'User guide demo producer’s products which are purchased. The fee is calculated according to the fee calculator which was selected when the [Enterprise Fee](../enterprise-fees.md) was created.
{% endhint %}

### 3) Outgoing Products

Here you can select one or more hub-distributors. All hubs chosen to be a distributor in this order cycle will have an open shop front for the duration of the order cycle.\
In a **simple model**, only one hub is listed as the sole distributor for the order cycle. Select the hub, and check the box 'Select all' to add all incoming products to the shop front. \
For more flexibility, the same order cycle may have **multiple hub distributors**.  In this case you may wish to select a different subset of the available incoming products for each distributor, and/or add different delivery dates for each.

![](<../../../.gitbook/assets/oc outgoing.jpg>)

The **Tags** column is where you can tag your order cycles to customise whether they are visible/invisible to certain customers. See [tags and tag rules](../customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) for more information.

The **‘Ready for (i.e. Date/Time)’ (**_**required**_**):** This box tells the customer when their order will be ready for either collection or delivery. If your order cycle is a perpetual one, which fulfils orders on an individual basis rather than in bulk, you should enter something like ‘Two days after order is received’. The example below shows how a customer can toggle between different order cycles to select the date which suits them best.

![](../../../.gitbook/assets/multipleoc3.jpg)

{% hint style="info" %}
If you operate with a continuously open shop front (i.e. you set your 'order cycle close date' further than 3 months away) then the blue 'Ready For' text box on your shop front (shown in above screenshot) will read 'Orders are currently open'.
{% endhint %}

**Add Fee:** Again, a previously created enterprise fee can be assigned to this distributor.  For simple models (with one hub distributor, who also is the coordinator of the order cycle) adding a fee at this stage is the same as adding a 'Coordinator Fee' (it will apply to all products).\
For complex models, the coordinator may wish to add different fees to all products sold though each distributor.  The best place to implement this functionality is here.

### 4) Checkout Options

Your enterprise may have several order cycles open at once, each with a different collection/delivery options or payment methods.  For example, you may wish to have two concurrent order cycles:

1. Products available for collection at a physical location at a specific time and date.  You will be there in person and so can offer cash on collection as a payment method for this.
2. Products which can be sent my courier or through the post (ie. non perishable goods).  You would prefer that customers pay for these items before they are dispatched and so only wish to allow the payment option of 'card payment' to be visible.

In order to do this, your enterprise will need to have both collection and delivery shipping methods set up, plus two different payment methods (cash on collection and a card payment).

You can then assign the shipping and payment methods you wish to use for specific order cycles (and hence the products they contain) during the fourth stage of setting up an order cycle simply by completing the check boxes:

<figure><img src="../../../.gitbook/assets/oc checkout options.jpg" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
By default the 'Select all' box will be checked.
{% endhint %}

The options will appear to the customer like this as they go through checkout:

![](<../../../.gitbook/assets/shipping checkout multi.jpg>)

And all the relevant information relating the shipping/delivery and payment will be summarised in the customer’s order confirmation email:

![collection details message](<../../../.gitbook/assets/customer order confirm email.jpg>)



### Open the shopfront

Click **Save** to schedule the order cycle. If the opening date has already passed, your shop is instantly open! If you are not ready to open right away, enter dates in the future, which you can change later.&#x20;

For periodic, repetitive order cycles, you can copy an existing order cycle and change the dates to make the process quicker. Click the button with two sheets of paper to the right of the table as highlighted below:

![](<../../../.gitbook/assets/oc list copy.jpg>)

Order cycles will display as green when they are active, yellow when scheduled for a future date, and grey when they have closed. If an order cycle closed over one month ago, it will no longer display on this list. To view all of your past order cycles click **show 30 more days** or **show 90 more days** at the bottom of the list.

{% hint style="warning" %}
Re-opening an order cycle to re-open a shopfront can cause confusion at customer checkout, see the warning shown below. For periodically opening shopfronts, duplicate or create new order cycles each time you open the shop rather than editing the open and close dates of one order cycle.
{% endhint %}

Customers will be advised when they have already ordered in an order cycle, even if the order cycle was closed for some time before being reopened:

![](<../../../.gitbook/assets/pop up in checkout.jpg>)

## **‘Notify Producers’ Button**

By using this button at the top of the page, all the Producers linked to the order cycle will receive an email containing a list of the products ordered for that particular order cycle thus far. &#x20;

![](<../../../.gitbook/assets/notify producers.jpg>)

When the Notify Producers button is selected there will be a confirmation prompt. Once confirmed, an email will be automatically sent to all relevant Producers. The email will include Delivery instructions (if this field is completed in the incoming products section) as well as the following product information:

* SKUs (if relevant)
* Name of Supplier
* Product name&#x20;
* Quantity ordered
* Price per unit
* Subtotal per product
* Included Tax (if relevant)\


### Setting up automatic producer notifications

If you would like the producer emails to be automatically sent when an order cycle closes, you can do this from the 'Advanced settings' menu in the edit order cycle screen:

![](<../../../.gitbook/assets/advanced settings.jpg>)

From the menu that appears, select the checkbox for 'automatic notifications' and click 'save and reload page' to save your changes:

![](<../../../.gitbook/assets/auto notify.jpg>)

To also show **customer names** in these reports, for example to help your producers to pack items by customer, ensure you have the setting 'customer names in reports' enabled from the shop preferences menu of your enterprise settings:

![](<../../../.gitbook/assets/names in reports.jpg>)

{% hint style="info" %}
By default, 'customer names in reports' is disabled. Ensure you have this enabled for your producers if you would like them to receive reports grouped by customer to help them pack their orders.&#x20;
{% endhint %}

Once you have the automatic notifications set up for an order cycle, your producers will automatically be sent an email after the order cycle closes. Enabling 'customer names in reports' will help them to pack the orders by customer.

## Producer / Supplier Reports

If your Order Cycle includes products from linked Producers / Suppliers they will be able to log in to their OFN account and view [reports](../../reports/) about the Order Cycle. By default they will not be able to see any Customer Details in these reports. If you would like your suppliers to access Customer Names in their reports, you can adjust these settings in Shop Preferences in your [Enterprise Settings](../../enterprise-profile/enterprise-settings.md).
