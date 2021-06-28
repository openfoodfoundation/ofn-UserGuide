# Soft Close an Order Cycle

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

From time to time you might find that your enterprise receives more orders than you can physically process \(for example during the panic buying March 2020 or at Christmas\).  

{% hint style="success" %}
It is always better to know the limits of your business and shut your order cycle early than over sell and then have to let people down. 
{% endhint %}

Products will disappear from your shop front when their [stock levels move to zero](../../basic-features/products-1/), but there may be a limit to the number of orders you can pack and deliver in the time frame of your shipping methods and this is not accounted for purely by stock \(processing 100 orders, each containing one item will take longer than one order of 100 items\).

{% hint style="danger" %}
Change the end date and time of an [order cycle](../../basic-features/shopfront/order-cycle/) to the current time will mean customers in the process of checking out will not receive their orders.
{% endhint %}

Therefore we recommend the following method- this way customers who are paying at the time will still have their orders accepted but no others will be taken.

## Process

* Your enterprise can process 100 orders a week- this is a the absolute max.
* Your [listing orders](../../basic-features/orders/view-orders.md#listing-orders) page shows that you have received 95 orders in this order cycle and there are still 2 more days for it to run.

{% hint style="info" %}
Visit Orders in your admin panel and filter results by distributor and order cycle \(highlighted in green below\). The number of orders received is shown under the 'Filter Results' heading \(highlighted in red\).
{% endhint %}

![](../../.gitbook/assets/orders.jpg)

* Add a new default [tag rule](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) by visiting **Enterprises -&gt; Settings -&gt; Tag Rules**. Default: Order cycles tagged '**Closed**' are not visible.

![](../../.gitbook/assets/closedtagrule.jpg)

  
No other tag rules are necessary.

* Edit the [order cycle](../../basic-features/shopfront/order-cycle/order-cycles-for-hubs.md) which is open currently and on page 3 \('Outgoing Products'\) add the tag '**Closed**'

![](../../.gitbook/assets/softcloseoc.jpg)

**Update** and your order cycle will close without disrupting customers in the process of checking out.

{% hint style="danger" %}
This process is only possible at the moment for enterprises which are registered as hubs.
{% endhint %}

