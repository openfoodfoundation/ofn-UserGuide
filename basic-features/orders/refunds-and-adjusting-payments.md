# Refunds and Adjusting Payments

From time to time, a customer may request that their order is adjusted, either to remove or add items. 

On other occasions you, as a business manager, may need to change an order. Common scenarios include:

1. A product was not delivered by a supplier
2. A product was of lower quality than expected
3. An order contains products with variable weights such as [meat or large vegetables](../products-1/pricing-irregular-items-kg.md#option-one-set-an-average-weight-price-and-reimburse) \(ie. whole items priced by weight\).

The process of issuing a refund or requesting further payment depends on the [payment method](../shopfront/payment-methods.md) employed.  

{% hint style="warning" %}
On the OFN platform, refunds and additional payments can only be taken **automatically** using the [Payment Method](../shopfront/payment-methods.md) Provider **Stripe/Stripe SCA**.
{% endhint %}

## Refunds

Using the OFN Platform, you can either process a Total refund, or make an adjustment to the order to change the balance owing, and then process a Partial refund.

{% hint style="warning" %}
 If you have integrated with Stripe as a Payment Method, you can log in to your Stripe account and issue an invoice to the customer via Stripe. The customer will be sent an email asking them to pay with a Credit or Debit Card, but be aware that OFN will not be notified of this transaction and you will still need to manually capture the payment as received in OFN.
{% endhint %}

### Total Refund

To issue a refund, select the relevant payment method from the tabs below:

{% hint style="warning" %}
For all methods it is best practice to refund the payment to the customer before you mark the order as cancelled. 
{% endhint %}

{% tabs %}
{% tab title="Cash/BACS" %}
For non-automated payment methods \(such as cash on collection or BACS\), there are two scenarios:

  
**The customer has not yet paid for the item.**  
If a customer places an order, selecting a payment method such as cash on collection or BACS and the payment has not been captured on the system it will appear as:

![](https://lh6.googleusercontent.com/9lIYAkArDP1yllI88_N00rOQYiQqu9KG-piADA0hJtUvelv1NZAPNOx0Q9Ph3a6yu1gal9zUuFgJox0xiRC4RM4UlwmcfCdspcSlG9w_m23a8Cv_SnWI8yfgNIBnfClRx3MJ7Ru0)

You can [cancel the order](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled) straight away following steps below.

**The customer has paid for the item.**

When [viewing orders](view-orders.md#listing-orders) the order appears as:

![](https://lh5.googleusercontent.com/7Uorian_j1n-fPDTQQSeSiHr1tcDQczsaCb_WSxIKRt1PRp1S3l4bKhaFA6WfMaiEsGgN0Qx5OdLfi_lBK9yz1r5-Oh0AcZKkM0MfrbfOzQCpejuQLWvAMRNFCom9-r-S2ZfqMjt)

1. Arrange for the customer to be reimbursed independently of the OFN platform.  
2. Record this action by [**Orders -&gt; Edit**](view-orders.md#editing-an-order) and select the ‘Payments’ tab from the right hand menu.   Select the ‘X’ to the right hand side of the payment to void it.

![Before marking the payment as void.](https://lh6.googleusercontent.com/1mhZhKoPtqPZVZIDz_VV4-8uBy5BefLVo9SftwfecciD7sJCGZhwgEWb-PeYAPI01w3AOZ0x_d7oWpMTQpLBqv201qb8VtmFjB1SaK0nChsy7knCt_EVQwlaioEPTtBZSUQLuLQa)

![After marking the payment as void.](https://lh6.googleusercontent.com/ui2lGGDHK7Pp6KZQ34UHg4KERF9eGDgQKHg3YIr20B8J0oyObiCVic5hOuvpR5HOK16dvvR8aCx70LYnPE-kKN2AKBfPkz3nXvhAM17oYgdPLmDhJiApl7-w_vfDKog2p8iFAKcY)

Then [mark the order as ‘cancelled'](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled) using the steps below.
{% endtab %}

{% tab title="Stripe" %}
Order payment is collected automatically on creation \(except for [subscriptions](../subscriptions/)\) and so in [listing Orders](view-orders.md#listing-orders) the order appears as:

![](https://lh6.googleusercontent.com/9_eN8vGTnyWSL997ebeYQeasxhaiOGKlkwLFydvAHJGiXvUgCR1CmuPRl-fZ4DbwUw3tVNnSSEI7S8M7ZqnYrkGdPkvRHvBpPKmhK47wjFCXfDrF8VUanpBe8NdErg-3nl6b549y)

Visit [**Orders -&gt; Edit**](view-orders.md#editing-an-order) and select ‘Payments’ from the right hand menu.   
Click on the ‘**X**’ to the right of the payment to void it. 

![](../../.gitbook/assets/stripetotal.jpg)

This will automatically send the payment back to the credit or debit card used by the customer.

{% hint style="info" %}
Note that Stripe payments can take 3-5 working days to appear on a customer’s bank statement.
{% endhint %}

Once you have issued a refund, follow the steps below to [cancel the order](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled). It is important to process the refund BEFORE you cancel the order! 
{% endtab %}

{% tab title="PayPal" %}
Payment is collected automatically on checkout from the customer and so in [listing Orders](view-orders.md#listing-orders) the order appears as:

![](https://lh6.googleusercontent.com/9_eN8vGTnyWSL997ebeYQeasxhaiOGKlkwLFydvAHJGiXvUgCR1CmuPRl-fZ4DbwUw3tVNnSSEI7S8M7ZqnYrkGdPkvRHvBpPKmhK47wjFCXfDrF8VUanpBe8NdErg-3nl6b549y)

{% hint style="danger" %}
**Orders placed and paid for via PayPal can not be refunded through the OFN platform.**
{% endhint %}

![](../../.gitbook/assets/pp.jpg)

To refund the customer you will need to log into your [PayPal account](https://www.paypal.com/uk/home) and issue the money back to the customer’s account through their interface.

Once this has been done, you can [mark the order as cancelled](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled) using the steps below.
{% endtab %}
{% endtabs %}

#### Marking an order as cancelled

Once you have issued a refund, you can now cancel the order. [Edit the order](view-orders.md#editing-an-order) and select ‘Cancel Order’ under ‘Actions’ \(top right hand blue button\)

![](https://lh6.googleusercontent.com/V3A6girSx2xUYYW9Jp3VIp41YZrgSq7JaicQlLWUrcVqA1u6SzFjagJkg0KLIL05LgRBXErJyk_iLVrBwt9metOp_RqXmSKL8dRCxFtj6VqTEDjx7z_NHERFNJPw-CdOlNGGmBYp)

{% hint style="success" %}
The customer will receive an email to state that their order has been cancelled.
{% endhint %}

{% hint style="danger" %}
Note you can not cancel an order which has been marked as ‘Shipped’
{% endhint %}

### Partial Refund

To issue a partial refund, you first need to edit the order to change the balance owing. There are two main ways to [edit an order](view-orders.md#editing-an-order) when you want to issue a partial refund. You can either remove an item, or make an adjustment \(eg. to fees\):

**1.Edit by Removing an item which is not in stock or changing the quantity of an item** by going to[ Orders -&gt; edit ](view-orders.md#adding-and-removing-products-from-an-order)order and clicking on the ‘edit’ icon to the right of the item in question, as shown below:

![](https://lh3.googleusercontent.com/j2D8s2OgT-b37OoQHBIitKnWXP6nQ4kDv-EoR4uuFAAjUyulllo0thorXy0UkABcLpXgmunQNeDzNk2buHsOv-B7qt7ZdpH2JNoBW-b5cHDQKn6d1zct_wiRuhTXOJ91gGPm1zYQ)

Select ‘Update and Recalculate Fees’ at the bottom of the page.

{% hint style="danger" %}
If the product has been deleted by the supplier from their master [product](../products-1/) list then it will not be possible to edit this page. In which case, use the ‘adjustments’ method below.
{% endhint %}

**2. Edit by Changing the Fees** in the [order](view-orders.md#modify-an-order) by visiting **Orders -&gt; Edit -&gt; Adjustments** from the right hand menu.

![](https://lh3.googleusercontent.com/qu1o7_GwVwvozkH-aSaxH7Pg9ZJ9mcd-jXM0VrNmUTGyMeOfKmdhf8WPa66FjVayQEryr1Bkv4Q_2UfVSlhSCDvvQcSaZ-ARj-gJG01cWPTRh4ktAMy1ofk4gyUiWQ4ZoK2OfkjB)

This will bring up a list of enterprise fees for each item in the order as well as shipping and payment method fees. You can adjust one of these fees by clicking on the ‘edit’ icon to the right of the item in question.  


**3. Edit by adding a new Adjustment** to the ****[**order**](view-orders.md#modify-an-order) ****by visiting **Orders -&gt; Edit -&gt; Adjustments** from the right hand menu and selecting **+New Adjustment** \(the top right hand button\) to make a separate adjustment that is unrelated to fees.

![](https://lh4.googleusercontent.com/EthxGvVJ3p4skPNpKYy4ivNt3e6xe3pJb4qtgfe_3Z3ESM3WxnkRXrGaXvKZIbKnJoNJ5lI-kn8J_sEe1Lwn-3VOiiSYtQ2OUcVu7LlKSVrjgoFo9UWyeBitqKXRFB1_5ccyuQdB)

Add the relevant details, remembering that for **a refund**,  the value needs to be a **negative number**. When finished, click ‘continue’.

![](https://lh3.googleusercontent.com/RfvWyS1G6v7NVNIDGWTlpfK9hfZj7Vy5_Q6NxlEEyWYtAnebNEphT8XTCSPGvC2EaIGrxioqhcGfaBOIpgqjhjqtSiCwCMKcd4BLFV9M2YIWQ32XkpkAqz_fV-8GWI7CpkLteRpl)

{% hint style="success" %}
You can use ‘Adjustments’ to partially refund a customer for a substandard product.
{% endhint %}

Once the order has been amended to reflect either the missing / adjusted products, the adjusted fees, or the new adjustment, the order will appear with the payment state of ‘Credit Owing’ for the amount they no longer need to pay.

**Process the Partial Refund**  
To process a partial refund of the amount that is now owing on the order, see instructions by choosing the payment method from the following tabs:

{% tabs %}
{% tab title="Cash/BACS" %}
1. Arrange for the refund to be made to the customer independently of the platform.  
2. Record this action by **Orders -&gt; Edit** and select ‘Payments’ from the right hand menu

![](https://lh5.googleusercontent.com/Zt7ppdgUXqxp178D72tj9A5asLzqKoaI8YrniuLDokcraOvNRBT6Hn2oEGxOtM8n7fLb54VrXRYDzyLj4rmki6rr6NC_8lRzME6B9VGjJ2dB78rpPMeoIT_KBKpzA9GMncfpCXPc)

Select **+New Payment**

![](https://lh3.googleusercontent.com/l7lOK1yuMFNLur3XJhDEWTmaKQcfXhmziy26qbxXgUF7vs8BkvTTj7NPivA1wqgkckp5_PNb3VtsNpOngDw7s9bszPMDMPvy5T7Ulu0c_F2AhbHNJY0BsABUPMm6603_ut7gqIpg)

A **negative value** in the ‘Amount’ field means the refund is recorded. 
{% endtab %}

{% tab title="Stripe" %}
Using the OFN platform you can automatically refund a customer who paid by Stripe. This will directly process the refund to their credit or debit card.

1.Visit **Orders -&gt; Edit Order** and then select ‘Payments’ from the right hand menu

![](https://lh6.googleusercontent.com/DEfR7g7tS3wpeX3d3425q0i5yMImnTnwtJEqP2GfHEB_nLp1SnqopkJUx8VHZ7jdZQLpYQdBwAtudkKp091KbNBBzB0jbRnd2jy5NBZH6g3WNfA18y8jSCVOPLabPe2tU-WRmfjy)

2.By clicking on the tick next to the payment, any credit owed to the customer will be automatically refunded. ****

![](../../.gitbook/assets/refundfeast2.jpg)

{% hint style="warning" %}
Note that Stripe payments can take 3-5 working days to appear on a customer’s bank statement.
{% endhint %}
{% endtab %}

{% tab title="PayPal" %}
**You can not issue a partial refund to a customer who paid by PayPal automatically via the OFN platform at present.**  

1. You will need to log into your business [PayPal account](https://www.paypal.com/uk/home) and refund the customer the correct amount through their interface.
2. To record this action you will need to set up a new [Payment Method](../shopfront/payment-methods.md) as follows: Name= ‘Paypal refunds’ Display = ‘Back Office Only’ Payment provider = ‘cash/EFT/etc’.
3. Visit **Orders - &gt; Edit Order-&gt; Payments** \(found in the right hand menu\).
4. Select **+New Payment** and select ‘Paypal refunds’:

![](https://lh4.googleusercontent.com/OxsAJGhZBmz7fZiuWo1Fp5l-hdfGvnFm2vIZRRAxYf5yc2z1q7pCz4-ef6wWb-T6QaKh5uxCFFAX-MG3PaXe_N3ry4fpZ8XEp59NpmGididpdfvzf4gXvGBhQyRbmYfqhtFWrg1s)

A negative value in the ‘Amount’ field means that a refund is recorded.

{% hint style="danger" %}
If you opt to add a new payment with the payment method provider ‘Paypal’ this will not be possible:
{% endhint %}

![](../../.gitbook/assets/paypalnewpayment%20%281%29.jpg)
{% endtab %}
{% endtabs %}

## Collecting Additional Payments

Follow the steps above for [Partial refunds](refunds-and-adjusting-payments.md#partial-refund) to add extra items to a customer's order or make adjustments via the [Bulk Order Management](../products-1/group-buy-for-bulk-ordering.md#adjusting-orders-to-make-complete-batches) page.

Orders will now display with the Payment State = ‘Balance Due’:

![](https://lh3.googleusercontent.com/0SIla3VUQfK-MqNQ0RTuLwndE2_EFmBmZhafSRbb3v0QkDFwXCfPNXyKupa3cwBjXAAoiH6cc-5fMru2xP7SvfraYDnwFrH5jucOVcVUSo1SMv5hiGWn3wgNr15Jz670O80pSZ39)

To record payment of the extra monies due visit [Orders -&gt; Edit Order](view-orders.md#editing-an-order) and then ‘Payments’.   
Select **+New Payment** \(top right hand blue button\)

1. If customer has given your business the money owing in **cash or BACS** payment then record this in the same manner as detailed for a refund, but use a positive value in the ‘Amount’ field.
2. If the customer is present or on the end of the phone you can take the extra payment by **Stripe**. You will need the customer’s credit/debit card details to do this:

![](https://lh3.googleusercontent.com/xou54OA2WQDBKXWmRqHkT6em-7qkd8F6CNJ_hvGWRCvzYbEh2JRtrI54C1ywHeL0X6VR8cFRnV3FELd_pO-kufo2nPszNDq6d2VdO-PPHgnpw3TcgY6n8ysSq8AhaGim-alJYZNX)

{% hint style="danger" %}
Note collection of the extra monies by PayPal through the platform is, at present, not possible.
{% endhint %}

{% hint style="warning" %}
If a payment method has an associated fee attached then the fee will be recorded by the system every time you collect extra money from the customer or issue them a refund.
{% endhint %}

