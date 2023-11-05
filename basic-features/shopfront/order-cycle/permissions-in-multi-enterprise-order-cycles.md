# Berechtigungen in unternehmensübergreifenden Auftragszyk

Diese Seite erläutert die unterschiedlichen Rechte, die jedes Unternehmen im Rahmen komplexer, unternehmensübergreifender Auftragszyklen hat. Sei es:

* the producer ([profile](../../../your-quick-start-on-ofn-given-who-you-are.md#profile) or [shop](../../../your-quick-start-on-ofn-given-who-you-are.md#shop)) who supplies the order cycle only,
* a [hub](../../../your-quick-start-on-ofn-given-who-you-are.md#hub) which distributes goods only,
* or a hub which [coordinates](permissions-in-multi-enterprise-order-cycles.md#the-coordinator) the order cycle (and may or may not also supply or distribute goods).

For more details about simple order cycles involving a single producer selling their own stock only ([producer shop](../../../your-quick-start-on-ofn-given-who-you-are.md#shop)), see [here](order-cycles-for-producers.md).

_**The coordinator has the highest degree of control over an order cycle. Other enterprises can view the order cycles they are involved in, but only edit settings which affect them.**_

## Der Koordinator

{% hint style="info" %}
**Full order cycle functionality** can only be obtained if an enterprise is registered as a [Hub](../../../your-quick-start-on-ofn-given-who-you-are.md#hub).  To change your enterprise type see [here](../../enterprise-profile/package-types.md#changing-your-profile-type).
{% endhint %}

{% hint style="warning" %}
Sobald ein Auftragszyklus erstellt wurde, ist es nicht mehr möglich, den Koordinator zu ändern.
{% endhint %}

The Coordinator of an [Order Cycle](order-cycles-for-hubs.md) can:

* Create the order cycles
* Set and edit the name of the order cycle as well as the opening and closing dates.
* Apply enterprise fees to all products (coordinator fee), to products supplied by producers (in the [incoming](permissions-in-multi-enterprise-order-cycles.md#incoming) section), and/or to products distributed by hubs (in the [outgoing](permissions-in-multi-enterprise-order-cycles.md#outgoing) section).

### **Incoming**

* The coordinator can add enterprises as suppliers. However, to do this the supplying enterprise (registered as a [Producer](../../enterprise-profile/package-types.md#for-producers) with OFN) must have granted the coordinating hub [permission to add their products to an order cycle](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md#granting-and-managing-permissions).
* The coordinator can select all or a subset of products from their suppliers that they wish include in the order cycle.
*   The coordinator can apply differential [enterprise fees](../enterprise-fees.md) to each supplier. For example, they may wish to charge a supplying butcher a higher rate (to cover the extra cost of refrigerated transport) than a baker.



### Ausgehend von

The coordinator can choose which enterprises the products listed in an order cycle are distributed through (including themselves).

To do this each potential distributor must be:

1. Registered as a [Hub](../../../your-quick-start-on-ofn-given-who-you-are.md#hub).
2. Have granted the coordinating hub [permission to add products](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md#granting-and-managing-permissions) to an order cycle.
3. Have at least one active [shipping](../shipping-methods.md) and [payment](../payment-methods.md) method.&#x20;

{% hint style="info" %}
If a potential distributing enterprise appears in the list of possible options in the outgoing section of the order cycle but can not be selected then it is probable that they haven't set up shipping and/or payment methods yet.
{% endhint %}

The coordinator can choose from the complete list of incoming products, which will be displayed on each distributing Hub's shopfront. _**The supplier (producer profile or shop) must have set up an**_ [_**enterprise permission**_](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) _**of 'add to order cycle' between themselves and the specific distributing hub (as well as the coordinator)**_.

The coordinator can apply differential [enterprise fees](../enterprise-fees.md) to each distributing hub if desired. This might be advantageous if one hub is further away from the coordinator than another, and hence would have a higher transport overhead associated with it.

## Versorgung von (eingehenden) Unternehmen

The supplier ([producer](../../enterprise-profile/package-types.md#for-producers)) can view all the order cycles they’re involved with by visiting the order cycle summary page (from the top horizontal blue menu), even if they haven't created the order cycles themselves. \
By clicking on the order cycle an incoming producer can see their details only, not the products or details of others involved in the order cycle.  They can edit items relating to themselves: for example they can remove a product which is out of stock from an order cycle.\
A supplying enterprise can not alter the name nor dates of an order cycle.

In the Reports section (top horizontal blue menu) an incoming supplying producer can view the orders they have received for the order cycle

{% hint style="warning" %}
An incoming supplying enterprise does not automatically see the names of customers who bought their products if they are not also the order cycle coordinator. This setting can be changed by the order cycle coordinator (enterprise that manages the order cycle). If you need to see customer names to facilitate packing and fulfilment of orders, you can contact your order cycle coordinator and ask them to select the Customer Names in Reports checkbox in [Enterprise Settings](../../enterprise-profile/enterprise-settings.md) under Shop Preferences.
{% endhint %}

### Eingehend

* A supplier can view, add and remove _**their**_ products from the 'Incoming Products' section of an order cycle.
* A supplier can add/remove enterprise fees which are applied to _**their**_ products in the 'Incoming Products' section of the order cycle.  This might be useful for producers who supply several hubs, some of which are much further away from them than others. They may wish to add an extra levy to more distant hubs to cove transport costs.

### Ausgehend von

The degree of influence a supplier has over their products in the 'Outgoing Products' section of an order cycle depends on the specific enterprise permissions they granted the distributing hub and vice versa.

* If the distributing hub granted the supplying producer (profile, shop or hub) the right to 'add to \[the hub's] order cycle' then the supplier can view, add and remove products from the list in the 'Outgoing Products' section of the order cycle.
* If the distributing hub did not grant the supplying producer (profile, shop or hub) the right to 'add to \[the hub's] order cycle' then the supplier can view but NOT add and remove products from the list in the 'Outgoing Products' section of the order cycle.
* A supplier is never able to change the pickup/delivery details, or the enterprise fees applied to the distributor.

## Verteilendes (ausgehendes) Unternehmen

A distributor can view Order Cycles they’re involved with in their Order Cycle summary page, even if they did not create them themselves (ie. they are not the order cycle coordinator). \
By clicking on an order cycle, the outgoing distributing enterprise can see the details of an order cycle which relate to them only.  (For example, if they are not the sole distributor of the order cycle they will not be able to see who the other distributing enterprises are nor the products they will offer on their shop front.)\
The outgoing distributing hub can view and edit details of their distribution- delivery dates and methods, and enterprise fees for distribution- but no the name nor period of the order cycle itself.

In the 'Reports' menu, a order cycle distributor can view the orders which have been placed (along with customer names) to aid delivery/dispatch of goods.

### Eingehend

A distributor can _**view**_ the incoming products of supplier who have granted them the enterprise permission 'add to order cycle' but they can not edit stock levels/availability nor apply/remove producer specific enterprise fees.

{% hint style="warning" %}
At present, only the coordinator of an order cycle can add extra suppliers (producers) to it.
{% endhint %}

### Ausgehend von

The degree of influence the distributing hub has over the products in the 'outgoing products' section of an order cycle, depends on the enterprise permissions between them and the supplying producer.

* The distributing hub can add/remove products from its outgoing exchange. This only applies to product from producers who been added to the order cycle by the coordinator, and have granted the distributor the enterprise permission 'add to order cycle'.
* Can change the pickup/delivery details
* Can add/remove their enterprise fee
