# Cicli di richieste \(per Hub\)

{% hint style="warning" %}
Leggi qui se il tuo profilo è un profilo '[Hub, sia produttore che non produttore](../../../your-quick-start-on-ofn-given-who-you-are.md#hub)'. 

Visita questa [pagina](order-cycles-for-producers.md), se sei invece registrato come '[Negozio Produttore](../../../your-quick-start-on-ofn-given-who-you-are.md#shop)' e vuoi impostare un ciclo di richieste per il tuo negozio.
{% endhint %}

Per aprire il tuo negozio devi creare un Ciclo di Richieste. Quando crei un ciclo di richieste, selezioni un periodo di apertura del tuo negozio \(da quando a quando\), quali prodotti vuoi mostrare nella tua vetrina e quali tariffe intendi applicare.

**Perchè Cicli di Richieste?**    
Alcuni hub potrebbero volere il proprio negozio online sempre aperto e soddisfare le richieste una alla volta, via via che le ricevono. Ma molti hub preferiscono invece lavorare con un sistema di richieste periodiche, che permette loro di affrontare con maggior efficienza le attività di produzione, confezionamente e distribuzione \(riducendo così i costi associati\). 

Per esempio, un ciclo di richieste può essere aperto per due settimane. Una volta raccolte tutte le richieste, queste possono essere preparate e consegnate nello stesso momento, il mercoledì successivo alla chiusura. Dopo aver consegnato i prodotti, l'hub può riaprire un nuovo ciclo di richieste, e così via. 

Una rapida presentazione di come impostare un nuovo ciclo di richieste:

![](../../../.gitbook/assets/ordercyclehub.gif)

## Visualizzare i Cicli di Richieste

Puoi creare un ciclo di richieste e vedere i cicli di richieste esistenti cliccando su **Gestisci Cicli di Richieste** da tuo [pannello di controllo](../../dashboard.md).

![](../../../.gitbook/assets/ordercycledash.jpg)

O dal menu orizzontale in alto \(**Cicli di richieste**\)

![](../../../.gitbook/assets/ordercycle1%20%282%29%20%282%29%20%282%29.jpg)

