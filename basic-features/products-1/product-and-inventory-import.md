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
3. Importar productos a un nuevo [inventario](inventory-tool.md) de tienda / hub(nodo)
4. Actualizar productos en un inventario de tienda / hub(nodo)

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

Utilice estas instrucciones si desea agregar nuevos productos al perfil de un productor.&#x20;

{% hint style="success" %}
Puede cargar nuevos productos y actualizar productos existentes simultáneamente con una sola carga de CSV. Las instrucciones de esta guía están separadas para mayor claridad, pero puede combinar nuevos productos y actualizaciones en la misma hoja de cálculo.
{% endhint %}

### Prepare el archivo CSV para importar

En primer lugar, descargue el archivo CSV **Plantilla de Lista de Productos** de la página de **Importación de Productos** y ábralo con Libre Office (Excel o equivalente).

Verá que la plantilla proporciona todos los encabezados de columna necesarios para importar correctamente un producto. Cada fila es para un nuevo producto o variante. A continuación se muestra una descripción de cómo completar cada columna.

{% hint style="danger" %}
Tenga en cuenta que todos los campos distinguen entre mayúsculas y minúsculas. P.ej. debe usar mL no ml, o Lácteos no lácteos.
{% endhint %}

| Título de la Columna            | ¿Requirido? | Descripción                                                                                                                                                                                            | Ejemplo                                          |
| ------------------------------- | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------ |
| producer                        | Y           | Este es el nombre del perfil de productor al que se asignará este producto                                                                                                                             | Four Mile Farm                                   |
| sku                             | N           | El código SKU de este producto                                                                                                                                                                         | AD001265                                         |
| name                            | Y           | Este es el nombre del producto                                                                                                                                                                         | Yoghurt                                          |
| display name                    | N           | Este campo se aplica si está creando variantes (consulte las instrucciones a continuación). Si no está creando una variante, deje este campo en blanco                                                 | Rasberry Yoghurt                                 |
| category                        | Y           | ¿A qué categoría pertenece este producto? Las categorías disponibles se enumeran en la página de importación de productos                                                                              | Lácteos                                          |
| units                           | Y           | El peso, el volumen o el valor de la cantidad                                                                                                                                                          | 500                                              |
| unit\_type                      | Maybe       | ¿En qué unidad se vende (g, kg, T, mL, L)? Si se vende como un artículo (p. Ej., Manojo) déjelo en blanco                                                                                              | g                                                |
| variant\_unit\_name             | Maybe       | Si el producto se vende como un artículo (por ejemplo, pan, manojo, calabaza) escriba el tipo de artículo aquí                                                                                         | Manojo                                           |
| price                           | Y           | El precio del producto. Si el artículo tiene impuestos, este debe ser el precio con impuestos incluidos                                                                                                | 3.70                                             |
| <p>On_Hand</p><p>(in_stock)</p> | Maybe       | Si tiene inventario limitado para el tipo de producto, indique el nivel de inventario aquí. Si tiene existencias infinitas disponibles (siempre puede obtenerlas) ingrese 0 y use la columna ilimitada | 40                                               |
| available\_on                   | N           | Dejar en blanco                                                                                                                                                                                        |                                                  |
| On\_demand (unlimited)          | Y           | Si tiene existencias infinitas disponibles para este producto, escriba 1, si está usando on\_hand déjelo en blanco. Si ingresa un número en in\_stock _y_ 1 en ilimitado, el producto será ilimitado   | 1                                                |
| shipping\_category              | Y           | ¿En qué categoría de envío se incluye este producto? Las categorías de envío disponibles se enumeran en la página Importación de productos                                                             |                                                  |
| tax\_category                   | N           | Si el precio de su producto incluye el tipo de impuesto IVA, si no, déjelo en blanco                                                                                                                   | IVA                                              |
| description                     | N           | Puede crear una descripción, pero no puede actualizarla. Asegúrese de que el texto que escribió coincida con la descripción actual en caso de una actualización                                        | Este yogur está elaborado con frambuesas locales |

#### Importar Variantes de Producto

En el proceso de importación, las variantes se distinguen por las unidades (como la ensalada que se vende en bolsas de 500 gy 750 g) o los campos display\_name (como un yogur que se vende en varios sabores). Siempre que el nombre del producto sea el mismo, las filas se importarán como variantes. El siguiente ejemplo muestra una ensalada que viene en variantes de 500 g y 750 g, y un yogur que viene en varios sabores.

