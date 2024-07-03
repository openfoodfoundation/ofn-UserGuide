# Add products

You can either add products to your catalog one by one (detailed below) or by [bulk import](product-and-inventory-import.md), if you have all the relevant details in a .csv file.

## Adding products

Once logged into the Admin Dashboard, select **Products** on the main horizontal menu and then click **+ New Product**.

![](<../../.gitbook/assets/add product.jpg>)

This will take you to the New Product page.

![](<../../.gitbook/assets/new product.jpg>)

**Supplier**&#x20;

Select the enterprise who produces and supplies the product.

{% hint style="info" %}
If you are a producer, this will be you. If you're a hub, remember you’ll only be able to add products to producer profiles which you have created, or if you have been granted permission to manage the products of a producer profile. See [here](../enterprise-profile/create-or-connect-with-your-supplying-producers.md) for more info.
{% endhint %}

**Product name:** This is the title of the product when displayed on the shop front.

{% hint style="info" %}
Products are listed on your shop front alphabetically by product name. This default ordering can be overruled using the 'Shopfront Category Ordering' field in your [enterprise settings](../enterprise-profile/enterprise-settings.md#shop-preferences).
{% endhint %}

**Units:** Choose the unit the product is sold in (g, oz, lb, kg, L… or item (bunch, bag, packet))

If you choose g and then enter 1000, the product will be displayed as 1kg for the buyer. Keep in mind that some units of measurement will impact on the operation of certain [enterprise fees](../shopfront/enterprise-fees.md).&#x20;

For example, a [fixed fee by weight](../shopfront/enterprise-fees.md#fee-calculators) can only be applied to products with units of **kg**. In this case, you can enter non-integer unit numbers, such as 0.2 kg, and the product will be displayed as 200 g but will be recorded in kg on the reports and when prices are calculated.

**Value:** Enter the value of units that this product is sold in (for example if it is sold as 100 g then enter '100' here and choose 'g' for 'units'; or if it is sold as bunches of flowers, enter '1' here and 'units= items'.

**Display As:** This field automatically shows you how the units and value fields will display, once you have filled the units and value fields. (i.e. units = kg, value = 2, Display as = 2kg)

{% hint style="info" %}
Note: If you have selected ‘**items**’ as your unit, the **display as** field will change to ‘**item name’**. Fill this in with the type of item it is. (i.e. jar, bottle, or bunch)
{% endhint %}

**Product category:** Select the most appropriate category for this product.  Assigning a product category makes it easier for customers to locate the items they wish to buy; shoppers can filter your product list by category on your shop front.

**Price:** Enter the price for the value noted above. Note that this is the base price charged by the producer and the amount they will receive for each purchase. Mark-ups and fees (for distribution admin etc) are added in [Enterprise Fees](../shopfront/enterprise-fees.md), [Shipping Fees](../shopfront/shipping-methods.md#fee-calculators) and [Payment Methods](../shopfront/payment-methods.md#fee-calculators).&#x20;

{% hint style="info" %}
If the product is taxable then the price you put here should be **inclusive of Tax** (UK/EU enterprises) OR **exclusive of Tax** (USA and Canada enterprises). How taxes are applied depend on the tax rules for the country where you are operating, if you are unsure when to include taxes contact your local instance. \
\
If you select that this product is tax free, the price you enter will be the tax free price.
{% endhint %}

**Unit Price:** This will be automatically calculated for you from the unit and price supplied.  If the units are in weight or volume then the unit price will be cost per kg/L etc. If the units are in 'items' then the unit price will be cost per item.

**On hand:** State how much/many of this product you have available and ready for sale.

Use this field if you want to track your stock levels. As customers place orders, the stock level will reduce, and when the in stock amount reaches zero, the product will no longer be visible in your shop. If you don’t want to track inventory in this way, click 'on demand'.

**On demand:** If you select this box, it will indicate that this product is always available. This stops the software from tracking inventory levels for products and instead it will always show that the product is in stock.

**Image:** Upload a photo of this product.

{% hint style="info" %}
Product images will be displayed on the shopfront in **square (1:1) format**.  We recommend uploading photos with these dimensions. Landscape and portrait photos will be cropped to square automatically.
{% endhint %}

![Product with units of weight](../../.gitbook/assets/productweightunit-price.jpg)

![Product with units of 'items' (pie)](../../.gitbook/assets/productitemunit-price.jpg)

{% hint style="warning" %}
High resolution images are resized (reduced in pixel dimension) automatically when displayed in your product list dependent on the customer's device.
{% endhint %}

{% hint style="success" %}
We recommend using good quality photos, preferably a real photo of your products rather than a standard image off the internet. This makes the product more attractive to the consumer. Always take your photographs in good light.

If you use an image off the internet, check that it is free of rights.&#x20;
{% endhint %}

**Tax category:** Select the applicable tax category from the drop-down list. Tax (VAT in the UK) depends on the nature of the product and the country in which you are retailing.

{% hint style="danger" %}
Tax will only be collected when enterprises have selected 'charges VAT = yes' under their Enterprise Settings -> Business Details.
{% endhint %}

**Product description:** Tell your customers a little bit about this product. You might like to include a story about the specific tomato variety, include hyperlinks to any certification it may have etc.

{% hint style="info" %}
Don't forget to click on the "create" or "create and add new" button at the bottom of the page once all mandatory fields have been entered (those indicated by a red asterisk).&#x20;
{% endhint %}

A short demonstration of the steps outlined above:

![](<../../.gitbook/assets/create product.gif>)

When you have finished creating a product, you are redirected to the "products" page where you will find all your products:

![](<../../.gitbook/assets/bulk page edit new.jpg>)

To customise the format of this table to only display information relevant to your organisation you can choose which columns are shown using the drop down menu under 'Columns'

<figure><img src="../../.gitbook/assets/bulk edit columns.jpg" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
SKU (or product codes) can be added in the 'Product Code' column for each item if desired (for example this may be useful if stocking dried/bulk/toiletry items from a wholesale catalogue).
{% endhint %}

This is how your products will display to your customers on the shop front:

![](../../.gitbook/assets/productbreakdown.jpg)

## Listing similar/variations of a Product&#x20;

If you are listing a product which comes in a number of different options (say different sizes or flavours, each of which may or may not have a different price), it is best to create a ‘variant’ for that product, rather than creating multiple separate products. Creating product variants is discussed fully on the [next page](product-variants.md).

{% hint style="success" %}
Variants are useful if, for example, you sell lemons singularly as well as in 'packs' of 5. Rather than have two product listings the two options can be available for the same product.
{% endhint %}

To edit or replicate a product, simply click on the three vertical dots in the 'Actions' column for the product row in question.  The two options: Edit (highlighted in green below) and Clone (highlighted in red below) become available.

![](<../../.gitbook/assets/edit or clone.jpg>)

## Edit your products

Once a product is created the best place to quickly edit its attributes, such as quantity, price and stock level, is through the listing products page shown above.

To edit images, product descriptions, categories and more you can select edit, from the actions column to the right of the product in question in the table. This will bring up the following page:

![](<../../.gitbook/assets/edit product.jpg>)

From the right hand menu, you might like to add:

* **Properties or labels** to your products. This allows customers to find your items when searching for specific criteria (e.g. certified Organic) and highlights specific qualities your products may have. Find out more [here](product-properties.md).
* **Group Buy:** This enables you to manage and organise sales of products in bulk lots. Read more about this [here](group-buy-for-bulk-ordering.md).
* **Search** terms described [below](products.md#search-keywords).

For tips on how to manage sales of **"irregular" products** such as meat or large vegetables sold in units but costed by weight, please read [here](pricing-irregular-items-kg.md).

{% hint style="danger" %}
**Do not edit** the **Permalink** field. This connects your product internally to an entry in the OFN database. Editing can corrupt the product entry.
{% endhint %}

### Search keywords

Customers can filter your products to identify what they wish to purchase based on their product category and product properties. The filters are found to the right hand side of the shop page.

![](<../../.gitbook/assets/searchfilter (1).jpg>)

Some customers will use the Search box at the top left of the page to locate their produce. The following fields are searched by this box:

* Product name
* Variant name
* Producer name
* Search keywords

Keywords can be added by visiting **Edit Product -> Search**.  Keywords entered into the top box (in red below) are reviewed by the platform if the customer uses the 'Search' field on your shop front. &#x20;

![](<../../.gitbook/assets/search keywords.jpg>)

The 'Notes' section is not an active field. It is a handy box for you to 'make a note' of a seasonal search term which may be very effective/ineffective one year, so that you don't forget.
