# Reward your volunteers

## Introduction

Would you like to say a little thank you to the people who help run your community food enterprise?  One option is to allow staff and volunteers to have a small discount off any shopping they do.  Below is a step-by-step guide on how to implement this.  The process draws on the highly flexible Customer Management tools available using [Tags and Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md).

## Process

* Ask your volunteers to  let you know the email address linked to their OFN account.
* Login to your business OFN account and visit [Customers](https://openfoodnetwork.org.uk/admin/customers) page.
* Use the ‘Quick Search’ box to identify if the person has shopped with you before. 

![](https://lh6.googleusercontent.com/DcRo1W18G7l7JKxuhHybJB4gIEzZWQIX-3kynCMX79RwtrKFpMR8b6SYI4uyoQjGOOlmrV1rv7oIbsYS55UkfeH1yfu4SJntTnO1vMPmwuTMljBhkX_kRhYLiI5fKzKjxYBR_uCO)

* If their email address doesn’t appear then click **+ New Customer** and add their address.
* Add the tag ‘volunteer’ to the customer’s entry.

![](https://lh6.googleusercontent.com/SQyjjQgyilzSxTiEtRooR_ELTZdT_v0JAId0xIT5YsSf7crTmCZFyIkLg6mhfFD3_BA9BA43QFWtCqeciTOyim-diGYfcrQrDHCb8umBvxb3nQcNOdS58tC0qg2bOlFPSsMinFbC)

* Visit **Enterprises -&gt; Settings** and then select ‘[Payment Methods](../../basic-features/shopfront/payment-methods.md)’ from the left hand menu.  
* Click **+ New Payment** Method.

![](../../.gitbook/assets/voldiscount.jpg)

  
****Name: Volunteer 5% Discount  
Description: Thank you for helping us run our local food hub.  
Display: Both Checkout and Back Office  
Active: yes  
**Tags: Add the tag ‘volunteer’ into this space.**  
Provider: choose the most appropriate method for your business.  
Fee Calculator: Flat Percent

* After selecting Create, add ‘-5’ \* to the ‘Amount’ field of the ‘Fee Calculator’ Section.  \(Negative sign results in a discount\)  \*-5 will result in a 5% discount if your enterprise does not use Enterprise Fees.

![](../../.gitbook/assets/pmcalc.jpg)

{% hint style="danger" %}
All **percentage fees** are calculated on a percentage of **product costs** only. 
{% endhint %}

{% hint style="warning" %}
If your business adds a flat percent Enterprise Fee to all products then the amount you need to enter into the 'Flat Percent' field for this discount payment method is:

 $$= (100 + Enterprise Fee)*Desired Discount/100$$ 

eg. for a business with an enterprise fee of 20% who would like to offer a 5% discount to volunteers, the amount to enter in the flat percent of this payment method is:

$$= -(100 + 20) *5/100 = -6$$ 
{% endhint %}

* Visit your **Enterprise -&gt; Settings** page and select ‘[Tag Rules](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-payment-methods)’ from the left hand menu.  Set up the following Tag rules:

Default: Payment Methods tagged ‘volunteer’ are not visible.  
For customers tagged ‘volunteer’ payment methods tagged ‘volunteer’ are visible.

![](https://lh5.googleusercontent.com/wSWqmOnwusb_3gWx8J5MVBceTFYfq7AB1-uKMcFfD2neWmuiESg2rI896B4iugX767fDxljCVLe-vFIS5V7pQojimIl2e3iuBPlFzLtlPL1oqtMhYesm9CPX-JybyR3rHpKJ0HXS)

**Bingo!  Only your volunteers will be offered a 5% discount when they shop with you.**

![Checkout view for volunteer](https://lh4.googleusercontent.com/aniH6MTDqxKFnR_7PRP4duUp33nNOd7XdQpa0RRFcEgcoyjsUHSwLXOSEO8lbXWtNTXYFGTrt6QAopPjuiu8zJGxwtcXYalNBw8Y3wi-alSuGLyyBXm4h_AH5pSc11fmvhS_IMuk)

![Checkout view for all other customers](../../.gitbook/assets/allcart.jpg)



