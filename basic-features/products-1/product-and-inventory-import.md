---
description: >-
  Esta página explica cómo los productores pueden importar detalles del producto
  y los distribuidores pueden configurar el inventario del hub/nodo de forma
  masiva
---

# Importación de Productos e Inventarios

La herramienta de importación de productos e inventario le permite cargar un archivo .csv para agregar y actualizar sus existencias. Esto puede ser mucho más rápido y eficiente que agregar o actualizar productos uno por uno. Para los productores que ya actualizan un catálogo de sus productos en una hoja de cálculo de Excel con regularidad, ¡esto puede ahorrar mucho tiempo!

La herramienta de importación de productos e inventario se puede encontrar haciendo clic en Productos en el menú azul horizontal e **Importación de productos** en el menú verde.

Hay cuatro formas principales de utilizar la herramienta:

1. Importar nuevos [productos](./)
2. Actualizar los detalles del producto existente
3. Importar productos a un nuevo [inventario](inventory-tool.md) de tienda / hub\(nodo\)
4. Actualizar productos en un inventario de tienda / hub\(nodo\)

{% hint style="info" %}
Si necesita esta funcionalidad, infórmeselo a [su OFN local](https://openfoodnetwork.org/ofn-local/). Agradecemos sus comentarios.
{% endhint %}

En todos los casos, el proceso implica descargar una plantilla csv, completar los campos y luego cargar su archivo csv nuevamente en OFN.

{% hint style="warning" %}
**Nota importante sobre archivos CSV**: Microsoft Excel no abre archivos .cvs directamente.

Si puede, le sugerimos que descargue la suite Libre Office gratuita [https://www.libreoffice.org/download/download/](https://www.libreoffice.org/download/download/)

Con Libre Office Calc, podrá abrir y editar CSV fácilmente y guardarlos en el formato de codificación correcto UTF-8.

Si no puede usar Libre Office, para abrir un archivo CSV en Microsoft Excel, debe seguir los siguientes pasos: [https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba](https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba)
{% endhint %}

{% hint style="danger" %}
No todos los campos se pueden capturar y cargar / actualizar con esta herramienta. Actualmente, las [Imágenes](products.md), [Propiedades](product-properties.md) y la [Configuración de Compra Grupal](group-buy-for-bulk-ordering.md) deben cargarse manualmente para cada producto.

Esperamos incluirlos en desarrollos futuros.
{% endhint %}

## Importar Nuevos Productos

Utilice estas instrucciones si desea agregar nuevos productos al perfil de un productor. 

{% hint style="success" %}
Puede cargar nuevos productos y actualizar productos existentes simultáneamente con una sola carga de CSV. Las instrucciones de esta guía están separadas para mayor claridad, pero puede combinar nuevos productos y actualizaciones en la misma hoja de cálculo.
{% endhint %}

### Prepare el archivo CSV para importar

En primer lugar, descargue el archivo CSV **Plantilla de Lista de Productos** de la página de **Importación de Productos** y ábralo con Libre Office \(Excel o equivalente\).

Verá que la plantilla proporciona todos los encabezados de columna necesarios para importar correctamente un producto. Cada fila es para un nuevo producto o variante. A continuación se muestra una descripción de cómo completar cada columna.

{% hint style="danger" %}
Tenga en cuenta que todos los campos distinguen entre mayúsculas y minúsculas. P.ej. debe usar mL no ml, o Lácteos no lácteos.
{% endhint %}

<table>
  <thead>
    <tr>
      <th style="text-align:left">T&#xED;tulo de la Columna</th>
      <th style="text-align:left">&#xBF;Requirido?</th>
      <th style="text-align:left">Descripci&#xF3;n</th>
      <th style="text-align:left">Ejemplo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">producer</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Este es el nombre del perfil de productor al que se asignar&#xE1; este
        producto</td>
      <td style="text-align:left">Four Mile Farm</td>
    </tr>
    <tr>
      <td style="text-align:left">sku</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">El c&#xF3;digo SKU de este producto</td>
      <td style="text-align:left">AD001265</td>
    </tr>
    <tr>
      <td style="text-align:left">name</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Este es el nombre del producto</td>
      <td style="text-align:left">Yoghurt</td>
    </tr>
    <tr>
      <td style="text-align:left">display name</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Este campo se aplica si est&#xE1; creando variantes (consulte las instrucciones
        a continuaci&#xF3;n). Si no est&#xE1; creando una variante, deje este campo
        en blanco</td>
      <td style="text-align:left">Rasberry Yoghurt</td>
    </tr>
    <tr>
      <td style="text-align:left">category</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">&#xBF;A qu&#xE9; categor&#xED;a pertenece este producto? Las categor&#xED;as
        disponibles se enumeran en la p&#xE1;gina de importaci&#xF3;n de productos</td>
      <td
      style="text-align:left">L&#xE1;cteos</td>
    </tr>
    <tr>
      <td style="text-align:left">units</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">El peso, el volumen o el valor de la cantidad</td>
      <td style="text-align:left">500</td>
    </tr>
    <tr>
      <td style="text-align:left">unit_type</td>
      <td style="text-align:left">Maybe</td>
      <td style="text-align:left">&#xBF;En qu&#xE9; unidad se vende (g, kg, T, mL, L)? Si se vende como
        un art&#xED;culo (p. Ej., Manojo) d&#xE9;jelo en blanco</td>
      <td style="text-align:left">g</td>
    </tr>
    <tr>
      <td style="text-align:left">variant_unit_name</td>
      <td style="text-align:left">Maybe</td>
      <td style="text-align:left">Si el producto se vende como un art&#xED;culo (por ejemplo, pan, manojo,
        calabaza) escriba el tipo de art&#xED;culo aqu&#xED;</td>
      <td style="text-align:left">Manojo</td>
    </tr>
    <tr>
      <td style="text-align:left">price</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">El precio del producto. Si el art&#xED;culo tiene impuestos, este debe
        ser el precio con impuestos incluidos.</td>
      <td style="text-align:left">3.70</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>On_Hand</p>
        <p>(in_stock)</p>
      </td>
      <td style="text-align:left">Maybe</td>
      <td style="text-align:left">Si tiene inventario limitado para el tipo de producto, indique el nivel
        de inventario aqu&#xED;. Si tiene existencias infinitas disponibles (siempre
        puede obtenerlas) ingrese 0 y use la columna ilimitada</td>
      <td style="text-align:left">40</td>
    </tr>
    <tr>
      <td style="text-align:left">available_on</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Dejar en blanco</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">On_demand (unlimited)</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">Si tiene existencias infinitas disponibles para este producto, escriba
        1, si est&#xE1; usando on_hand d&#xE9;jelo en blanco. Si ingresa un n&#xFA;mero
        en in_stock <em>y</em> 1 en ilimitado, el producto ser&#xE1; ilimitado</td>
      <td
      style="text-align:left">1</td>
    </tr>
    <tr>
      <td style="text-align:left">shipping_category</td>
      <td style="text-align:left">Y</td>
      <td style="text-align:left">&#xBF;En qu&#xE9; categor&#xED;a de env&#xED;o se incluye este producto?
        Las categor&#xED;as de env&#xED;o disponibles se enumeran en la p&#xE1;gina
        Importaci&#xF3;n de productos</td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">tax_category</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Si el precio de su producto incluye el tipo de impuesto IVA, si no, d&#xE9;jelo
        en blanco</td>
      <td style="text-align:left">IVA</td>
    </tr>
    <tr>
      <td style="text-align:left">description</td>
      <td style="text-align:left">N</td>
      <td style="text-align:left">Puede crear una descripci&#xF3;n, pero no puede actualizarla. Aseg&#xFA;rese
        de que el texto que escribi&#xF3; coincida con la descripci&#xF3;n actual
        en caso de una actualizaci&#xF3;n</td>
      <td style="text-align:left">Este yogur est&#xE1; elaborado con frambuesas locales</td>
    </tr>
  </tbody>
