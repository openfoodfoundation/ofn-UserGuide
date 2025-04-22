# Payment Methods

{% hint style="danger" %}
You **must** create at least one payment method before you can open your shop.
{% endhint %}

## Setting up a Payment Method

* Go to the Payment Methods page by clicking on **Enterprises** on the main horizontal menu, and then click **Settings** next to your enterprise. The **Payment Methods** page is found in the menu on the left hand side.
* Click **Create new payment method +** . You will be directed to a page like this:

![](<../../.gitbook/assets/payment method.jpg>)

* Tick your enterprise, in the box on the right hand side of the page titled Hubs. This indicates which enterprise the payment method you are about to create will apply to. You can select more than one enterprise.
* **Name:** Choose a name for this payment method. (eg 'Pay with credit card using Paypal'). This name is displayed at checkout and on customers' order confirmation emails.

![](<../../.gitbook/assets/payment checkout2.jpg>)

* **Description:** provide further details about the payment method. For example, for a bank transfer, you would enter the bank account details in this box into which you would like a customer to make the BACS payment. This description is displayed at checkout and in order confirmation emails.
* **Display:** Opt for either 'Back Office Only' or 'Both Checkout and Back Office'

{% hint style="info" %}
If you want to inactivate a payment method for a while but might want to offer it again in the future (perhaps due to a COVID outbreak you temporarily need to stop offering cash on collection) then change it to 'Back Office Only'.
{% endhint %}

{% hint style="warning" %}
Changing all your enterprise's payment methods to 'Back Office Only' will result in a [Display Only Shopfront](display-only-order-cycles.md) for active order cycles.
{% endhint %}

* **Active:** Select whether this payment method is currently visible and available, or not.
* **Tags:** Use tag rules if you want to make certain payment methods available/unavailable for specific customers (for example you may wish to allow only wholesale customers to pay by BACS but 'force' domestic customers to pay by Credit Card or PayPal.). For more information read [here](customer-management-and-conditional-displays-prices/).
* **Payment providers**: Select the option which is relevant to the payment method you are creating. There are three options:
  * PayPal Express&#x20;
  * Stripe SCA
  * Cash / EFT / etc. (Cash, cheque or bank transfer. These payments do not go through an online payment portal and do not involve automatic validation)&#x20;

![](<../../.gitbook/assets/payment provider.jpg>)

