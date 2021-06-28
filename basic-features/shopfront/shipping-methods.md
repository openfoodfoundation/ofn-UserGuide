# Métodos de Envío

{% hint style="warning" %}
 **Debe** crear por lo menos un método de envío antes de poder abrir su tienda.
{% endhint %}

Antes de seguir leyendo, es posible que desee ver una demostración rápida de cómo configurar su primer método de envío:

![](../../.gitbook/assets/shippingmethod.gif)

## Configurar un método de envío

* Vaya a la página Métodos de envío haciendo clic en **Organizaciones** en el menú horizontal azul y luego haga clic en **Configuración** junto a su organización. La página de **Métodos de Envío** se encuentra en el menú del lado izquierdo.
* Haga clic en **Crear nuevo método de envío +**. Será dirigido a una página como esta: 

![](../../.gitbook/assets/newshipping.jpg)

* Marque la casilla junto a su organización en el lado derecho de la página debajo de 'Hubs/Nodos'. Esto indica que el método de envío que está a punto de crear se aplicará a esa organización. Puede seleccionar varias empresas, si lo desea. 
* **Nombre**: Elija un nombre para el método. Este nombre se mostrará al cliente durante su proceso de compra y en los correos de confirmación de pedido. Ejemplo: 

![](../../.gitbook/assets/shippinginfo.jpg)

* **Descripción:** Agregue detalles adicionales, como la dirección precisa del punto de recolección. Estos detalles serán visibles para los clientes en gris junto al nombre \(vea la captura de pantalla anterior\).
* **Categoría:** ¿Este método es una entrega o una recogida? 
* **Etiquetas:** ingrese etiquetas aquí si desea diferenciar entre clientes. Las etiquetas pueden ser útiles si desea ofrecer envío gratuito a un subconjunto de clientes o solo ofrecer entrega a aquellos que tienen una dirección registrada cercana. Lee mas [aquí](customer-management-and-conditional-displays-prices/).
* **Calculadora:** Seleccione la forma en que se agregarán las tarifas de envío a este método de envío. Tenga en cuenta que la tarifa de envío puede ser cero. Consulte a continuación para obtener más detalles.
* **Categorías:** Condiciones de transporte \(refrigeración, congelado, por defecto\) asociadas con este método de envío. 
* **Zonas:** Seleccione la zona apropiada \(esto es para habilitar la calculadora de impuestos correcta\).

Al hacer clic en **Crear**, se creará el método de envío y, a continuación, se le proporcionarán nuevos campos para agregar detalles de los cargos del método de envío. Los campos presentados dependerán de la calculadora de tarifas de envío que haya seleccionado.

{% hint style="info" %}
Si cambia el tipo de calculadora para un método de envío, **primero debe guardar** antes de poder editar la configuración de la calculadora.
{% endhint %}

## Calculadora de Comisiones

![](../../.gitbook/assets/shippingcalc.jpg)

**Peso \(por kg\)** – Esta tasa se aplica a los productos por kg. La tarifa _solo se aplicará a los productos cuyo precio sea por kg_, no a los productos enumerados como artículos \(por ejemplo, un producto enumerado como "1 manojo de perejil" no contribuirá a la tarifa general que se le cobra al cliente por el envío\)

**Porcentaje Fijo** – Esta tarifa se cobra como un porcentaje del monto total gastado en el pedido.

**Tasa Fija \(por pedido\)** – Esta tarifa se aplica como tarifa estándar a todos los pedidos, independientemente del tamaño del pedido.

**Tasa Flexible** – Esta calculadora de tarifas es especialmente útil si desea alentar a los clientes a realizar pedidos grandes: el costo de envío puede reducirse o reducirse a cero cuando se alcanza un número mínimo de artículos. 

* "Costo del Primer Artículo": la tarifa que se cobra por el primer artículo del pedido.
* "Costo de Artículo Adicional": la tarifa que se cobra por artículos más allá del primer artículo.
* "Máximo de Artículos": el número máximo de artículos a los que se aplicará la tarifa. A los artículos comprados que superen esta cantidad no se les cobrará la tarifa. 

![](../../.gitbook/assets/shippingfeeflex.jpg)

> Por ejemplo: si la tarifa de envío para el 'Costo del primer artículo' es $2000, 'Costo adicional del artículo' = $1000 y 'Max artículos' = 3. A un cliente que compre 5 artículos se le cobrarán $ 4000 de envío \($2000 por el primer artículo, $1000 por los artículos dos y tres y $0  por los artículos cuatro y cinco\).

**Tarifa Fija \(por ítem\)** – Esta tarifa es una tarifa constante que se aplica a los productos enumerados como "artículos". \(No se aplica a los productos vendidos por peso o volumen. Por lo tanto, no se cobrará ningún costo de envío asociado a un cliente que, por ejemplo, compra arroz por kg\).

**Precio Saco** – Este es un método flexible tarifa de envío cobrado por la _venta total en pesos_, en lugar de número de artículos comprados \(Tarifa Flexible arriba\).

* "Cantidad Mínima": valor Monetario del umbral entre la tarifa de envío normal y la tarifa de envío con Descuento.
* 'Importe Normal': tarifa de envío aplicada a las ventas por debajo del umbral indicado en 'Importe Mínimo'. 
* "Importe de Descuento": tarifa de envío que se aplica a las ventas por encima del umbral indicado en "Importe Mínimo".

![](../../.gitbook/assets/shippingfeepc.jpg)

