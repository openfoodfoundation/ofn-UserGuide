---
description: >-
  This page explains how both producers can to import product details and
  distributors can set up their hub inventory in bulk.
---

# Product and Inventory import



The product and inventory import tool lets you upload a .csv file to add and update your stock. This can be much quicker and efficient than adding or updating products one by one. For producers who already update a catalogue of their products in an Excel spreadsheet regularly, this can save a lot of time!

The product and inventory import tool can be found by clicking **Products** in the horizontal blue menu, and **product import** in the green menu.

There's four main ways you can use the tool:

1. Import new [products](./)
2. Update existing product details
3. Import products to a new shop/hub [inventory](inventory-tool.md)&#x20;
4. Update products in a shop/hub inventory

In all cases the process involves downloading a CSV template, filling in the fields and then uploading your CSV file back into OFN.

{% hint style="warning" %}
**Important note on CSV files**: Microsoft Excel does not open .csv files directly.\
If you can, we suggest you download the free Libre Office suite [https://www.libreoffice.org/download/download/](https://www.libreoffice.org/download/download/)\
With Libre Office Calc, you will be able to open and edit CSV very easily and save them in the right encoding format UTF-8.\
If you can't use Libre Office, then in order to open a CSV file in Microsoft Excel, you need to follow the following steps: [https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba](https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba)
{% endhint %}

{% hint style="danger" %}
Not all fields can be captured and uploaded/updated using this tool. Currently [Images](products.md), [Properties](product-properties.md) and [Group Buy ](group-buy-for-bulk-ordering.md)Settings must be uploaded manually for each product.

We hope to include these in future developments.
{% endhint %}

## Import New Products

Use these instructions if you want to add new products to a producer's profile.

{% hint style="success" %}
You can simultaneously upload new products and update existing products with a single CSV upload. The instructions in this guide are separated for clarity but you can combine new products and updates in the same spreadsheet.
{% endhint %}

### Prepare the CSV file for import

Firstly, download the **Product List Template CSV** file from the [**Product Import**](https://openfoodnetwork.org.uk/admin/product\_import) page and open it with Libre Office, Excel or equivalent.

You'll see that the template gives all the column headings required to successfully import a product. Each row is for a new product or variant. Below is a description of how to fill in each column.

{% hint style="danger" %}
**N.B.** All fields are case sensitive e.g. you must use mL and Dairy, not ml or dairy.
{% endhint %}

<table><thead><tr><th width="195">Column Title</th><th width="110">Required?</th><th width="259">Description</th><th>Example</th></tr></thead><tbody><tr><td>producer</td><td>Y</td><td>The name of the producer profile that this product will be assigned to</td><td>Four Mile Farm</td></tr><tr><td>sku</td><td>N</td><td>The SKU code for this product</td><td>AD001265</td></tr><tr><td>name</td><td>Y</td><td>The name of the product</td><td>Yoghurt</td></tr><tr><td>display_name</td><td>N</td><td>You can use this field to give unique names to different  variants. If you're not creating a variant, leave this field blank.</td><td>Raspberry Yoghurt</td></tr><tr><td>category</td><td>Y</td><td>The product category of the item. Categories are listed on the <a href="https://openfoodnetwork.org.uk/admin/product_import">Product Import</a> page</td><td>Dairy</td></tr><tr><td>description</td><td>N</td><td>An optional description of the product</td><td>This Yoghurt is made from local raspberries</td></tr><tr><td>units</td><td>Y</td><td>The weight, volume or quantity value</td><td>500</td></tr><tr><td>unit_type</td><td>Maybe</td><td>The unit the product is sold in (g, kg, T, mL, L). If sold as an item, (e.g. bunch) leave this blank</td><td>g</td></tr><tr><td>variant_unit_name</td><td>Maybe</td><td>If the product is sold as an item (e.g loaf, bunch, pumpkin) write the item type here</td><td>Bunch</td></tr><tr><td>price</td><td>Y</td><td>The price of the product. If the item carries tax, this must be the tax inclusive price.</td><td>3.70</td></tr><tr><td>on_hand <br>(stock count)</td><td>Maybe</td><td>If you have limited stock for the product, type the stock level here. If you have unlimited stock available, leave this blank</td><td>40</td></tr><tr><td>available_on</td><td>N</td><td>Leave this blank</td><td></td></tr><tr><td>on_demand (unlimited stock)</td><td>Y</td><td>If you have unlimited stock available for this product, type 1. If you enter a number in on_hand <em>and</em> 1 in unlimited, the product will be marked as unlimited.</td><td>1</td></tr><tr><td>shipping_category</td><td>Y</td><td>The shipping category of the product. Categories are listed on the <a href="https://openfoodnetwork.org.uk/admin/product_import">Product Import</a> page</td><td></td></tr><tr><td>tax_category</td><td>N</td><td>The tax category of the product. Categories are listed on the <a href="https://openfoodnetwork.org.uk/admin/product_import">Product Import</a> page</td><td>Full Rate</td></tr></tbody></table>

#### Import Product Variants

In the import process, variants are distinguished by the units (such as raspberries sold in 200g and 500g packs) or display\_name fields (such as apples sold in multiple varieties). As long as the product name is the same, the rows will be imported as variants. For products sold as items, the unit\_type must be the same across variants (e.g. rolls below).&#x20;

| name            | display\_name    | price | units | unit\_type |
| --------------- | ---------------- | ----- | ----- | ---------- |
| Raspberries     |                  | 3.60  | 200   | g          |
| Raspberries     |                  | 4.80  | 300   | g          |
| Apples          | Golden Delicious | 3.60  | 500   | g          |
| Apples          | Pink Lady        | 4.80  | 500   | g          |
| Wholemeal rolls |                  | 0.40  | 2     | rolls      |
| Wholemeal rolls |                  | 1.00  | 5     | rolls      |

The image below shows how these products will display in the shop. Note that the 'name' field becomes the primary heading, and the 'display\_name' field and/or the units becomes the secondary heading.

![](../../.gitbook/assets/samedisplayname.jpg)

![](../../.gitbook/assets/differentdisplaynames.jpg)

#### Unit type examples

Below are some examples to show how products with different units (g, ml, kg and items) should be uploaded.

<table data-header-hidden><thead><tr><th width="121">producer</th><th>name</th><th width="105">category</th><th width="73">price</th><th width="75">units</th><th width="110" align="center">unit_type</th><th align="center">variant_unit_name</th></tr></thead><tbody><tr><td>producer</td><td><strong>name</strong></td><td><strong>category</strong></td><td><strong>price</strong></td><td><strong>units</strong></td><td align="center"><strong>unit_type</strong></td><td align="center"><strong>variant_unit_name</strong></td></tr><tr><td>Sue's Salads</td><td>Salad Bag</td><td>Vegetables</td><td>3.50</td><td>500</td><td align="center">g</td><td align="center"></td></tr><tr><td>Henry Orchards</td><td>Fruit Juice</td><td>Drinks</td><td>3.50</td><td>300</td><td align="center">ml</td><td align="center"></td></tr><tr><td>Fernwell Produce</td><td>Potatoes</td><td>Vegetables</td><td>9.50</td><td>5</td><td align="center">kg</td><td align="center"></td></tr><tr><td>Tom's Bakery</td><td>Wholemeal Bread</td><td>Baked goods</td><td>3.00</td><td>1</td><td align="center"></td><td align="center">loaf</td></tr></tbody></table>

### Import the CSV

Once you have filled out the **Product List Template CSV** you are ready to upload it into OFN.

1. Go to **Products** >  **Product Import.**
2. Select import type:  **Product List**
3.  **Select a spreadsheet to upload:** select the CSV file you've updated with your product info.

    Because you are uploading new products, you can leave the '_Set stock to zero for all exiting products not present in the file_' checkbox unchecked (see next section for an explanation of this feature).
4. Click **Upload**.

You'll be shown a summary of your upload, including any errors. You'll also be told how many products you are creating and how many you are updating. If you're happy with the upload results, click **save**.

{% hint style="success" %}
It's good practice to check that the products uploaded/updated as you intended.
{% endhint %}

You can then upload another spreadsheet or go to the products page to view your new products.

## Update Existing Product Details

The instructions below relate to updating the details of an existing product. This tool is intended as a quick way to update product prices and stock levels.

{% hint style="info" %}
You can simultaneously upload new products and update existing products with a single CSV upload. The instructions in this guide are separated for clarity but you can combine new products and updates in the same spreadsheet.
{% endhint %}

### Prepare the CSV file for import

The process for updating product details is similar to [uploading new products](product-and-inventory-import.md#import-new-products). The first step is to download the **Product List Template** and fill in the product names and the supplier names. If you have this spreadsheet on hand from a previous upload even better.

The system requires seven fields to correctly identify the product you want to update. There are four fields which can be updated and four fields which cannot using this tool.

| Required fields (you can't update)   | Fields you can update | Fields that won't update and aren't required |
| ------------------------------------ | --------------------- | -------------------------------------------- |
| \*producer                           | sku                   | ^variant\_unit\_name                         |
| \*name                               | price                 | ^tax\_category                               |
| ^category                            | in\_stock             | ^shipping\_category                          |
| \*units                              | unlimited             | ^description                                 |
| ^unit\_type (if applicable)          |                       |                                              |
| ^variant\_unit\_name (if applicable) |                       |                                              |
| \*display\_name                      |                       |                                              |

_^ if you try to update these fields you'll see an error message_

_\*If you try to update these fields you'll actually create new products or variants, rather than update an existing product._

Once complete, the .csv can be [imported](product-and-inventory-import.md#import-the-csv) in the same manner as for new products.

{% hint style="info" %}
**Set stock to zero for all exiting products not present in the file:**\
If you select this tickbox the system will set the 'In Stock' value to zero for _all products already in your product list that are not in the product import file._\
If a product was 'Unlimited', removing it from the import will mark the item as 0 in stock.
{% endhint %}

## Import New Inventory or update your inventory

## Import New Inventory or update your inventory

Use these instructions if you want to add or update new products to your [inventory](inventory-tool.md).

### Prepare the CSV file for import

Firstly, download the **Inventory Template CSV** file from the **Product Import** page.

You'll see that the template gives all the column headings required to successfully import a product. Each row is for a new product or variant. Below is a description of how to fill in each column.

{% hint style="info" %}
**N.B.** that all fields are case sensitive e.g. you must use mL not ml , or Dairy not dairy.
{% endhint %}

| Column Title           | Required? | Description                                                                                                                                                                                                                                              | Example                              |
| ---------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| producer               | Y         | This is the name of the producer profile that this inventory item will be assigned to                                                                                                                                                                    | Four Mile Farm                       |
| distributor            | Y         | This is the name of the hub profile the inventory item will be assigned to                                                                                                                                                                               | Demo Hub                             |
| name                   | Y         | This is the name of the product                                                                                                                                                                                                                          | Yoghurt                              |
| display name           | N         | This field applies if you are creating variants (see instructions below). If you're not creating a variant leave this field blank.                                                                                                                       | Rasberry Yoghurt                     |
| variant\_unit\_name    | Y         | If the product is sold as an item (e.g loaf, bunch, pumpkin) write the item type here                                                                                                                                                                    | Bunch                                |
| units                  | Y         | The weight, volume or quantity value                                                                                                                                                                                                                     | 500                                  |
| unit\_type             | Y         | What unit is it sold in (g, kg, T, mL, L)? If sold as an item (e.g. bunch) leave blank                                                                                                                                                                   | g                                    |
| price                  | Y         | The price of the product. If the item carries tax, this must be the tax inclusive price.                                                                                                                                                                 | 3.70                                 |
| On\_Hand  (in\_stock)  | Y         | Please check the rules for unlimited below                                                                                                                                                                                                               | leave blank as unlimited is set to 1 |
| On\_demand (unlimited) | Y         | If blank - Read as "Use producer stock settings", so "in\_stock" should be blank.   If you set it to "1" - Read as unlimited of "Yes", so "in\_stock" should be blank.     If you set it to "0" - Read as unlimited of "No", so "in\_stock" is required. | 1                                    |
| sku                    | N         | The SKU code for this product                                                                                                                                                                                                                            | AD001265                             |

### Import the CSV <a href="#import-the-csv" id="import-the-csv"></a>

Once you have filled out the **Inventory Template CSV** you are ready to upload it into OFN.

1. Go to **Products** >  **Product Import.**
2. **Select import type:** Select Inventories
3. **Select a spreadsheet to upload**
4. Click **Upload**.

You'll be shown a summary of your upload, including any errors. You'll also be told how many products you are creating and how many you are updating. If you're happy with the upload results, click **save**.

{% hint style="success" %}
It's good practice to check that the products uploaded/updated as you intended.
{% endhint %}

**N.B.** All fields are case sensitive so you must use the exact category and unit\_type names, e.g. 'mL' and 'Dairy' instead of 'ml' or 'dairy'.
