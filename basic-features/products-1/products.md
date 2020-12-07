# Agregar productos

Puede agregar productos a su catálogo uno por uno \(detallado a continuación\) o por [importación masiva](product-and-inventory-import.md), si tiene todos los detalles relevantes en un archivo .csv.

## Agregando productos

Una vez que haya iniciado sesión en el Panel de Administración, seleccione **Productos** en el menú azul horizontal y luego haga clic en **+Nuevo producto**.

![](../../.gitbook/assets/add-new-product.png)

Esto lo llevará a la página de Nuevo Producto.

![](../../.gitbook/assets/new-product2.png)

**Proveedor** 

Seleccione la organización que produce y suministra el producto.

Si es un productor, este será ud. Si es un hub/nodo, recuerde que solo podrá agregar productos a los perfiles de productor que haya creado, o si se le ha otorgado permiso para administrar los productos de un perfil de productor. Vea [aquí](../enterprise-profile/create-or-connect-with-your-supplying-producers.md) más información.

**Nombre del producto**: este es el título del producto cuando se muestra en la tienda.

**Unidades**: Elija la unidad en la que se vende el producto? \(g, kg, L ... o artículo \(manojo, bolsa, paquete\)\)

Si elige g luego ingresa 1000, el producto se mostrará como 1 kg para el comprador. Tenga en cuenta que algunas unidades de medida afectarán el funcionamiento de determinadas [comisiones de la organización](../shopfront/enterprise-fees.md).

Por ejemplo, una[ comisión fija](../shopfront/enterprise-fees.md) por peso solo se puede aplicar a productos con unidades de kg. En este caso, puede ingresar números de unidades no enteros, como 0.2 kg, y el producto se mostrará como 200 g, pero se registrará en kg en los informes y cuando se calculen los precios.

**Valor**: Ingrese el valor de las unidades en las que se vende este producto \(por ejemplo, si se vende como 100 g, ingrese '100' aquí y elija 'g' para 'unidades'; o si se vende como racimos de flores, ingrese '1' aquí y 'unidades = artículos'.

**Mostrar como**: este campo muestra automáticamente cómo se mostrarán los campos de unidades y valores, una vez que haya completado los campos de unidades y valores. \(es decir, unidades = kg, valor = 2, mostrar como = 2 kg\)

{% hint style="info" %}
Nota: Si ha seleccionado "**artículos**" como su unidad, el campo **mostrar como** cambiará a "**nombre del artículo**". Complete esto con el tipo de artículo que es. \(es decir, frasco, botella o manojo\)
{% endhint %}

**Categoría de producto**: seleccione la categoría más adecuada para este producto. La asignación de una categoría de producto facilita a los clientes la localización de los artículos que desean comprar; Los compradores pueden filtrar su lista de productos por categoría en su tienda. 

**Precio**: Ingrese el precio por el valor indicado arriba. Tenga en cuenta que este es el precio base que cobra el productor y la cantidad que recibirá por cada compra. Los márgenes y las comisiones \(para administración de distribución, etc.\) se agregan en [Comisiones de la Organización](../shopfront/enterprise-fees.md), [Comisiones de Envío](../shopfront/shipping-methods.md) y [Métodos de Pago](../shopfront/payment-methods.md).

{% hint style="info" %}
Si su organización está registrada para impuestos o si selecciona que este producto tenga impuestos, el precio que ponga aquí **incluye los impuestos**. Si selecciona que este producto está libre de impuestos, el precio que ingrese será el precio libre de impuestos.
{% endhint %}

**En Inventario**: indique la cantidad o cantidad de este producto que tiene disponible y listo para la venta.

Utilice este campo si desea realizar un seguimiento de sus niveles de existencias. A medida que los clientes realicen pedidos, el nivel de existencias se reducirá y, cuando la cantidad en existencia llegue a cero, el producto ya no estará visible en su tienda. Si no desea realizar un seguimiento del inventario de esta manera, haga clic en "a pedido".

**Ilimitado**: Si selecciona esta casilla, indicará que este producto siempre está disponible. Esto evita que el software rastree los niveles de inventario de los productos y, en su lugar, siempre mostrará que el producto está en inventario.

**Imagen**: Suba una foto de este producto.

{% hint style="success" %}
Recomendamos utilizar fotos de buena calidad, en formato cuadrado \(1: 1\), y preferiblemente una foto real de sus productos en lugar de la imagen estándar de la web. Esto hace que el producto sea más atractivo para el consumidor. Siempre tome sus fotografías con buena luz.

Si utiliza una imagen de la web, compruebe que está libre de derechos. 
{% endhint %}

**Categoría de impuestos**: seleccione la categoría de impuestos correspondiente de la lista desplegable. El impuesto \(IVA en Colombia\) depende de la naturaleza del producto y del país en el que lo vende.

{% hint style="danger" %}
Los impuestos solo se cobrarán cuando las empresas hayan seleccionado 'cargos IVA = sí' en su configuración organizacional -&gt; Detalles de la Organización.
{% endhint %}

**Descripción del producto**: Cuéntele a sus clientes un poco sobre este producto. Es posible que desee incluir una historia sobre la variedad de tomate específica, incluir hipervínculos a cualquier certificación que pueda tener, etc.

{% hint style="info" %}
No olvide hacer clic en el botón "crear" o "crear y agregar nuevo" en la parte inferior de la página una vez que se hayan ingresado todos los campos obligatorios \(los indicados con un asterisco rojo\). 
{% endhint %}

Una breve demostración de los pasos descritos anteriormente:

![](../../.gitbook/assets/productsadd.gif)

Cuando haya terminado de crear un producto, se le redirigirá a la página "productos" donde encontrará todos sus productos:

![](../../.gitbook/assets/productspage.jpg)

## Listado Similar / variaciones de un producto 

Si está enumerando un producto que viene en varias opciones diferentes \(por ejemplo, diferentes tamaños o sabores, cada uno de los cuales puede tener o no un precio diferente\), es mejor crear una 'variante' para ese producto, en lugar de crear múltiples productos separados. La creación de variantes de productos se analiza en detalle en la [página siguiente](product-variants.md).

{% hint style="success" %}
Las variantes son útiles si, por ejemplo, vende limones individualmente, así como en 'paquetes' de 5. En lugar de tener dos listados de productos, las dos opciones pueden estar disponibles para el mismo producto.
{% endhint %}

Si desea crear un producto SIMILAR, puede duplicar productos seleccionando el icono de doble página a la derecha de un artículo \(cuadro rojo\). Al seleccionar posteriormente el icono de lápiz y papel \(cuadro verde\), se puede editar el producto copiado y modificar los detalles del segundo elemento.

![](../../.gitbook/assets/productspagecopy.jpg)

## Refine los atributos del producto

Con OFN puede agregar **propiedades o etiquetas** a sus productos. Esto permite a los clientes encontrar sus artículos cuando buscan criterios específicos \(por ejemplo, orgánicos certificados\) y destaca las cualidades específicas que pueden tener sus productos. Descubra más [aquí](product-properties.md).

Para obtener sugerencias sobre cómo administrar las ventas de **productos "irregulares"**, como carne o verduras grandes, que se venden en unidades pero cuyo precio se calcula por peso, lea [aquí](pricing-irregular-items-kg.md).

Nuestra herramienta Grupo de Compras le permite gestionar y organizar las ventas de productos en lotes. Descubra más [aquí](group-buy-for-bulk-ordering.md).