| name              | display\_name | price | units | unit\_type |
| ----------------- | ------------- | ----- | ----- | ---------- |
| Bolsa de Ensalada |               | 3.50  | 500   | g          |
| Bolsa de Ensalada |               | 5.50  | 750   | g          |
| Yoghurt           | Banano        | 4     | 500   | g          |
| Yoghurt           | Fresa         | 4     | 500   | g          |

La siguiente imagen muestra cómo se mostrarán estos productos en la tienda. Tenga en cuenta que el campo 'nombre' se convierte en el encabezado principal y el campo 'display\_name' se convierte en el encabezado secundario. En el caso de la Bolsa de Ensalada, el campo 'display\_name' está en blanco, por lo que el 'nombre' se usa por defecto.

![](<../../.gitbook/assets/image (1).png>)

#### Ejemplos de tipos de unidades

A continuación se muestran algunos ejemplos para mostrar cómo se deben cargar productos con diferentes unidades (g, ml, kg y artículos).

| producer         | **name**        | **category** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| ---------------- | --------------- | ------------ | --------- | --------- | :------------: | :---------------------: |
| Sue's Salads     | Salad Bag       | Vegetables   | 3.50      | 500       |        g       |       <p><br></p>       |
| Henry Orchards   | Fruit Juice     | Drinks       | 3.50      | 300       |       ml       |       <p><br></p>       |
| Fernwell Produce | Potatoes        | Vegetables   | 9.50      | 5         |       kg       |       <p><br></p>       |
| Tom's Bakery     | Wholemeal Bread | Baked goods  | 3.00      | 1         |   <p><br></p>  |           loaf          |

### Importar el CSV

Una vez que haya completado la **Plantilla CSV de la Lista de Productos**, estará listo para cargarlo en OFN.

1. Vaya a **Productos** >  **Importación.**
2. **Seleccione tipo de importación:** Seleccione Lista de  Productos
3.  **Seleccione la hoja de cálculo para cargar:** Encuentre el archivo csv que desea cargar.

    Debido a que está cargando nuevos productos, puede dejar sin marcar la casilla de verificación "_Establecer stock en cero para todos los productos existentes que no están presentes en el archivo"_.&#x20;
4. Haga click en  **Subir**.

Se le mostrará un resumen de su carga, incluidos los errores. También se le dirá cuántos productos está creando y cuántos está actualizando. Si está satisfecho con los resultados de la carga, haga clic en **guardar**.

{% hint style="success" %}
Es una buena práctica comprobar que los productos se hayan subido o actualizado según lo previsto.
{% endhint %}

Luego puede cargar otra hoja de cálculo o ir a la página de productos para ver sus nuevos productos.

## Actualizar los Detalles de Producto Existente

Las instrucciones a continuación se relacionan con la actualización de los detalles de un producto existente. Esta herramienta está pensada como una forma rápida de actualizar los precios de los productos y los niveles de existencias.

{% hint style="info" %}
Puede cargar nuevos productos y actualizar productos existentes simultáneamente con una sola carga de CSV. Las instrucciones de esta guía están separadas para mayor claridad, pero puede combinar nuevos productos y actualizaciones en la misma hoja de cálculo.
{% endhint %}

### Prepare el archivo CSV para importar