{% hint style="warning" %}
NB Per poter pubblicare un ciclo di richieste, dovrai aver prima impostato per la tua azienda almeno un [metodo di pagamento](https://app.gitbook.com/@ofn-user-guide/s/ofn-user-guide-master/~/drafts/-M_UynsQV5vzExOcrhs9/v/it/basic-features/shopfront/payment-methods) ed almeno un [metodo di spedizione](https://app.gitbook.com/@ofn-user-guide/s/ofn-user-guide-master/~/drafts/-M_UynsQV5vzExOcrhs9/v/it/basic-features/shopfront/shipping-methods).
{% endhint %}

## Creare un nuovo Ciclo di Richieste

Il primo passo è selezionare un coordinatore per il tuo ciclo di richieste. Solo il coordinatore ha il permesso di modificare **tutti** gli aspetti del ciclo.  
Le altre imprese coinvolte \(come fornitori o distributori\), avranno un accesso parziale.    
Per maggiori informazioni sulle possibilità di controllo incrociato dei cicli di richieste, [clicca qui](permissions-in-multi-enterprise-order-cycles.md).

![](../../../.gitbook/assets/ordercycle2.jpg)

Una volta scelto il coordinatore del ciclo di richieste, il processo di impostazione si divide in tre passaggi: 

### 1\) Impostazioni generali

![](../../../.gitbook/assets/ordercycle3%20%281%29.jpg)

**Nome \(**_**obbligatorio**_**\):** Dai al ciclo di richieste un nome che sia significativo per te. Ti suggeriamo di seguire una regola di nominazione, per poi riuscire a trovare agevolmente il ciclo di richieste ad una ricerca futura. Ti suggeriamo inoltre di inserire il nome del tuo hub nel nome del ciclo di richieste, di modo da permettere un agevole supporto da parte di OFN in caso di necessità. Es. NomeCoordinatore\_settimana12\_2021.

**Richieste aperte dal:** Questa è la data e l'orario a partire da cui il tuo negozio OFN sarà aperto, visibile e pronto ad accettare richieste dai consumatori. 

**Orders Close:** This is the date \(and time\) when your OFN store will close and stop accepting orders. If you intend to have an order cycle which is continuously open, select a close date which is well into the future.

**Schedules:** Leave blank unless using [Subscriptions](../../subscriptions/).

**Add Coordinator Fee:** As a hub, the coordinator is most likely you. Here you can apply your Enterprise Fee which acts as the markup. The fee will be calculated according to the calculator selected in [Enterprise Fees](../enterprise-fees.md). You can only apply an enterprise fee which has previously been created.

### 2\) Incoming Products

![](../../../.gitbook/assets/ordercycle4.jpg)

On this page you can select the producers, and their produce, which will be available in this order cycle. In the dropdown menu you will see all producers who have granted you permission to add their produce to your order cycle \(See [Enterprise Permissions](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) section\).   
After selecting a supplier and clicking **Add Supplier** all of the products associated with that supplier will be visible. Check those products you wish to add to the store, or click **select all.** 

{% hint style="info" %}
Products which are out of stock \(ie their 'in stock' value is zero\) are included in this list.  If added to an order cycle they will not appear on our shop front.  It is always good to double check stock levels. 
{% endhint %}

The **Receival Details** field is optional.  Information added to this field will automatically added to any email sent to producers at the end of an order cycle \(after clicking 'Notify Producers'\).  It might be a good idea to include an exact delivery address for produce prior to distribution to customers here.

The **Add Fee** button in this section, at the end of each producer's entry in the table, allows you to add different [enterprise fees](../enterprise-fees.md) to different suppliers. For example, transporting flour or heavy goods to customers may be more expensive for a hub than salad.  Hence, a hub can, in a transparent manner, add a slightly higher enterprise fee to all goods supplied by the flour miller than the salad farmer.

Select the name of the enterprise in the first dropdown box, then click the name of the enterprise fee in the second dropdown box. In the example below, an enterprise fee named OrderAdmin is applied to the Producer of Fruit.

![Apply enterprise fee to incoming supplier](../../../.gitbook/assets/enterprise-fee.png)

{% hint style="warning" %}
This fee will be applied to all of the Producer of Fruit’s products which are purchased. The fee is calculated according to the fee calculator which was selected when the [Enterprise Fee](../enterprise-fees.md) was created.
{% endhint %}

### 3\) Outgoing Products

Here you can select one or more hub-distributors.  All hubs chosen to be a distributor in this order cycle will have an open shop front for the duration of the order cycle.  
In a **simple model**, only one hub is listed as the sole distributor for the order cycle. Select the hub, and check the box 'Select all' to add all incoming products to the shop front.   
For more flexibility, the same order cycle may have **multiple hub distributors**.  In this case you may wish to select a different subset of the available incoming products for each distributor, and/or, add different delivery dates for each.

![](../../../.gitbook/assets/oc3.jpg)

The **tags** column is where you can tag your order cycles to customise whether they are visible/invisible to certain customers. See [tags and tag rules](../customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) for more information.

The **‘ready for \(ie Date/Time\)’ \(**_**required**_**\):** This box tells the customer when their order will be ready for either collection or delivery. If your order cycle is a perpetual one, which fulfils orders on an individual basis rather then in bulk, you should enter something like ‘Two days after order is received’. The example below shows how a customer can toggle between different order cycles to select the date which suites them best.

![](../../../.gitbook/assets/multipleoc3.jpg)

The note is also shown at check out, when the customer selects their shipping method \(see below\) and is included in the order confirmation email.

![](../../../.gitbook/assets/readyfor2.jpg)

The **Pick-Up Instructions** message will be included in the customer’s order confirmation email, below the message that corresponds to their chosen shipping method \(see below\). This note is designed to only be visible to customers, so you can include more sensitive information like addresses, or phone numbers etc. See below for an example of the order confirmation email.

![collection details message](../../../.gitbook/assets/collection-details.png)

**Add Fee:** Again, a previously created enterprise fee can be assigned to this distributor.  For simple models \(with one hub distributor, who also is the coordinator of the order cycle\) adding a fee at this stage is the same as adding a 'Coordinator Fee' \(it will apply to all products\).  
For complex models, the coordinator may wish to add different fees to all products sold though each distributor.  The best place to implement this functionality is here.

### Open the shopfront

Click **Save** to schedule the order cycle. If the opening date has already passed, your shop is instantly open! If you are not ready to open right away, enter dates in the future, which you can change later. 

For periodic, repetitive order cycles, you can copy an existing order cycle and change the dates, to make the process quicker. See below.

![](../../../.gitbook/assets/occpy.jpg)

Order cycles will display as green when they are active, yellow when scheduled for a future date, and grey when they have closed. When an order cycle close over one month ago, it will no longer display on this list. To view all of your past order cycles click ‘show more’ at the top of the list.

## **‘Notify Producers’ Button**

By using this button at the top of the page, all the Producers linked to the order cycle will receive an email containing a list of the products ordered for that particular order cycle thus far.  

![](../../../.gitbook/assets/notifyproducers.jpg)

When the Notify Producers button is selected there will be a confirmation prompt. Once confirmed, an email will be automatically sent to all relevant Producers. The email will include Delivery instructions \(if this field is completed in the incoming products section\) as well as the following product information:

* SKUs \(if relevant\)
* Name of Supplier
* Product name 
* Quantity ordered
* Price per unit
* Subtotal per product
* Included Tax \(if relevant\) 

## Producer / Supplier Reports

If your Order Cycle includes products from linked Producers / Suppliers they will be able to log in to their OFN account and view reports about the Order Cycle. By default they will not be able to see any Customer Details in these reports. If you would like your suppliers to access Customer Names in their reports, you can adjust these settings in Shop Preferences in your [Enterprise Settings](../../enterprise-profile/enterprise-settings.md).