{% hint style="warning" %}
Remember!  If your enterprise has '_**Customers can change or cancel orders while an order cycle is open'**_ enabled (found in Enterprises -> Settings -> [Shop Preferences](../enterprise-profile/enterprise-settings.md#shop-preferences)) then the only recommended payment provider which is compatible with this feature is 'Cash, EFTs, ...)
{% endhint %}

* **Calculator:** Select how you would like any charges associated with the payment method to apply to an order. Note that payment method fees can be set to zero. See below for more information about [Payment Method Fees](payment-methods.md#fee-calculators).&#x20;

By clicking Create, the payment method will be created and you will have new fields to define payment method fees. These fields visible depend on which 'Calculator' you selected.&#x20;

{% hint style="info" %}
If you change the Payment Method fee 'Calculator' field you must first save your changes (Update) for the new associated fields to become visible.
{% endhint %}

## Integrated Payment Providers

For Paypal, MasterCard, Stripe and Pin Payments (Australia only) additional instructions are below.

{% tabs %}
{% tab title="Paypal" %}
To setup a PayPal payment method, you need a PayPal business or merchant account. You can create one [here](https://www.paypal.com). Once you have that, you can set up ‘API access’ within PayPal, which will enable OFN to connect customers directly with your PayPal account.

1. Login to your PayPal Account
2. Under your account name on the top right there is a drop down menu with 'Account Settings'

![](../../.gitbook/assets/paypalmay1.jpg)

3\. Select 'Update' from API Access

![](../../.gitbook/assets/paypalmay2.jpg)

4\. Select 'Manage API credentials' from the custom checkout experience option.

![](../../.gitbook/assets/paypalmay3.jpg)

From here you will be able to access your API username, password and signature.

![](../../.gitbook/assets/paypalmay4.jpg)

**In OFN,** make sure you are logged in as your Enterprise User. Go to an Enterprise and create a Payment Method. Select PayPal and fill in the details from the PayPal site.

**Server:** Change the ‘server’ field to ‘live’ – this is case sensitive.

**Login:**&#x54;ype the API Username.

**Password:**&#x54;ype the API Password.

**Signature:**&#x54;ype the API Signature in this field.

![](../../.gitbook/assets/paypal.jpg)

**Solution:** Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a paypal account, or “Sole” if they can checkout without a Paypal account (with credit card) - this field is case sensitive.

**Landing Page:** You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal (if you selected “Mark” above) or “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account (if you selected “Sole” above) - n.b. this field is case sensitive.
{% endtab %}

{% tab title="MIGS" %}
&#x20;MasterCard Internet Gateway Service (MIGS)

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.
{% endtab %}

{% tab title="Stripe" %}
[Stripe](https://stripe.com/au) is an online payment platform similar to Paypal. It will allow you to accept credit card payments from your customers. Stripe is a global platform, but is only available on certain OFN instances. Contact your [local OFN team](https://openfoodnetwork.org/ofn-local/) to see whether it’s available on your OFN.

#### Why use Stripe?

Stripe is simple to setup for shop owners and is reasonably priced. The fees charged by Stripe vary in each country; [Australia](https://stripe.com/au/pricing), [Canada](https://stripe.com/ca/pricing), [France](https://stripe.com/fr/pricing), [UK](https://stripe.com/gb/pricing), [USA](https://stripe.com/us/pricing).

Stripe is also easy for customers to use. Unlike Paypal, when the customer checks out, they don’t need to login with Paypal to place their order, rather they just need to enter their card details and then complete their order.

Stripe is the recommended payment method for shops who wish to use [**subscriptions** ](../subscriptions/)on OFN, as Stripe allows customers to give permission to a shop to automatically bill their credit card for subscription orders. This isn’t offered by Paypal, Pin or MIGS payment platforms.

#### Setup

**Connect with Stripe**

Before you can setup a payment method that uses Stripe, you’ll need to Connect with Stripe. To do this, click on the ‘Connect with Stripe’ button.

![](../../.gitbook/assets/connect-with-stripe.png)

You’ll be taken to a form to fill in your details. If you already have an account with Stripe, you can login, if not, fill in the form to create a Stripe account.

The information you’ll be asked for includes: country, a description of your business, your Business address and ABN, your personal details and your bank account (where received payments will be deposited).

**Create a New Payment Method**

Once you’ve connected with Stripe, you can then create a payment method which will work with your connected account.

Treat the **Name**, **Description**, **Active** and **Tags** fields as you would with any payment method.

**Provider:** Select Stripe.

Once you select Stripe, ‘Provider Settings’ will be shown.

**Stripe Account Owner:**

Select the enterprise that has a Stripe account connected.

If you select an enterprise that is not Connected to Stripe (see above) , you will get the error shown below. Either click ‘Connect One’ or return to your Payment Methods tab to Connect with Stripe. See instructions above.

![](../../.gitbook/assets/stripe-connect.png)

#### Stripe Payments for Customers

When customers checkout in a shop and pay with a Stripe payment method, they’ll have the options of selecting a tickbox allowing their credit card details to be stored against their account (if they are logged in).

Customer can also save a credit card in their Account, or delete saved ones.

![](../../.gitbook/assets/add-card.png)

When the customer next shops with an OFN shop offering Stripe as a payment method, they’ll be able to select from their saved credit cards.

**Viewing and redeeming your payments via Stripe**

When a customer pays for their order with Stripe, the funds (minus Stripe's fees) will go to your stripe account. Depending on your setting in Stripe the funds will be automatically transferred to your chosen bank account periodically.

**Taking further payment**

If you need to take additional payment from a customer because they have further balance due,  you can create an invoice in Stripe. The customer will get sent an email asking for them to pay with Credit/Debit card. This won't be communicated to OFN, so you'll need to mark the payment off manually.

![](<../../.gitbook/assets/image (31).png>)
{% endtab %}

{% tab title="Pin Payments" %}
For Pin Payments you only require your API key. You need to set up an account with Pin Payments first, and can get a discount by signing up as an OFN member ([https://pinpayments.com/partners/openfoodnetwork/signup](https://pinpayments.com/partners/openfoodnetwork/signup))

**API Key:**&#x45;nter your “Live Secret API Key’ here – you can find this in your PinPayments account (see below). First from your account, select API Keys. Then once you have generated an API key, copy the ‘Live Secret API Key’ and paste it into the API key field in OFN.

![](../../.gitbook/assets/api-keys.png)

![](../../.gitbook/assets/api-2.png)

**Server:**&#x54;ype ‘live’ – this is case sensitive.
{% endtab %}
{% endtabs %}

## Payment Method Fees

![](<../../.gitbook/assets/fee calculator.jpg>)

You can attach a fee to payment methods. Most commonly this is used to pass on a payment portal's fees to the customer.  For example, you may wish to charge the customer for the convenience of paying by PayPal to cover the fee charged by PayPal.

{% hint style="danger" %}
Payment Method Fees DO NOT include tax (VAT)
{% endhint %}

### Fee Calculators

**Flat Percent:** This fee is charged as a percentage of the total amount charged in the order.

{% hint style="danger" %}
All **percentage fees** are calculated on a percentage of **product costs** only.&#x20;
{% endhint %}

{% hint style="warning" %}
If your business adds a flat percent [Enterprise Fee](enterprise-fees.md) to all products then in order to make the 'Flat Percent' **Amount** your desired percentage of a customer's basket is

&#x20;$$= (100 + Enterprise Fee)*Desired Percent/100$$&#x20;

eg. for a business with an enterprise fee of 20% who would like to charge a fee of 5% of a customer's total basket for payment, the amount to enter in the flat percent of this payment method is:

$$= (100 + 20) *5/100 = 6$$&#x20;
{% endhint %}

**Flat Rate (per order):** This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate** – This fee calculator is especially useful if you'd like to encourage customers to place large orders: the cost of payment can be reduced or zero when the threshold number of items has been reached.&#x20;

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for items beyond the first item.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

![](<../../.gitbook/assets/fee- flexible rate.jpg>)

> For Example: if the 'First Item Cost' is set to £0.20, 'Additional Item Cost' is £0.10 and 'Max Items' is 3 then a customer who purchases 5 items will be charged £0.40 in payment fees (£0.20 for the first item, £0.10 for items two and three, and £0.00 for items four and five).

**Flat Rate (per item):** This fee is a constant fee, applied to products listed as ‘items’. (It is not applied to products sold by weight or volume. Hence there will be no associated payment method fee charged to a customer who, for example, buys rice by kg.)

**Price Sack:** This is a flexible shipping fee method that allows you to reward shoppers who spend over a ‘minimal amount’ by applying a discount. If the shopper spends less than the ‘minimal amount’ you can set what shipping fee they pay.&#x20;

* Minimal Amount: If the order total is below this amount, no discount is applied. If the order is above this amount, the discount will be applied at checkout.
* ‘Normal Amount’: This will be the shipping fee applied to sales below the ‘Minimal Amount’.
* ‘Discount Amount’: This will be the shipping fee applied to sales above the ‘Minimal Amount’.

{% hint style="danger" %}
The **Minimum Amount** is the _**total cost of the products**_ in a customer's basket and does not include any [enterprise fees](enterprise-fees.md).
{% endhint %}

![](<../../.gitbook/assets/fees price sack (1).jpg>)

{% hint style="warning" %}
For example, if a business adds an Enterprise Fee of 20% to all products and they wish to set the threshold between no fee for payment (Discount Amount = 0) and, say, a £0.50 fee (= Normal Amount) to be a basket of £30 then the Minimum amount is

$$= £30 * 100 /(100+20) = £25$$&#x20;
{% endhint %}

{% hint style="info" %}
Payment portals often charge businesses a fixed amount per transaction plus a small % of the total cost.  Thus fees encountered by a Hub or Shop for customers who purchase the same total amount in multiple small sales will be higher than if the customer did all their shopping at once.&#x20;

The Flexible Rate and Price Sack calculators, applied to payment method fees, may prove useful to counter balance this.
{% endhint %}

## Refunds

Issuing and managing refunds depends on how a customer originally paid for  their order.  More details are found[ here.](../orders/refunds-and-adjusting-payments.md)
