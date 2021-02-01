# Metodi di Spedizione

{% hint style="warning" %}
 Devi creare almeno un metodo di spedizione prima di poter aprire il tuo negozio. 
{% endhint %}

Qui sotto trovi un breve tutorial \(in inglese\):

![](../../.gitbook/assets/shippingmethod.gif)

## Impostare un metodo di spedizione

* Puoi accedere alla pagina "Metodi di Spedizione" cliccando su **Aziende** nel menù azzurro orizzontale e poi su **Impostazioni**, accanto al nome della tua azienda. La voce "**Metodi di Spedizione**" si trova nel menù laterale a sinistra.
* Clicca su **Crea un nuovo metodo di spedizione**. Sarai indirizzato ad una pagina come questa:

![](../../.gitbook/assets/shippingmethods.jpg)

* Controlla il riquadro a destra "HUB". Puoi selezionare le aziende \(anche più di una, se occorre\) a cui applicare il metodo di spedizione che stai creando. 
* **Nome**: Scegli un nome per il metodo. Questo nome sarà visibile nella schermata dedicata nel processo d'ordine e nelle mail di conferma che verranno inviate ai tuoi clienti. Esempio:

![](../../.gitbook/assets/shippinginfo.jpg)

* **Descrizione:** Aggiungi ulteriori dettagli, come l'indirizzo completo del punto di ritiro. Questi dettagli saranno mostrati in un riquadro grigio di fianco al nome, quando selezionato.
* **Visualizza:** Puoi scegliere tra "Solo Back Office" o "Entrabi Checkout e back office"

{% hint style="info" %}
Se vuoi disattivare un metodo di spedizione temporaneamente, ma hai intenzione di riattivarlo in seguito \(ad esempio un punto di ritiro estivo, non attivo in inverno\) allora puoi selezionare "Solo Back Office".
{% endhint %}

* **Category:** Is this method a delivery or pick-up?
* **Tags:** enter labels here if you wish to differentiate between customers. Tags could be useful if you want to offer free shipping to a sub set of customers or only offer delivery to those who have a registered address which is close by.  Read more [here](customer-management-and-conditional-displays-prices/).
* **Calculator:** Select the way that shipping fees will be added to this shipping method.  Note that a shipping fee may be zero. See below for more details.
* **Categories:** Transport conditions \(refrigeration, frozen, default\) associated with this shipping method.
* **Zones:** Select the appropriate zone \(this is to enable correct tax calculations\).

By clicking **Create,** the shipping method will be created, and you will then be provided with new fields, to add details of the shipping method charges. The fields presented will depend upon which shipping fee calculator you have selected. 

{% hint style="info" %}
If you change the calculator type for a shipping method, you must **save first** before you can edit the calculator settings.
{% endhint %}

## Fee Calculators

![](../../.gitbook/assets/shippingcalc.jpg)

**Weight \(per kg\)** – this fee is applied to products on a per kg basis. The fee will _only be applied to products which are priced at a per kg rate_, not products listed as items \(e.g. A product listed as ‘1 bunch of parsley’ will not contribute to the overall fee a customer is charged for shipping\)

**Flat Percent** – This fee is charged as a percentage of the total amount spent in the order.

**Flat Rate \(per order\)** – This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate** – This fee calculator is especially useful if you'd like to encourage customers to place large orders: the cost of shipping can be reduced or zero when the threshold number of items has been reached. 

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for items beyond the first item.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

![](../../.gitbook/assets/shippingfeeflex.jpg)

> For example: If the shipping fee for the 'First item cost' is £2, 'Additional Item Cost' = £1 and 'Max items' = 3.   
> A customer who purchases 5 items, will be charged £4 shipping \(£2 for the first item, £1 for items two and three, and £0 for items four and five\).

**Flat Rate \(per item\)** – This fee is a constant fee, applied to products listed as ‘items’. \(It is not applied to products sold by weight or volume. Hence there will be no associated shipping cost charged to a customer who, for example, buys rice by kg\).

**Price Sack** – This is a flexible shipping fee method charged by _total monetary sale_, rather than number of items purchased \(Flexible Rate above\)

* ‘Minimum Amount’: Monetary value of the threshold between Normal shipping fee and Discounted shipping fee. 
* 'Normal Amount': Shipping fee applied to sales below the threshold stated in 'Minimum Amount'.
* ‘Discount Amount’: Shipping fee applied to sales above the threshold stated in 'Minimum Amount'.

![](../../.gitbook/assets/shippingfeepc.jpg)

