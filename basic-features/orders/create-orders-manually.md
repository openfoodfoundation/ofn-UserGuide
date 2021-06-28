# Create orders manually

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

Sometimes you may wish to manually put an order into the system. This may be on behalf of a customer, or so that your reports will capture an order from a different sales stream. You can create an order by going to **Orders** and clicking on the **+ New Order** button.

![](../../.gitbook/assets/manorder1.jpg)

There you are then lead through a step-by-step process to place the order:

![](../../.gitbook/assets/manorder2.jpg)

Firstly you will be prompted to select the distributor that the order will be placed with.   
Next you will need to select the order cycle that you want the order to be placed in. You choice of order cycle will dictate which products will be available to be added into the order and the fees applied.  
You will then be redirected to the following page where you can select products. You must type at least the first 3 characters of the product for it to appear as an option in the drop down list:

![](../../.gitbook/assets/manorder3.jpg)

After finding the product you'd like to order, enter the quantity and click the **+** button to the right of the product to add it to the cart.

![](../../.gitbook/assets/manorder4.jpg)

Once a product is added you can edit \(quantity for example\) by selecting the pen and paper icon to the right of the item:

![](../../.gitbook/assets/manorder5.jpg)

After editing any aspect of the cart, click **update and recalculate fees** to update the price.

The next step is to add in the customer’s details \(right hand menu, second option down\). If it is a customer who is on your customer list, you can select them from the dropdown menu, otherwise you can fill in the customer’s details details and check them out as a guest.

![](../../.gitbook/assets/manorder6.jpg)

Click **Update** and go back to Order Details \(top option on right hand menu\).  You will now be able to select a shipping method for the customer.

![](../../.gitbook/assets/manorder7.jpg)

Tick to update changes and cross to cancel.

{% hint style="danger" %}
You can not select a shipping method prior to adding the customer's details.
{% endhint %}

The final step is to add the customer’s payment method.  This is found from the bottom option of the right hand menu:

![](../../.gitbook/assets/manorder8.jpg)

{% hint style="warning" %}
Note, if you opt for a [payment method](../shopfront/payment-methods.md) provided by **Stripe** then you will be directed to input the customer's card details.  
 ![](../../.gitbook/assets/stripeextra.jpg)  
{% endhint %}

{% hint style="danger" %}
You should NEVER write down a customer's card details.
{% endhint %}

{% hint style="success" %}
Best practice is to complete the above form directly into a computer/tablet/mobile device while the customer reads out the numbers over the phone.
{% endhint %}

{% hint style="danger" %}
You will not be able to opt for a [Payment Method](../shopfront/payment-methods.md) provided by **PayPal** for an order created manually.

![](../../.gitbook/assets/paypalnewpayment%20%281%29.jpg) 
{% endhint %}

Clicking **update** will finalise this order and send an email confirmation to the customer.