</table>

#### Import Product Variants

In the import process, variants are distinguished by the units \(such as salad sold as 500 g and 750 g bags\) or display\_name fields \(such as a yoghurt sold in multiple flavours\).  As long as the product name is the same, the rows will be imported as variants.  The example below shows a salad that comes in 500g and 750g variants, and a yoghurt that comes in multiple flavours.

| name | display\_name | price | units | unit\_type |
| :--- | :--- | :--- | :--- | :--- |
| Salad Bag |  | 3.50 | 500 | g |
| Salad Bag |  | 5.50 | 750 | g |
| Yoghurt | Banana | 4 | 500 | g |
| Yoghurt | Strawberry | 4 | 500 | g |

The image below shows how these products will display in the shop. Note that the 'name' field becomes the primary heading, and the 'display\_name' field becomes the secondary heading. In the case of the Salad Bag, the 'display\_name' field is blank, so the 'name' is used by default.

![](../../.gitbook/assets/image%20%281%29.png)

#### Unit type examples

Below are some examples to show how products with different units \(g, ml, kg and items\) should be uploaded.

| producer | **name** | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| :--- | :--- | :--- | :--- | :--- | :---: | :---: |
| Sue's Salads | Salad Bag | Vegetables | 3.50 | 500 | g |   |
| Henry Orchards | Fruit Juice | Drinks | 3.50 | 300 | ml |   |
| Fernwell Produce | Potatoes | Vegetables | 9.50 | 5 | kg |   |
| Tom's Bakery | Wholemeal Bread | Baked goods | 3.00 | 1 |   | loaf |

