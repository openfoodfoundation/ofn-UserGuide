# Taking Orders on Credit in OFN

## Introduction

Although this feature is not-yet built into OFN, with a few quick steps it is possible to allow customers to pay with prepaid credit
on OFN. In a nutshell, this involves first creating a credit product that the customer checks out with. The store manager will 
then go into the backoffice and ‘delete’ this product putting ‘credit’ on the customer account.  Future orders can then be ‘paid’ 
with the credit on the account.  

## Process

First create a credit product in the backend.  When creating the product in the backend also create a variant named ‘Place Holder credit’ variant for $0 and with ‘0’ for ‘on hand’ available.  It will come in handy later in the backend order admin.  Then add all the variants to an order cycle to sell the prepaid credit to your customers. 

<img width="805" alt="image1" src="https://user-images.githubusercontent.com/88801240/207038941-0057bceb-5690-41d8-86d1-d8490ebd656b.png">

Here is an example credit product in the storefront that the customer can choose to add ‘credit’ to their account.

<img width="782" alt="image2" src="https://user-images.githubusercontent.com/88801240/207040327-75df5d0d-6930-4a8e-aa8b-f3c6be167c7a.png">

Instruct the customer to choose the amount of credit they want to apply to their account and check out their order.  Make sure they ‘save’ their account info by choosing ‘LOGIN’ when checking out and creating an account with a password. 

<img width="854" alt="image3" src="https://user-images.githubusercontent.com/88801240/207040600-029c79d3-f975-4985-849d-4af2f0df0085.png">

Now in the backend you will have their order with the amount of credit they are purchasing.  

<img width="801" alt="image4" src="https://user-images.githubusercontent.com/88801240/207039638-ce1ea75d-1f3b-4b65-9972-2e7aaf1a0d54.png">

Once they have paid the order you can ‘capture’ the payment by using the green checkmark. 

<img width="807" alt="image5" src="https://user-images.githubusercontent.com/88801240/207040438-4b5b9877-0aad-49a9-967c-daa82cb3f9d1.png">

Then you need to go in and ‘edit’ the order, but first you will have to add ‘on hand’ to the ‘place holder credit’ product.  Add the amount of ‘on hand’ equal to the number of credit orders you are processing at that time (i.e. you have 1 credit orders, add ‘1’ as ‘on hand’ to the ‘place holder credit’ variant and SAVE CHANGES). 

<img width="825" alt="image6" src="https://user-images.githubusercontent.com/88801240/207040827-ec6cd04e-5745-4801-ae7c-47ad1725942a.png">

Now you can go back to your order list and choose to ‘edit’ the credit order.

<img width="812" alt="image7" src="https://user-images.githubusercontent.com/88801240/207041020-b5e382b7-1776-4cba-8553-287e1f76a33c.png">

First you will need to add the ‘Place Holder credit’ to the order.

<img width="873" alt="image8" src="https://user-images.githubusercontent.com/88801240/207059609-13145207-dd5c-405e-8e2b-c30a4e71bdb1.png">
<img width="880" alt="image9" src="https://user-images.githubusercontent.com/88801240/207059642-b0de508e-8bea-454b-bffb-36a75eb0fb09.png">

Now you can delete the other ‘credit’ product from the order (adding the ‘place holder credit’ variant first prevents the entire order from being canceled; that step would be unnecessary if the order already contained other products).

<img width="856" alt="image10" src="https://user-images.githubusercontent.com/88801240/207060185-d46f6439-e8d3-41f8-a226-973a55cf1cb1.png">

Now in your orders list the payment state for the order will revert to ‘credit owed’ for the amount of the prepaid credit. 

<img width="814" alt="image11" src="https://user-images.githubusercontent.com/88801240/207060500-e4aac659-658e-4254-aa06-e0d8df583401.png">

It will also look like this in your customer list under the **Customers** tab for that customer.

<img width="808" alt="image12" src="https://user-images.githubusercontent.com/88801240/207062769-cc237a5c-f3c2-4f4f-93f4-2d675c3066ec.png">

And if you do a **Order Cycle Management - Delivery Report**, it will show a positive balance for the customer.

<img width="822" alt="image13" src="https://user-images.githubusercontent.com/88801240/207063074-e30a03f6-fd21-4b4f-8675-7b9abbd49e5b.png">

And if the customer logins to their account on OFN and goes to Transactions they will see a running balance of their account with you.

<img width="821" alt="image14" src="https://user-images.githubusercontent.com/88801240/207063221-32d10df6-9e0d-4318-aaa4-ef3198d5f739.png">

