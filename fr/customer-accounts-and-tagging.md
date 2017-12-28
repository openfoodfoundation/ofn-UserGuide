# Customer Accounts and Tagging

Any customers who have placed an order in your shop will be listed on the **Customer Page**. Each unique email address used, will be listed as a unique customer. You can also add customer emails to your list by typing the email in the Add New Customer field. Once customers are in your customers page, you will be able to apply tags to them  \(see below\).

## [![](https://openfoodnetwork.org/wp-content/uploads/2015/10/customers.png "customers")](https://openfoodnetwork.org/wp-content/uploads/2015/10/customers.png)

## Customer Billing and Shipping Address

Each customer may be assigned with a default billing and shipping address. These details will be auto-saved by the system when the customer shops with their given email address. Or you can overwrite these details at your customers’s request.

What’s the benefit of saving default address details? These details will be auto-filled for the customer when they go to checkout, making checkout quicker. These details will also auto-fill if you choose to create an order for your customer in the back end, via [orders](/hubs-set-up-guide.md).

If a customer changes address, they can also update their default address records during checkout by selecting the ‘save as default’ checkbox:

## [![](https://openfoodnetwork.org/wp-content/uploads/2015/10/save.png "Save details")](https://openfoodnetwork.org/wp-content/uploads/2015/10/save.png)

## 

## Customer Tagging

Customer tagging is a way to control the shopfront settings for different customers. Currently this includes:

* Making particular variants available/unavailable
* Making certain shipping methods available/unavailable
* Making certain payment methods available/unavailable
* Making order cycles visible/invisible

Most often this feature is required by enterprises who have different shop setups for members Vs non-members or different groups of customers such as wholesale Vs retail customers.

Using the tagging feature involves two main steps:

1. Tagging your customers
2. Setting up a
   **tag rule**

### Tagging Customers

Any customer’s who have placed an order in your shop will be listed on the C**ustomers **page \([https://www.openfoodnetwork.org.au/admin/customers](https://www.openfoodnetwork.org.au/admin/customers)\). Each unique email address used, will be listed as a unique customer.

You can create a tag for groups of customers, such as your members or your wholesale customers, for whom you will set up tag rules \(which carry a discount, or special shipping methods\). To create a tag, type the tag in the **tag** column next to a customer and hit the enter button when you’re done. You should do this for all customers in the group \(this could just be one, or many customers\). You can add multiple tags to a single customer also. Remember to type the tag with identical characters each time \(tags are case sensitive\).

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Customer-taggs.png "Customer tags")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Customer-taggs.png)

Once you have applied tags to your customers, you can then apply **Tag Rules **to control certain setting for customers in certain tag groups \(see Tag Rules below\).

Any tags that you attach will also show up in your ‘Order cycle customer totals’ report, next to this customer’s order. If you take these reports to excel you can then filter your reports according to these tags, making it easy to sort your orders based on certain information.

Note: If you are transferring an existing hub/shop onto the OFN there is no way to import your database of customers into the system. Customers will only show on this page after they place their first order on the OFN.

### Tag Rules

Once you have tagged your customers you can define how certain feature will apply to customers with different tags. Currently you can use tags to change four elements:

* Making particular variants available/unavailable
* Making certain shipping methods available/unavailable
* Making certain payment methods available/unavailable
* Making order cycles visible/invisible

To set up your tags go to Edit your Enterprise interface and select **Tag Rules**.

### By Default

By default, all items will be visible to all customers whether they are tagged or not. The general approach is to then create a rule dictating that certain items \(variant, shipping/payment methods or order cycles\) will be invisible to certain customers who are tagged. However, if you wish to change this default, such that tagged items are ‘not visible’ until a rule is setup reversing this, you can do so by changing your ‘By Default’ rules.

The example below shows that my shipping methods tagged ‘wholesale’ will now be invisible by default. If I then wish to make these shipping methods available to customers tagged wholesale I’ll need to set up a Tag Rule below overriding this default.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Default-tags.png "Default tags")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Default-tags.png)

### Tag Rules

Keeping in mind your default setting above, you can now apply rules to vary the default settings for certain customers.

Firstly, you’ll need to select which tag your new tag rule will apply to. To do this type the tag into the ‘for customers tagged:’ field.

Next you can select which condition your rule is based on.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Rule-Typess.png "Rule Types")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Rule-Typess.png)

#### **Show or Hide Variants in my shopfront**

This rule lets you make particular variants visible/invisible to tagged customers. For this rule to operate you need to have tagged the customer and the product variant **in your inventory** with the same tag. The screenshot below shows that my 10kg apple variant is tagged ‘wholesale’ in inventory.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-tagged.png "Inventory tagged")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-tagged.png)

* **Invisible:**
   If by default your variants are visible, you can select to make them invisible for customers with a particular tag.
* **Visible:**
   If by default your variants are invisible, you can select to make them visible for customers with a particular tag.

The example below shows that my wholesale variants are invisible by default. A rule has been created so that variants tagged wholesale are made visible just for customers tagged ‘wholesale’.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-taggedd.png "Inventory tagged")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Inventory-taggedd.png)

#### **Show/Hide shipping methods**

This rule lets you make particular shipping methods specifically available or unavailable to certain customers. For this rule to operate you need to have tagged the customer and the shipping method with the same tag. To tag a shipping method, go to **edit shipping method **and apply the relevant tag. E.g. the shipping method below has been tagged ‘wholesale’.

![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagging-a-shipping-method.png "Tagging a shipping method")

* **Invisible:**
   If by default your shipping methods are visible, when you set the rule where ‘shipping methods tagged\_are invisible’ shipping methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged shipping methods will still be visible to these customers.
* **Visible:**
  If by default your tagged shipping methods are invisible, you can make them visible to particular customer by setting a ‘shipping methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this shipping method at checkout.

#### **Show/Hide payment methods**

This rule lets you make particular payment methods specifically available or unavailable to particular customers. For this rule to operate you first need to have tagged the customer and the payment method with the same tag. To tag a shipping method, go to **edit payment method **and apply the relevant tag. E.g. the payment method below has been tagged ‘wholesale’.

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagged-payment.png "Tagged payment method")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Tagged-payment.png)

* **Invisible:**
   If by default your payment methods are visible, when you set the rule where ‘payment methods tagged\_are invisible’ payment methods with the tag will be hidden from customers with a matching tag when they checkout. Untagged payment methods will still be visible to these customers.
* **Visible:**
  If by default your tagged payment methods are invisible, you can make them visible to particular customer by setting a ‘payment methods tagged\_are visible’ tag rule.  Customer without tags or with different tags will still be unable to see this payment method at checkout.

#### **Show/Hide order cycles at my shopfront**

This rule lets you make certain order cycles visible to certain customers only. For this rule to operate you need to have tagged the customer and the order cycle with the same tag. To tag an order cycle, see the Tags tab in the outgoing section of an order cycle \(see below\).

[![](https://openfoodnetwork.org/wp-content/uploads/2015/10/Outgoing.png "Tag OC in Outgoing")](https://openfoodnetwork.org/wp-content/uploads/2015/10/Outgoing.png)

* **Invisible:**
   If by default your order cycles are visible, when you set the rule where ‘Order cycles tagged\_are invisible’ order cycles with the tag will be hidden from customers with a matching tag. Untagged order cycles will still be visible to these customers.
* **Visible:**
  If by default your order cycles are invisible, you can make them visible to particular customer by setting a ‘order cycles tagged\_are visible’ tag rule.  Customer without tags or with different tags will not see this order cycle.