### Import the CSV

Once you have filled out the **Product List Template CSV** you are ready to upload it into OFN. 

1. Go to **Products** &gt;  **Product Import.**
2. **Select import type:** Select Product List
3. **Select a spreadsheet to upload:** Find the csv file you wish to upload.

   Because you are uploading new products, you can leave the '_Set stock to zero for all exiting products not present in the file_' checkbox unchecked. 

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

| Required fields \(you can't update\) | Fields you can update | Fields that won't update and aren't required |
| :--- | :--- | :--- |
| \*producer | sku | ^variant\_unit\_name |
| \*name | price | ^tax\_category |
| ^category | in\_stock | ^shipping\_category |
| \*units | unlimited | ^description |
| ^unit\_type \(if applicable\) |  |  |
| ^variant\_unit\_name \(if applicable\) |  |  |
| \*display\_name |  |  |

_^ if you try to update these fields you'll see an error message_

_\*If you try to update these fields you'll actually create new products or variants, rather than update an existing product._

Once complete, the .csv can be [imported](product-and-inventory-import.md#import-the-csv) in the same manner as for new products. 

{% hint style="info" %}
**Set stock to zero for all exiting products not present in the file:**   
If you select this tickbox the system will set the 'In Stock' value to zero for _all products already your product list_.   
If a product was 'Unlimited' it will remain 'Unlimited'.   
The Products in this import will retain the stock level set in the .csv
{% endhint %}

## Import New Inventory or update your inventory

Use these instructions if you want to add or update new products to your [inventory](inventory-tool.md).

### Prepare the CSV file for import

Firstly, download the **Inventory Template CSV** file from the **Product Import** page.

You'll see that the template gives all the column headings required to successfully import a product. Each row is for a new product or variant. Below is a description of how to fill in each column.

{% hint style="info" %}
Note that all fields are case sensitive. E.g. you must use mL not ml , or Dairy not dairy.
{% endhint %}

| Column Title | Required? | Description | Example |
| :--- | :--- | :--- | :--- |
| producer | Y | This is the name of the producer profile that this inventory item will be assigned to | Four Mile Farm |
| distributor | Y | This is the name of the hub profile the inventory item will be assigned to | Demo Hub |
| name | Y | This is the name of the product | Yoghurt |
| display name | N | This field applies if you are creating variants \(see instructions below\). If you're not creating a variant leave this field blank. | Rasberry Yoghurt |
| variant\_unit\_name | Y | If the product is sold as an item \(e.g loaf, bunch, pumpkin\) write the item type here | Bunch |
| units | Y | The weight, volume or quantity value | 500 |
| unit\_type | Y | What unit is it sold in \(g, kg, T, mL, L\)? If sold as an item \(e.g. bunch\) leave blank | g |
| price | Y | The price of the product. If the item carries tax, this must be the tax inclusive price. | 3.70 |
| On\_Hand  \(in\_stock\) | Y | Please check the rules for unlimited below | leave blank as unlimited is set to 1 |
| On\_demand \(unlimited\) | Y | If blank - Read as "Use producer stock settings", so "in\_stock" should be blank.   If you set it to "1" - Read as unlimited of "Yes", so "in\_stock" should be blank.     If you set it to "0" - Read as unlimited of "No", so "in\_stock" is required. | 1 |
| sku | N | The SKU code for this product | AD001265 |

### Import the CSV <a id="import-the-csv"></a>

Once you have filled out the **Inventory Template CSV** you are ready to upload it into OFN. 

1. Go to **Products** &gt;  **Product Import.**
2. **Select import type:** Select Inventories
3. **Select a spreadsheet to upload**
4. Click **Upload**.

You'll be shown a summary of your upload, including any errors. You'll also be told how many products you are creating and how many you are updating. If you're happy with the upload results, click **save**. 

{% hint style="success" %}
It's good practice to check that the products uploaded/updated as you intended.
{% endhint %}



