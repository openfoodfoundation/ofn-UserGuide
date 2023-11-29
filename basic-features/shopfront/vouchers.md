# Vouchers

{% hint style="info" %}
Vouchers is in 'beta' mode, meaning it's a new feature that may still have some glitches. Please [contact us](https://www.openfoodnetwork.org/find-your-local-open-food-network/) with any feedback about what works, what needs improving or how it could be better explained.
{% endhint %}

Voucher codes can be created to offer shopping discounts to new or existing customers. Voucher functionality is still relatively limited, please read through this guide before implementing vouchers in your shop process.

Set up and manage vouchers in the **Vouchers** tab in your [Enterprise Settings](../enterprise-profile/enterprise-settings.md).

<figure><img src="../../.gitbook/assets/vouchers 1.jpg" alt=""><figcaption></figcaption></figure>

## Setting up a voucher

* Go to 'Vouchers' by clicking on **Enterprises** in the blue bar at the top of the page and then click **Settings** next to your enterprise. The **Vouchers** page is found in the menu on the left hand side
* Click **Add New** in the top right of the vouchers page to be taken to the new vouchers page

<figure><img src="../../.gitbook/assets/vouchers 2.jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/voucher 3.jpg" alt=""><figcaption></figcaption></figure>

* **Voucher Code** - the code customers will enter to recieve a discount. Code is string matched, so double check the spelling, spaces and numbers.&#x20;
* **Voucher Type**
  * **Percentage:** The voucher will add a percentage discount to the entire order the code is applied to.
  * **Amount:** The numeric percentage or flate rate you wish the discount to apply
* Click **save** to create the voucher.

{% hint style="warning" %}
New vouchers will be created as active. If you do not want your voucher to be active, switch it off using the steps below
{% endhint %}

## Managing vouchers

Vouchers can be turned off and on as needed by enterprise managers.&#x20;

{% hint style="warning" %}
Voucher codes will not automatically switch off after customer use
{% endhint %}

In the **Vouchers** page in Enterprise Settings, use the checkbox against each voucher code to deactivate or reactive your vouchers.&#x20;

Click **update** to save changes

<figure><img src="../../.gitbook/assets/voucher edit.png" alt=""><figcaption></figcaption></figure>

## Customer facing use

Customers will need the exact code as entered in the Voucher Code field of set up (above).

In step 2 of check out, **Payment method**, customers can enter the voucher code to have it applied to their order.&#x20;

{% hint style="info" %}
Only 1 voucher code can be applied per order
{% endhint %}

After applying the code, continue through check out to finalise the order

<div data-full-width="true">

<figure><img src="../../.gitbook/assets/Screenshot 2023-11-21 103819.png" alt=""><figcaption></figcaption></figure>

</div>

{% hint style="info" %}
If the voucher brings the **order total cost to zero**, or below, the customer will not be prompted to enter payment method or details. _See screenshot below_
{% endhint %}

<figure><img src="../../.gitbook/assets/Screenshot 2023-11-21 105438.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
If only part of the voucher is used (**order total becomes negative**), the remaining credit will not be carried over to the customers next order.
{% endhint %}
