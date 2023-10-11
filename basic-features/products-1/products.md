# Add products

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

You can either add products to your catalog one by one (detailed below) or by [bulk import](product-and-inventory-import.md), if you have all the relevant details in a .csv file.

## Adding products

Once logged into the Admin Dashboard, select on **Products** on the horizontal blue menu, and then click **+ New Product**.

![](../../.gitbook/assets/addnewproduct.jpg)

This will take you to the New Product page.

![](../../.gitbook/assets/new-product2.png)

**Supplier**&#x20;

Select the enterprise who produces and supplies the product.

{% hint style="info" %}
If you are a producer, this will be you. If you're a hub, remember you’ll only be able to add products to producer profiles which you have created, or if you have been granted permission to manage the products of a producer profile. See [here](../enterprise-profile/create-or-connect-with-your-supplying-producers.md) for more info.
{% endhint %}

**Product name:** This is the title of the product when displayed on the shop front.

{% hint style="info" %}
Products are listed on your shop front alphabetically by product name. This default ordering can be over ruled using the 'Shopfront Category Ordering' field in your [enterprise settings](../enterprise-profile/enterprise-settings.md#shop-preferences).
{% endhint %}

**Units:** Choose the unit the product is sold in? (g, oz, lb, kg, L… or item (bunch, bag, packet))

If you choose g and then enter 1000, the product will be displayed as 1kg for the buyer. Keep in mind that some units of measurement will impact on the operation of certain [enterprise fees](../shopfront/enterprise-fees.md).&#x20;

For example, a [fixed fee by weight](../shopfront/enterprise-fees.md#fee-calculators) can only be applied to products with units of **kg**. In this case, you can enter non-integer unit numbers, such as 0.2 kg, and the product will be displayed as 200 g but will be recorded in kg on the reports and when prices are calculated.

**Value:** Enter the value of units that this product is sold in (for example if it is sold as 100 g then enter '100' here and choose 'g' for 'units'; or if it is sold as bunches of flowers, enter '1' here and 'units= items'.

**Display As:** This field automatically shows you how the units and value fields will display, once you have filled the units and value fields. (i.e. units = kg, value = 2, Display as = 2kg)

{% hint style="info" %}
Note: If you have selected ‘**items**’ as your unit, the **display as** field will change to ‘**item name’**. Fill this in with the type of item it is. (i.e. jar, bottle, or bunch)
{% endhint %}

**Product category:** Select the most appropriate category for this product.  Assigning a product category makes it easier for customers to locate the items they wish to buy; shoppers can filter your product list by category on your shop front.

**Price:** Enter the price for the value noted above. Note, this is the base price charged by the producer and the amount they will receive for each purchase. Mark-ups and fees (for distribution admin etc) are added in [Enterprise Fees](../shopfront/enterprise-fees.md), [Shipping Fees](../shopfront/shipping-methods.md#fee-calculators) and [Payment Methods](../shopfront/payment-methods.md#fee-calculators).&#x20;

{% hint style="info" %}
If your enterprise is registered for tax or you select that this product carries tax, then the price you put here is **inclusive of Tax**. If you select that this product is tax free, the price you enter will be the tax free price.
{% endhint %}

**On hand:** State how much/many of this product you have available and ready for sale.

Use this field if you want to track your stock levels. As customers place orders, the stock level will reduce, and when the in stock amount reaches zero, the product will no longer be visible in your shop. If you don’t want to track inventory in this way, click 'on demand'.

**On demand:** If you select this box, it will indicate that this product is always available. This stops the software from tracking inventory levels for products, and instead it will always show that the product is in stock.

**Image:** Upload a photo of this product.

{% hint style="info" %}
Product images will be displayed on the shopfront in **square (1:1) format**.  We recommend uploading photos with these dimensions.  Landscape and portrait photos will be cropped to square automatically.
{% endhint %}

![](../../.gitbook/assets/bread.jpg)

{% hint style="warning" %}
High resolution images are resized (reduced in pixel dimension) automatically when displayed in your product list dependent on the customer's device.
{% endhint %}

{% hint style="success" %}
We recommend using good quality photos, preferably a real photo of your products rather than the standard image of the web. This makes the product more attractive to the consumer. Always take your photographs in good light.

If you use an image of the web, check that it is free of rights.&#x20;
{% endhint %}

**Tax category:** Select the applicable tax category from the drop-down list. Tax (VAT in the UK) depends on the nature of the product and the country in which you are retailing in.

{% hint style="danger" %}
Tax will only be collected when enterprises have selected 'charges VAT = yes' under their enterprise settings -> Business Details.
{% endhint %}

**Product description:** Tell your customers a little bit about this product. You might like to include a story about the specific tomato variety, include hyperlinks to any certification it may have etc.

{% hint style="info" %}
Don't forget to click on the "create" or "create and add new" button at the bottom of the page once all mandatory fields have been entered (those indicated by a red asterisk).&#x20;
{% endhint %}

A short demonstration of the steps outlined above:

![](../../.gitbook/assets/productsadd.gif)

When you have finished creating a product, you are redirected to the "products" page where you will find all your products:

![](../../.gitbook/assets/productspage.jpg)

{% hint style="success" %}
Products listed in your admin panel can be sorted alphabetically by name (click on 'NAME' in the table to implement this).
{% endhint %}

This is how your products will display to your customers on the shop front:

![](../../.gitbook/assets/productview.jpg)

## Listing Similar / variations of a Product&#x20;

If you are listing a product which comes in a number of different options (say different sizes or flavours, each of which may or may not have a different price), it is best to create a ‘variant’ for that product, rather than creating multiple, separate products.  Creating product variants is discussed fully on the [next page](product-variants.md).

{% hint style="success" %}
Variants are useful if, for example, you sell lemons singularly as well as in 'packs' of 5. Rather than have two product listings the two options can be available for the same product.
{% endhint %}

If you would like to create a SIMILAR product then you can duplicate products by selecting the double page icon to the right of an item (red box). By subsequently selecting the pencil and paper icon (green box) the copied product can be edited and the details amended for the second item.

![](../../.gitbook/assets/productspagecopy.jpg)

## Edit your products

Once a product is created, the best place to quickly edit its attributes, such as quantity, price and stock level, is through the listing products page shown above.

To edit images, product descriptions, categories and more you can select the edit symbol (pen on paper icon) to the right of the product in question in the table. This will bring up the following page:

![](../../.gitbook/assets/editproduct.jpg)

From the right hand menu, you might like to add

* **Properties or labels** to your products.  This allows customers to find your items when searching for specific criteria (eg. certified Organic) and highlights specific qualities your products may have. Find out more [here](product-properties.md).
* **Group Buy:** This enables you to manage and organise sales of products in bulk lots. Read more about this [here](group-buy-for-bulk-ordering.md).
* **Search** terms described [below](products.md#search-keywords).

For tips on how to manage sales of **"irregular" products** such as meat or large vegetables sold in units but costed by weight, please read [here](pricing-irregular-items-kg.md).

{% hint style="danger" %}
**Do not edit** the **Permalink** field.  This connects your product internally to an entry in the OFN database.  Editing can corrupt the product entry.
{% endhint %}

### Search keywords

Customers can filter your products to identify what they wish to purchase based on their product category and product properties.  The filters are found to the right hand side of the shop page.

![](../../.gitbook/assets/searchfilter.jpg)

Some customers will use the Search box at the top left of the page to locate their produce.  The following fields are searched by this box:

* Product name
* Variant name
* Producer name
* Search keywords

Keywords can be added by visiting **Edit Product -> Search**.  Keywords entered into the top box (in red below) are reviewed by the platform if the customer uses the 'Search' field on your shop front.  Those entered into the second box (in green below) are searched by external search engines on the internet (for example Google).&#x20;

![](../../.gitbook/assets/searchedit.jpg)

The 'Notes' section is not an active field. It is a handy box for you to 'make a note' of a seasonal search term which may be very effective/ineffective one year, so that you don't forget.