El proceso para actualizar los detalles del producto es similar a [cargar nuevos productos](product-and-inventory-import.md#importar-nuevos-productos). El primer paso es descargar la **Plantilla de Lista de Productos** y completar los nombres de los productos y los nombres de los proveedores. Si tiene esta hoja de cálculo a mano de una carga anterior, aún mejor.&#x20;

El sistema requiere siete campos para identificar correctamente el producto que desea actualizar. Hay cuatro campos que pueden actualizarse y cuatro campos que no pueden usar esta herramienta.

| Required fields (you can't update)   | Fields you can update | Fields that won't update and aren't required |
| ------------------------------------ | --------------------- | -------------------------------------------- |
| \*producer                           | sku                   | ^variant\_unit\_name                         |
| \*name                               | price                 | ^tax\_category                               |
| ^category                            | in\_stock             | ^shipping\_category                          |
| \*units                              | unlimited             | ^description                                 |
| ^unit\_type (if applicable)          |                       |                                              |
| ^variant\_unit\_name (if applicable) |                       |                                              |
| \*display\_name                      |                       |                                              |

_^ si intenta actualizar estos campos, verá un mensaje de error._

_\* Si intenta actualizar estos campos, creará nuevos productos o variantes, en lugar de actualizar un producto existente._

Una vez completado, el .csv se puede  [importar](product-and-inventory-import.md#import-the-csv) de la misma manera que para los productos nuevos.&#x20;

{% hint style="info" %}
**Establezca el inventario en cero para todos los productos existentes que no estén presentes en el archivo:** \
****Si selecciona esta casilla de verificación, el sistema establecerá el valor 'En stock' en cero para _todos los productos que ya están en su lista de productos_.

Si un producto era 'Ilimitado', seguirá siendo 'Ilimitado'.

Los productos de esta importación conservarán el nivel de stock establecido en el archivo csv
{% endhint %}

## Importar nuevo Inventario o actualizar su inventario

Utilice estas instrucciones si desea agregar o actualizar nuevos productos a su [inventario](inventory-tool.md).

### Prepare el archivo CSV para importar

En primer lugar, descargue el archivo **CSV de Plantilla de Inventario** de la página de **Importación de Productos**.&#x20;

Verá que la plantilla proporciona todos los encabezados de columna necesarios para importar correctamente un producto. Cada fila es para un nuevo producto o variante. A continuación se muestra una descripción de cómo completar cada columna.

{% hint style="info" %}
Tenga en cuenta que todos los campos distinguen entre mayúsculas y minúsculas. P.ej. debe usar mL no ml, o Lácteos no lácteos.
{% endhint %}

| Column Title                  | Required? | Description                                                                                                                                                                                                                                                                                                       | Example                                            |
| ----------------------------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| producer                      | Y         | Este es el nombre del perfil de productor al que se asignará este producto                                                                                                                                                                                                                                        | Four Mile Farm                                     |
| distributor                   | Y         | Este es el nombre del perfil del hub/nodo al que se asignará el artículo de inventario                                                                                                                                                                                                                            | Demo Hub                                           |
| name                          | Y         | Este es el nombre del producto                                                                                                                                                                                                                                                                                    | Yoghurt                                            |
| display name                  | N         | Este campo se aplica si está creando variantes (consulte las instrucciones a continuación). Si no está creando una variante, deje este campo en blanco                                                                                                                                                            | Rasberry Yoghurt                                   |
| variant\_unit\_name           | Y         | Si el producto se vende como un artículo (por ejemplo, pan, manojo, calabaza) escriba el tipo de artículo aquí                                                                                                                                                                                                    | Bunch                                              |
| units                         | Y         | El peso, el volumen o el valor de la cantidad                                                                                                                                                                                                                                                                     | 500                                                |
| unit\_type                    | Y         | ¿En qué unidad se vende (g, kg, T, mL, L)? Si se vende como un artículo (p. Ej., Manojo) déjelo en blanco                                                                                                                                                                                                         | g                                                  |
| price                         | Y         | El precio del producto. Si el artículo tiene impuestos, este debe ser el precio con impuestos incluidos                                                                                                                                                                                                           | 3.70                                               |
| <p>On_Hand <br>(in_stock)</p> | Y         | Consulte las reglas para ilimitado a continuación                                                                                                                                                                                                                                                                 | dejar en blanco ya que ilimitado se establece en 1 |
| On\_demand (unlimited)        | Y         | Si está en blanco: lea como "Usar configuración de stock del productor", por lo que "in\_stock" debe estar en blanco. Si lo establece en "1" - Leer como ilimitado de "Sí", por lo que "in\_stock" debe estar en blanco. Si lo establece en "0" - Leer como ilimitado de "No", por lo que se requiere "in\_stock" | 1                                                  |
| sku                           | N         | El código SKU de este producto                                                                                                                                                                                                                                                                                    | AD001265                                           |

### Importe el archivo CSV <a href="#import-the-csv" id="import-the-csv"></a>

Una vez que haya completado el **CSV de la Plantilla de Inventario**, estará listo para cargarlo en OFN. &#x20;

1. Vaya a **Productos**> **Importación de Productos**.
2. **Seleccione el tipo de importación**: Seleccione Inventarios
3. **Seleccione una hoja de cálculo para cargar**
4. Haga click en **Subir**.

Se le mostrará un resumen de su carga, incluidos los errores. También se le dirá cuántos productos está creando y cuántos está actualizando. Si está satisfecho con los resultados de la carga, haga clic en **guardar**.&#x20;

{% hint style="success" %}
Es una buena práctica comprobar que los productos se hayan subido o actualizado según lo previsto.
{% endhint %}

