# Permisos de la Organización

## Permisos de la Organización

Dentro de los Permisos de la Organización hay reglas que rigen las relaciones comerciales entre organizaciones: proveedores y distribuidores. Estas reglas deben establecerse antes de que una organización \(Perfil de productor o Tienda de productor\) pueda convertirse en proveedor de otra \(Hub/Nodo\), o viceversa. Una empresa concede un permiso \(o 'derecho'\) a otra con respecto al acceso / modificación de productos y perfil. Esta página detalla los diferentes permisos y cómo asignarlos.

Para acceder a los permisos de su organización:

![](../../.gitbook/assets/permissions.gif)

Por último, exploramos este tema desde el punto de vista de:

* [un Hub/Nodo](enterprise-to-enterprise-permissions-e2es.md#hub-perspective) \(el distribuidor\)
* [un perfil de productor o tienda](enterprise-to-enterprise-permissions-e2es.md#producers-perspective) \(el proveedor\)

## Los Cuatro Permisos

Hay 4 tipos diferentes de permisos de Organización. Se pueden combinar en distintas formas para dar a las organizaciones más o menos permisos de acuerdo a sus perfiles. 

![](../../.gitbook/assets/e2emenu2.jpg)

**Permiso para agregar al ciclo de pedidos**: el proveedor \(productor\) permite al distribuidor \(un Hub/Nodo OFN\) agregar productos a los ciclos de pedidos de este último. Por lo tanto, los productos del proveedor pueden aparecer en la tienda del hub/nodo.

**Permiso para administrar productos**: el proveedor autoriza a otra organización registrada en OFN \(generalmente un hub/nodo\) para crear, eliminar y modificar productos directamente en su catálogo de proveedores.

{% hint style="danger" %}
Esto puede afectar potencialmente a todos los hubs/nodos a los que el productor suministra bienes a través de OFN.
{% endhint %}

> _Por ejemplo, si la Finca La María suministra papas a los Hubs/Nodos A y B pero le otorga al Hub/Nodo A permiso para administrar sus productos, entonces si el Hub/Nodo A cambia el precio de las papas, este cambio de precio \(en la configuración estándar\) se reflejará en las fachadas de las tiendas de ambos. hubs/nodos A y B._

**Permiso para editar perfil**: una organización permite a otra modificar detalles en su [Perfil Organizacional](./) \(datos de contacto, dirección, descripción, ...\).

**Permiso para agregar productos al inventario**: el proveedor \(productor\) autoriza al distribuidor \(hub/nodo\) a agregar sus productos al catálogo de la tienda \(o '[Inventario](../products-1/inventory-tool.md)'\) del hub/nodo.

Si un productor suministra bienes a más de un hub/nodo, entonces para permitir que cada uno de estos hubs/nodos administre los precios y los niveles de existencias de sus productos de forma independiente, recomendamos agregar este permiso entre las dos organizaciones y que los hubs/nodos cambien su [configuración de inventario](../products-1/inventory-tool.md#modify-sku-prices-and-stock-levels-for-products-in-your-shopfront).

## Concesión y Administración de Permisos

Para modificar, agregar o eliminar permisos, vaya al panel de administración y luego a 'Organizaciones' en el menú azul y 'Permisos' en el submenú verde. 

![](../../.gitbook/assets/e2emenu.jpg)

Dar permiso:

* Seleccione su organización en el menú desplegable de la primera columna \(es un productor que suministra a otros\)
* Seleccione el nombre de la organización \(hub/nodo\) que desea suministrar en la segunda columna.
* Marque los permisos que desea otorgar al distribuidor de sus productos \(hub/nodo\) o para otorgar múltiples permisos, seleccione 'todo'.
* Haga clic en 'Crear'.

Tenga en cuenta que puede eliminar o cambiar estos permisos en cualquier momento.

{% hint style="warning" %}
Solo los usuarios que figuran como [Administradores](transfer-ownership.md) de una organización pueden cambiar sus permisos. 
{% endhint %}

Si necesita que otra organización le otorgue permisos, debe comunicarse con ellos por correo electrónico o por teléfono. No hay una función en línea para hacer esto. 

## Permisos Generados Automáticamente

Cuando un usuario es el administrador principal de varias organizaciones en la plataforma, [los cuatro permisos](enterprise-to-enterprise-permissions-e2es.md#los-cuatro-permisos) se crean automáticamente entre cada organización. Este no es el caso cuando las organizaciones son administradas por diferentes usuarios.

## Perspectiva del Hub/Nodo

Los siguientes escenarios comunes demuestran los permisos de organización a organización que puede necesitar configurar para su hub/nodo.

> **He creado** [**Perfiles de Productor para cada uno de mis Proveedores**](./)**. ¿Qué permisos necesito configurar antes de poder almacenar sus productos en mi tienda Hub/Nodo?**

El sistema está configurado para que los hubs/nodos que crean perfiles de productor tengan los _permisos correctos instalados de forma predeterminada_, para que puedan comenzar a agregar productos y comerciar con estos perfiles de productor de inmediato.

> **Mi** [**proveedor ya tiene una organización registrada en OFN**](create-or-connect-with-your-supplying-producers.md#supplyingproducer)**. Me gustaría agregar sus productos a la tienda de mi hub/nodo.**

Debe comunicarse con su proveedor en persona. Sus datos de contacto \(número de teléfono, dirección y dirección de correo electrónico\) se ubicarán en su perfil OFN.

Si solo tiene la intención de **almacenar sus productos** y no desea ayudarlos a administrar el resto de su perfil OFN, solicite al productor que otorgue permiso **para agregar al ciclo de pedidos** y permiso **para agregar al inventario**.

Si el proveedor desea que usted, como administrador de Hub/Nodo, lo ayude a organizar su organización OFN, entonces puede otorgarle los cuatro permisos. Si esto ocurre, podrá editar su perfil y administrar sus productos.

> **My Hub/Nodo distribuye a través de grupos de compra. ¿Qué permisos necesitará el grupo comprador con mi hub/nodo y mis productores?**

{% hint style="warning" %}
Este es un ejemplo de dónde el hub/nodo que gestiona \(coordina\) un ciclo de pedidos difiere de la organización de la que los clientes recogen sus compras.

_Si el Hub/Nodo A gestiona \(coordina\) un ciclo de pedido para un grupo de compras \(Hub/Nodo B\), el ciclo de pedido se mostrará en la tienda OFN del Hub/Nodo B._ 
{% endhint %}

\_\_

El grupo de compras \(Hub/Nodo B arriba\) deberá otorgarle al coordinador del ciclo de pedidos \(Hub/Nodo A arriba\) permiso para agregar al ciclo de pedidos \(e idealmente permiso para agregar al inventario\).

Los productores que suministran al Hub/Nodo A productos que también serán vendidos por el grupo de compra \(Hub/Nodo B\) deben otorgar a los Hub/Nodo A y B permiso para agregar al ciclo de pedidos \(e idealmente permiso para agregar al inventario\).

## Perspectiva del Productor

Cuando un productor desea comenzar a vender sus productos a través de otras organizaciones \(hubs/nodos o grupos de compra\), debe establecer los permisos adecuados de organización a organización. Hay diferentes niveles de permiso que un productor puede otorgar, dependiendo de la cantidad de poder que quiera otorgar al hub/nodo para administrar sus productos y su perfil \([ver la parte superior de la página](enterprise-to-enterprise-permissions-e2es.md)\).

Estos ejemplos exploran algunos escenarios comunes.

> **Soy productor y me gustaría tener un hub/nodo OFN local para almacenar y vender mis productos.**

**Esencial**: Para que el hub/nodo agregue sus productos a su tienda, deberá otorgarles "_permiso para agregar al ciclo de pedidos_".

**Opcional**: Es posible que también desee otorgar permiso al hub/nodo para administrar sus productos, editar su perfil o agregar al Inventario.

> **Un hub/nodo que yo suministro distribuye a través de grupos de compra.**

Para que sus productos sean distribuidos por los grupos de compra, tendrá que agregar un permiso mínimo 'para agregar al ciclo de pedido' para la organización del grupo de compras, _así como_ para el hub/nodo que suministra directamente.

> **Soy un Tienda de Productor que suministra un Hub/Nodo local además de dirigir mi propia tienda. Al Hub/Nodo le gustaría gestionar los niveles de inventario y los precios de mis productos.** _**También**_ **me gustaría gestionar los niveles de inventario y los precios de mis productos.**

Este escenario se puede resolver otorgando al hub/nodo permiso para agregar al Inventario, así como permiso para agregar al ciclo de pedidos.

Esto permite que el hub/nodo almacene sus productos en su tienda, pero establezca sus propios precios y niveles de inventario. Cuando abastezca su propia tienda con sus productos, estos seguirán reflejando los precios y los niveles de inventario que ha establecido.

