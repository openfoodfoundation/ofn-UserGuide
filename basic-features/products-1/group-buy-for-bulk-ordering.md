# Acquisto di gruppo

La funzionalità di **Acquisto di gruppo** è pensata per le aziende che acquistano all'ingrosso per rivendere in confezioni al dettaglio (ad esempio, acquistano il riso in sacchi da 25 kg e poi lo rivendono ai consumatori al kg).&#x20;

L'acquisto di gruppo è una pratica comune tra i GAS (Gruppi di Acquisto Solidali), che, acquistando grossi volumi, possono usufruire di prezzi all'ingrosso al pari dei distributori convenzionali. Così facendo, i soci ottengono prezzi più convenienti rispetto a quelli che troverebbero nei negozi.&#x20;

Queste realtà possono decidere di ordinare un certo prodotto solo se i consumatori hanno ordinato collettivamente una quantità sufficiente ad ottenere un prezzo più conveniente, grazie a sconti sui volumi o tariffe di consegna. Questa funzione rende più agevole per gli hub ottenere efficienze da acquisti "massivi".

Quando si imposta la funzionalità di acquisto di gruppo per un prodotto, quando il consumatore lo selezionerà per acquistarlo, comparirà una finestra pop up, con la richiesta di quantità minima e massima:

![](<../../.gitbook/assets/Acquisto di gruppo.png>)

* La quantità **minima** - è la quantità ideale per il consumatore.&#x20;
* La quantità massima - è la quantità massima che il consumatore è disposto ad acquistare per eventualmente raggiungere il minimo richiesto.&#x20;

{% hint style="info" %}
In pratica, questa è una modo per far dire al consumatore: "avete il mio permesso di aumentare il mio ordine fino a questo limite se questo permette al gruppo di ottenere la quantità minima richiesta dal fornitore."&#x20;
{% endhint %}

Nella [gestione tabellare degli ordini](../orders/view-orders.md#bulk-order-management), puoi visualizzare la quantità minima e massima richiesta da ciascun consumatore per ciascun prodotto in cui questa funzionalità è stata attivata. Da qui puoi aumentare la quantità degli ordini per raggiungere il minimo richiesto, oppure cancellare gli ordini nel caso il minimo non sia raggiunto.&#x20;

## Enabling Group Buy for a product

On the admin dashboard, go to '**Products**' on the blue horizontal menu.  Select to **Edit** a product by clicking on the pencil and paper icon to the right of the product in question:

![](../../.gitbook/assets/productedit.jpg)

Then select **Group Buy Options** in the menu to the right.

![](../../.gitbook/assets/groupbuy.jpg)

Select **Yes** under **Group Buy? to activate this feature for the product.**

The **Bulk Unit Size** is the amount that the group’s collective order needs to reach.&#x20;

{% hint style="warning" %}
The **units** for the Bulk Unit Size quantity depend on the units selected for retailing the product to customers. &#x20;

If the product is sold by:

* **Weight**: units are in g (so if collective total must equal 5 kg then enter '5000' in this field)
* **Volume**: units are in litres (so if collective total must be 10 l then enter '10' in this field)
* **Items**: eg. selling bunches of flowers but must purchase 100 bunches in total then enter '100' in this field.
{% endhint %}

## Adjusting Orders to make complete Batches

Under Orders-> [bulk order management](../orders/view-orders.md#bulk-order-management) you can view and edit customer orders for Bulk Buy products to make the combined order from all customers reach your required threshold.

1. Select the order cycle or date range of interest.
2. Search for the product (Fish in the example below).
3. Make sure the ‘Max’ column is displayed so you can see the upper limit each customers is prepared to purchase.
4. Next, click on the value ('test fish: Fish One' in the example below) in the **Product : Unit** column, to display the orders total box (in blue) for the product in question.&#x20;
5. Using the information in the column **Max**, you can increase the quantities ordered to reach the threshold for a complete batch.&#x20;
6. Click update to save changes to customer orders.

![](../../.gitbook/assets/bulkorder2.jpg)

**Current Fulfilled Units** divides your total quantity ordered by the group buy unit size. If this figure is greater than 1, it tells you that the existing customer orders satisfy or exceed your required group buy unit size. If this figure is less than 1, existing customer orders don’t meet that threshold. As you raise the quantity of customer orders, this figure will raise.&#x20;

**Max Fulfilled Units** takes the sum of all of the customer’s MAX order quantities and divides this by the Group Buy Unit Size. If this figure is greater than 1, then you know that the total of your MAX orders exceeds the required group buy quantity. If this figure is less than 1, it means that even the MAX order quantities won’t reach the threshold.
