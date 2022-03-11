# Compra Grupal: para pedidos al por mayor

La función **Compra Grupal** está diseñada para empresas que compran algunas de sus existencias entrantes en cantidades a granel y las revenden en unidades más pequeñas (por ejemplo, compran una bolsa de arroz de 25 kg y venden al por menor a los clientes por kg).

La compra al por mayor es una práctica común para los **grupos de compra**, quienes, al comprar grandes volúmenes, pueden beneficiarse de los precios al por mayor de la misma manera que los distribuidores convencionales. Al hacerlo, los miembros acceden a alimentos mucho más baratos de lo que podrían obtener de los minoristas de la calle.

Para tales empresas, la decisión de pedir un determinado producto depende de si los clientes han pedido colectivamente lo suficiente para justificar una compra al por mayor. Esto puede deberse a descuentos por volumen o tarifas de envío. La función de compra grupal hace que sea más fácil para el hub/nodo lograr eficiencias de compra masiva.

Cuando un producto se asigna a la compra grupal, se mostrará de manera diferente en la tienda (ver más abajo), con una doble columna de cantidad mínima / máxima visible:

![](<../../.gitbook/assets/group-buy (1).png>)

Se solicita al cliente que indique:

* Su cantidad **mínima**: esta es la cantidad del producto que idealmente desean.
* Su cantidad **máxima**: esta es la cantidad máxima que estarían dispuestos a comprar.Customer are asked to indicate:

{% hint style="info" %}
Básicamente, esta es una forma de que el cliente diga _"tiene mi permiso para aumentar mi pedido hasta este punto, si eso significa que, como grupo, podemos lograr la cantidad de pedido al por mayor"_.
{% endhint %}

En [Gestión de Pedidos al Por Mayor](../orders/view-orders.md#bulk-order-management), puede ver las cantidades totales mínimas y máximas de pedido del producto de todos sus clientes. Luego, puede aumentar los pedidos de los clientes, dentro de su rango aceptable, para lograr la cantidad a al por mayor, o si la cantidad máxima de pedido es insuficiente, puede eliminar todos los pedidos de este producto.

## Habilitando la Compra Grupal para un producto&#x20;

En el panel de administración, vaya a '**Productos**' en el menú horizontal azul. Seleccione **Editar** un producto haciendo clic en el icono de lápiz y papel a la derecha del producto en cuestión:

![](../../.gitbook/assets/productedit.jpg)

Luego, seleccione **Opciones de Compra Grupal** en el menú de la derecha.

![](../../.gitbook/assets/groupbuy.jpg)

Seleccione **Sí** en ¿**Compra Grupal**? **para activar esta función para el producto**.

El **Tamaño de la Unidad al Por Mayor** es la cantidad que debe alcanzar la orden colectiva del grupo.

{% hint style="warning" %}
Las **unidades** para la cantidad de Tamaño de Unidad al POr Mayor dependen de las unidades seleccionadas para vender el producto a los clientes.

Si el producto es vendido por:

* **Peso**: las unidades están en g (por lo tanto, si el total colectivo debe ser igual a 5 kg, ingrese '5000' en este campo)
* **Volumen**: las unidades están en litros (por lo tanto, si el total colectivo debe ser 10 l, ingrese '10' en este campo)
* **Artículos**: ej. vende ramos de flores pero debe comprar 100 ramos en total entonces ingrese '100' en este campo.
{% endhint %}

## Ajustando Pedidos para hacer Lotes completos

En Pedidos-> [gestión de pedidos al por mayor](../orders/view-orders.md#bulk-order-management), puede ver y editar los pedidos de los clientes de productos de Compra al Por Mayor para que el pedido combinado de todos los clientes alcance el umbral requerido.

1. Seleccione el ciclo de pedido o el rango de fechas que le interese.
2. Busque el producto (pescado en el ejemplo siguiente).
3. Asegúrese de que se muestre la columna "Máx" para que pueda ver el límite superior que cada cliente está preparado para comprar.
4. A continuación, haga clic en el valor ('pez de prueba: pez uno' en el ejemplo siguiente) en la columna **Producto: Unidad**, para mostrar el cuadro total de pedidos (en azul) para el producto en cuestión.
5. Con la información de la columna **Máx**., Puede aumentar las cantidades pedidas para alcanzar el umbral de un lote completo.
6. Haga clic en actualizar para guardar los cambios en los pedidos de los clientes.

![](../../.gitbook/assets/bulkorder2.jpg)

**Unidades Realizadas Actuales** divide la cantidad total ordenada por el tamaño de la unidad de compra grupal. Si esta cifra es mayor que 1, le indica que el pedido de cliente existente satisface o excede el tamaño de unidad de compra de grupo requerido. Si esta cifra es menor que 1, los pedidos de clientes existentes no alcanzan ese umbral. A medida que aumenta la cantidad de pedidos de clientes, esta cifra aumentará.

**Las Unidades Máximas Cumplidas** toma la suma o la totalidad de las cantidades MÁXIMAS de pedido del cliente y lo divide por el tamaño de la unidad de compra del grupo. Si el número es superior a 1, entonces sabrá que el total de sus pedidos MAX excede la cantidad de compra grupal requerida. Si está por debajo de 1, significa que incluso las cantidades MÁXIMAS de pedidos no alcanzarán el umbral.
