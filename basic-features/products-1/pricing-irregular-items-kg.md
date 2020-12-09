# Precios de la Carne y otros productos 'completos' de peso desconocido

Aquí nos referimos a los productos como "**irregulares**" si se venden de acuerdo con su peso / volumen pero la cantidad exacta no se conoce hasta el momento de la cosecha / distribución.

Por ejemplo, porciones de carne, lonchas de queso, verduras grandes.

Hay varias herramientas diferentes disponibles en la plataforma OFN para ayudar a administrar y organizar estas ventas. 

## Opción uno: establecer un peso / precio promedio y reembolsar

Puede cobrar el precio promedio del producto y luego reembolsar o cobrar al cliente un extra, si el peso real se desvía de la media.

Cuando sepa el peso real de los productos \(es decir, cuando esté preparando pedidos para que los clientes los recojan\), inicie sesión en "Gestión de pedidos al por mayor" \(Pedidos -&gt; Gestión de pedidos al por mayor\) y agregue la columna Peso / Volumen a la tabla.

![](../../.gitbook/assets/bom1.jpg)

Luego, puede cambiar el peso que se muestra para cada comprador para un pedido determinado y un producto determinado. El precio se volverá a calcular automáticamente según la cantidad ingresada.

{% hint style="info" %}
No olvide volver a enviar un correo electrónico de confirmación del pedido al cliente para notificarle la diferencia de precio y cualquier cantidad que pueda adeudar posteriormente.
{% endhint %}

## Opción Dos: mostrar rangos de precios 

La misma lógica que la Opción Uno, pero simplemente en lugar de mostrar un precio promedio inicialmente, indique un rango de precios. Esta solución tiene la ventaja de indicar claramente al comprador que es probable que se modifique el precio final.

Las [variantes](product-variants.md) también se pueden utilizar para crear diferentes rangos.

> **Ejemplo 1** \(producto único y una variante\):  
> Producto = Pollo \(entre 8 y 12 kg con precio según peso, £ 10 / kg\)
>
> **Ejemplo 2** \(dos variantes para un producto\):  
> Producto = Pollo \(£ 10 / kg\)  
> Variante 1 = Pollo pequeño \(entre 8 y 12 kg, precio según peso real\)  
> Variante 2 = Pollo grande \(entre 13 y 20 kg, precio según peso real\) ...

## Opción Tres: crear variantes con precios fijos 

Una versión un poco más simple de la Opción Dos es crear variantes para sus productos en función de los rangos de peso, pero cobrar un **precio fijo** por todos los artículos que se encuentran dentro del rango.

Por ejemplo, si la calabaza cuesta $ 1000 / kg, entonces podría enumerar las variantes con los siguientes precios fijos:

* Pequeño \(0,7 - 0,9 kg\) $8000
* Mediano \(0,9 - 1,1 kg\) $1000
* Grande \(1,1 - 1,3 kg\) $1200
* Extra grande \(1,3 - 1,5 kg\) $1500

## Opción Cuatro: crear variantes con pesos conocidos

Si conoce el peso de todo su pescado, por ejemplo, de antemano puede utilizar la función de variante para mostrar directamente el precio exacto de cada artículo. Ejemplo:

![](../../.gitbook/assets/bom2.jpg)

## Editar Pedidos 

Puede ser difícil para los productores de carne conocer de antemano la disponibilidad del producto o preparar su empaque en consecuencia. \(Hasta el momento del sacrificio, tal vez se desconozca el peso de un pollo o una pierna de cordero\).

Esto no es un problema ya que los pedidos se pueden modificar \(agregando, modificando o eliminando productos\) si es necesario. Para obtener más información, consulte [Pedidos](../orders/). 

## Reembolsar o cobrar a los clientes la diferencia: ¿Cómo funciona? 

Si un cliente **paga por sus productos en su recogida o entrega**, entonces el administrador del hub/nodo habrá podido modificar el pedido antes del pago de acuerdo con el peso real y los productos realmente entregados. Por lo tanto, en este caso, no será necesario reembolsar o volver a facturar al cliente.

Si un pedido se **paga en línea antes de la entrega**, debe reembolsar o facturar la diferencia entre el dinero ya recibido y el adeuda para que se entreguen los productos precisos. Haga clic [aquí para ver cómo](../orders/refund-payments.md).

{% hint style="danger" %}
Una alternativa es utilizar un sistema de pago online para almacenar temporalmente el importe "pendiente" hasta que el pedido haya sido validado.

_Esta función aún no está implementada en Open Food Network. También estamos trabajando en la implementación automatizada de "créditos" que permiten a un hub/nodo reembolsar en forma de nota de crédito que el cliente podría utilizar como pago parcial de su próximo pedido._ 
{% endhint %}

## Informar al comprador sobre su política de precios

Puede notificar a sus clientes sobre sus políticas de precios para artículos de peso variable \(como carne\) en el [cuadro de mensaje](../enterprise-profile/enterprise-settings.md) que se muestra en la parte superior del frente de su tienda. Esto se encuentra en Configuración empresarial -&gt; Preferencias de la tienda.

También puede ser útil agregar un recordatorio de estas políticas de precios en el cuadro de descripción de [Métodos de Pago](../shopfront/payment-methods.md). Por ejemplo, es posible que desee agregar: "Recuerde que el precio final puede variar en un 10% dependiendo del peso si ha comprado artículos no divisibles como carne o verduras grandes".