To apply the credit to future orders you will need to [create a payment option](https://guide.openfoodnetwork.org/basic-features/shopfront/payment-methods#setting-up-a-payment-method) - ‘pay by credit’ that customers can choose when they checkout to indicate they want you to use their credits.  You can use [tags](https://guide.openfoodnetwork.org/basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules) if you want this payment option only available/visible to those customers that have purchased prepaid credit with you.

<img width="843" alt="image15" src="https://user-images.githubusercontent.com/88801240/207065857-debdc92d-00ef-4744-afb3-8260e1a13da9.png">

This is what the customer will see when they checkout.

<img width="790" alt="image16" src="https://user-images.githubusercontent.com/88801240/207066041-355ae709-8829-446c-80a7-b08aaa76ac25.png">

Once the customer has placed a 2nd order it will appear in your **Orders** list with a **Balance Due**.

<img width="818" alt="image17" src="https://user-images.githubusercontent.com/88801240/207066716-406ea6b8-9513-4a3f-8289-5c2c36b03042.png">

This is what they will see if they login to their account.  The negative amount means their remaining credit balance.

<img width="832" alt="image18" src="https://user-images.githubusercontent.com/88801240/207066968-74831a05-a51d-4830-9b94-1d5d5f4c2042.png">

And this is what you will see if you as a manager from your customer list.

<img width="837" alt="image19" src="https://user-images.githubusercontent.com/88801240/207067200-d43397ad-52f8-4e66-8c31-4a2f8f70d758.png">

And if you run the Delivery Report.

<img width="798" alt="image20" src="https://user-images.githubusercontent.com/88801240/207067405-8b3e529c-d2a5-492b-ac16-394065edca00.png">

**IF** you want to mark the new order as ‘Paid’ changing the payment state from ‘Balance Due’ to ‘Paid’, you can click the green check mark to the right of the order. (**Note**: You may first want to check your customer list to ensure the customer has enough ‘credit owed’ to cover the order cost.  If they don’t you can make a partial payment on the order with the ‘credit owed’ amount remaining and then send them an invoice for the balance on the order.)

<img width="831" alt="image21" src="https://user-images.githubusercontent.com/88801240/207068083-b0e93789-0d9e-4ca1-b7f4-a50d36a102f6.png">

Now the payment state of the order is 'paid' in your orders list.

<img width="825" alt="image22" src="https://user-images.githubusercontent.com/88801240/207068453-39e70e87-531d-441c-98a1-acdfc2c929c2.png">

But in the customer record and in your customer list the running balance will revert back to the full prepaid credit amount.  

<img width="807" alt="image23" src="https://user-images.githubusercontent.com/88801240/207068600-438bd501-a1f0-4538-90e7-9108c5913129.png">

<img width="817" alt="image24" src="https://user-images.githubusercontent.com/88801240/207068773-43aad4dd-1442-43af-987e-248ef793603c.png">

To credit the payment on the 2nd order to the running balance of credit we must now go into that original credit order and make a negative payment in the amount of the 2nd order (i.e. - $48).

First Edit the original credit order.

<img width="823" alt="image25" src="https://user-images.githubusercontent.com/88801240/207069023-fdcea2ce-b8f4-4265-aecc-fa9b4e5e55eb.png">

Then choose Payments from the right side menu.

<img width="859" alt="image26" src="https://user-images.githubusercontent.com/88801240/207069192-5667adf7-d909-4bac-b5c7-48deaf41e52d.png">

Choose New Payment from the top right menu.

<img width="836" alt="image27" src="https://user-images.githubusercontent.com/88801240/207069376-c4392942-9fce-4671-8e57-5f3e442a91bb.png">

Enter the amount of the order paid that has been 'paid by credit' preceded with a minus sign (i.e. -$48.0) and choose ‘Pay by Credit’, then ‘Update’.

<img width="862" alt="image28" src="https://user-images.githubusercontent.com/88801240/207069563-80bb5932-36d1-42f8-9a09-80e4cba7ef89.png">

‘Capture’ that payment with the green check mark.

<img width="847" alt="image29" src="https://user-images.githubusercontent.com/88801240/207069762-73f6f730-db4c-4f2a-ab1c-4228e0a1ec40.png">

Now the ‘credit owed’ has been reduced by the correct amount on the credit order.

<img width="817" alt="image30" src="https://user-images.githubusercontent.com/88801240/207069952-80e23eb1-92a8-4654-931d-1bdd316d7be9.png">

And the balance is correct in your customer list.

<img width="832" alt="image31" src="https://user-images.githubusercontent.com/88801240/207070124-9cf2c97c-e1ad-4d95-8764-e7a17173543b.png">

And the Delivery Report will show the up-to-date balance for the customer.  The 2nd order has been paid (so it is no longer negative) and the credit or positive balance has been reduced.

<img width="808" alt="image32" src="https://user-images.githubusercontent.com/88801240/207070339-fb5f4274-746e-4c3d-ad73-91feda7d1557.png">

And, finally, when the customer logs into their account the running balance and credit amount will be accurate. 

<img width="852" alt="image33" src="https://user-images.githubusercontent.com/88801240/207070532-c55e1200-87b1-4bba-a42f-6800b7907daa.png">









