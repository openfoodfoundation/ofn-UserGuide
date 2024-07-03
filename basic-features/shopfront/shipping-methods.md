# Shipping Methods

{% hint style="warning" %}
&#x20;You **must** create at least one shipping method before you can open your shop.
{% endhint %}

## Setting up a shipping method

* Go to the Shipping Methods page by clicking on **Enterprises** in the main horizontal menu, and then click **Settings** next to your enterprise. The **Shipping Methods** page is found in the menu on the left hand side.
* Click **Create new shipping method +** . You will be directed to a page like this:

![](<../../.gitbook/assets/new shipping method.jpg>)

* Check the box next to your enterprise on the right hand side of the page under 'Hubs'. This indicates that the shipping method you are about to create will apply to that enterprise.  You can select multiple enterprises, if desired.
* **Name**: Choose a name for the method. This name will be displayed to the customer during their purchase process and on order confirmation emails. Example:

![](<../../.gitbook/assets/shipping checkout multi.jpg>)

* **Description:** Add additional details, such as the precise address of the collection point. These details will be visible to customers in grey next to the name (see screenshot above) and in their order confirmation email.
* **Display:** Opt for either 'Back Office Only' or 'Both Checkout and Back Office'

{% hint style="info" %}
If you want to inactivate a shipping method for a while but might want to offer it again in the future (perhaps a summer only collection point that you don't want to be available to customers in the winter) then change it to 'Back Office Only'.
{% endhint %}

* **Category:** Is this method a delivery or pick-up?
* **Tags:** enter labels here if you wish to differentiate between customers. Tags could be useful if you want to offer free shipping to a sub set of customers or only offer delivery to those who have a registered address which is close by.  Read more [here](customer-management-and-conditional-displays-prices/).
* **Calculator:** Select the way that shipping fees will be added to this shipping method.  Note that a shipping fee may be zero. See below for more details.
* **Tax Category:** This enables you to set the tax associated with your shipping method/collection fee independently to that assigned to tax-eligible products owned by your enterprise.  The options are: none, full rate, zero rated, reduced rate or shipping.
* **Categories:** Transport conditions (refrigeration, frozen, default) associated with this shipping method.

{% hint style="danger" %}
Under 'Categories' tick all boxes which apply to your food enterprise ie. if you sell products listed with a shipping category of 'frozen' then in order for the customer to be able to successfully checkout their shopping, the 'frozen' category will need to be checked in their desired shipping method.
{% endhint %}

* **Zones:** Select the appropriate zone (this is to enable correct tax calculations).

By clicking **Create,** the shipping method will be created, and you will then be provided with new fields, to add details of the shipping method charges. The fields presented will depend upon which shipping fee calculator you have selected.&#x20;

{% hint style="info" %}
If you change the calculator type for a shipping method, you must **save first** before you can edit the calculator settings.
{% endhint %}

## Fee Calculators

![](<../../.gitbook/assets/shipping fee calc.jpg>)

**Flat Percent** – This fee is charged as a percentage of the total amount spent in the order.

{% hint style="danger" %}
All **percentage fees** are calculated on a percentage of **product costs** only.&#x20;
{% endhint %}

{% hint style="warning" %}
If your business adds a flat percent [Enterprise Fee](enterprise-fees.md) to all products then in order to make the 'Flat Percent' **Amount** your desired percentage of a customer's basket is

&#x20;$$= (100 + Enterprise Fee)*Desired Percent/100$$&#x20;

eg. for a business with an enterprise fee of 20% who would like to charge a fee of 5% of a customer's total basket for shipping, the amount to enter in the flat percent of this shipping method is:

$$= (100 + 20) *5/100 = 6$$&#x20;
{% endhint %}

**Weight (per kg)** – this fee is applied to products on a per kg basis. The fee will _only be applied to products which are priced at a per kg rate_, not products listed as items (e.g. A product listed as ‘1 bunch of parsley’ will not contribute to the overall fee a customer is charged for shipping)

**Flat Rate (per order)** – This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flat Rate (per item)** – This fee is a constant fee, applied to products listed as ‘items’. (It is not applied to products sold by weight or volume. Hence there will be no associated shipping cost charged to a customer who, for example, buys rice by kg).

**Flexible Rate** – This fee calculator is especially useful if you'd like to encourage customers to place large orders: the cost of shipping can be reduced or zero when the threshold number of items has been reached.&#x20;

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for items beyond the first item.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

![](<../../.gitbook/assets/fee- flexible rate.jpg>)

> For example: If the shipping fee for the 'First item cost' is £2, 'Additional Item Cost' = £1 and 'Max items' = 3. \
> A customer who purchases 5 items, will be charged £4 shipping (£2 for the first item, £1 for items two and three, and £0 for items four and five).

**Price Sack** – This is a flexible shipping fee method charged by _total monetary sale_, rather than number of items purchased (Flexible Rate above)

* ‘Minimum Amount’: Monetary value of the threshold between Normal shipping fee and Discounted shipping fee.&#x20;
* 'Normal Amount': Shipping fee applied to sales below the threshold stated in 'Minimum Amount'.
* ‘Discount Amount’: Shipping fee applied to sales above the threshold stated in 'Minimum Amount'.

{% hint style="danger" %}
The **Minimum Amount** is the _**total cost of the products**_ in a customer's basket and does not include any [enterprise fees](enterprise-fees.md).
{% endhint %}

{% hint style="warning" %}
For example, if a business adds an Enterprise Fee of 20% to all products and they wish to set the threshold between free delivery (Discount Amount = 0) and, say, £5 delivery (= Normal Amount) to be a basket of £30 then the Minimum amount is

$$= £30 * 100 /(100+20) = £25$$&#x20;
{% endhint %}

![](<../../.gitbook/assets/fees price sack (1).jpg>)
