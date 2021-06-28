# Making a producer profile searchable by product category

{% hint style="danger" %}
![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&token=aef3eea2-4d60-4d24-99ec-6edbda36b45c)--&gt;​![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&token=9bbe895b-2aa1-40da-8221-01fb74558b92) Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF~A)!
{% endhint %}

When customers come to the Open Food Network they are able to search for producers by name or location. They are also able to filter the producer profiles according to what kinds of products the producers stock \(see below\). 

![](../../.gitbook/assets/filter-by-product.png)

Producers with online shops on the OFN have products in the system, which get picked up by the search filter tool. However, producers who don’t have an OFN shop \(just a profile\) won’t be searchable in this way, unless they add some fake products into the system. By adding a dummy product for each product category that you want to be searchable under, you’ll show up when customers search for your products.

Here’s how to do this…

Click **Products** in the horizontal blue menu, and then click **+ New Product** to add your dummy products.

![](../../.gitbook/assets/addnewproduct.jpg)

Because you don’t have an OFN shopfront, this product won’t be visible anywhere. Therefore you can call it whatever you like, and set the price and units to anything. The important thing is that you select the correct **Product Category** that you wish to be found under. Below is an example of a dummy meat product. This producer’s profile will now show if a customer searches for producers of meat.

![](../../.gitbook/assets/dummy-meat-product.png)

Their summary profile will also indicate that they sell meat products \(below\).

![](../../.gitbook/assets/meat.png)



