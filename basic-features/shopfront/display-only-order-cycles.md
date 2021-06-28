# Display only shopfront

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

In some cases, shop owners may want to be able to display products in their shop but not actually allow customers to checkout. For example to show their full product range \(which may vary seasonally\), or to give potential customers an idea of the products which will be on offer in the next order cycle, before it opens.

To setup a display only order cycle:

* Open an [Order Cycle](order-cycle/order-cycles-for-hubs.md) as usual, with the products you wish to display and date range for the order cycle to remain open.
* Change the 'Display' state of all your [Payment Methods](payment-methods.md) to 'Back Office Only'.  This can be done from Enterprises -&gt; Settings -&gt; Payment Methods -&gt; Edit:

![](../../.gitbook/assets/displayonlyback.jpg)

Your shop will now be in the ‘display only’ state.   
Below is an example of how the shop appears to customers. It’s clearly marked as closed, but customers can see the product range.

![](../../.gitbook/assets/displayonly.jpg)

{% hint style="warning" %}
When you next open a live order cycle from which you wish to sell produce, you will need to change the Display state of at least one [payment method](payment-methods.md) to 'Checkout and Back Office' or 'Checkout only'.
{% endhint %}

