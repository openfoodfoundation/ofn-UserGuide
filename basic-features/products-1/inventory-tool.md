# Inventario

## Introduzione

L'Inventario consente alle aziende di avere maggiori controllo e flessibilità nella gestione dei prodotti. Questa funzionalità interessa principalmente gli Hub ed i loro gestori.&#x20;

Usando l'"Inventario", un Hub A può modificare i prezzi e le disponibilità degli articoli che ha il permesso di rivendere. Questa funzionalità permette anche ad un Hub A di rivendere nel proprio negozio online solo una selezione di prodotti dei propri fornitori se non intende proporre la loro lista completa. Tutto questo può essere fatto senza modificare la scheda originale dei prodotti e dunque senza influenzare la disponibilità di quei prodotti per altri Hub. Se ad esempio gli Hub A e B rivendono gli stessi prodotti, l'Hub A, utilizzando lo strumento Inventario, può alterarne il prezzo ed altre informazioni fondamentali senza influenzare l'Hub B.&#x20;

## Impostazioni di profilo per l'Inventario

Per accedere all'Inventario, vai su 'Aziende' (nel menù azzurro orizzontale) e poi 'Impostazioni'. Dal menu a sinistra, seleziona quindi 'Impostazioni Inventario'.&#x20;

![](../../.gitbook/assets/inventory-settings.png)

Hai due opzioni:&#x20;

* **I nuovi prodotti possono essere inseriti nella mia vetrina (suggerita):** I prodotti dei tuoi fornitori possono essere aggiunti nella tua vetrina _senza che tu debba prima aggiungerli nel tuo inventario_. Quando crei un ciclo di richieste, _tutti_ i prodotti dei produttori selezionati potranno essere inseriti nei tuoi prodotti 'in entrata'. \
  Questa è l'opzione di default ed è suggerita per gli hub che non desiderano modificare prezzo e disponibilità dei prodotti che rivendono.&#x20;

{% hint style="warning" %}
ATTENZIONE - se mantieni questa opzione di default, ma allo stesso tempo aggiungi prodotti nell'inventario del tuo hub e modifichi i loro prezzi e le loro disponibilità, le informazioni modificate saranno visibili sul tuo negozio online, non nella scheda originale del prodotto.&#x20;
{% endhint %}

* **I nuovi prodotti devono essere aggiunti al mio inventario prima di poter essere inseriti nella mia vetrina:** Quando crei un ciclo di richieste, solo quei prodotti che son stati inseriti nel tuo inventario saranno visibili nella sezione 'in entrata' del tuo ciclo di richieste.&#x20;

## Visitare l'inventario del tuo Negozio o Hub

Dal menù azzurro orizzontale, clicca su 'Prodotti' e poi su 'Inventario' nel sottomenù verde. Se gestisci più di un'azienda, ti sarà chiesto di selezionarne una, perchè ogni Inventario è gestito indipendentemente.&#x20;

![](../../.gitbook/assets/inventory1.jpg)

Se i tuoi fornitori hanno aggiunto nuovi prodotti dall'ultima volta che hai visitato l'inventario del tuo hub, allora visualzzerai il seguente messaggio:&#x20;

![](../../.gitbook/assets/new-products-alert.png)

Finchè non avrai aggiunto questi prodotti a tuo inventario, rimarranno nella categoria '**Nuovi Prodotti**' e non saranno visibili quando crei un nuovo ciclo di richieste. Cliccando su '**Rivedi adesso**' sarai ridiretto alla lista dei nuovi prodotti. &#x20;

## Revsione Nuovi Prodotti

I nuovi prodotti possono essere **Aggiunti** al tuo inventario oppure **Nascosti**. Se c'è un prodotto nella lista per il quale desideri sovrascrivere informazioni, dovrai **aggiungerlo** alla lista del tuo inventario. Se c'è un prodotto che non vuoi vendere nel tuo negozio, o che non vuoi immagazzinare nel prossimo futuro, puoi decidere di **nasconderlo** (vedi sotto la sezione **Prodotti Nascosti**).&#x20;

![](../../.gitbook/assets/new-products.png)

{% hint style="info" %}
Ricorda, se nelle tue **Impostazioni Inventario** hai selezionato "I nuovi prodotti devono essere aggiunti al mio inventario prima di poter essere inseriti nella mia vetrina", tutti i prodotti che lasci nella lista dei Nuovi prodotti saranno nei fatti nascosti. Se hai selezionato "I nuovi prodotti possono essere inseriti nella mia vetrina", allora i prodotti nella lista dei Nuovi prodotti saranno visibili nei prodotti in entrata dei tuoi cicli di richieste.
{% endhint %}

## Gestire i tuoi Prodotti in Inventario

La tua lista di Prodotti in Inventario è dove puoi sovrascrivere i dettagli dei prodotti, cambiarne le disponibilità, nascondere i prodotti.

![](../../.gitbook/assets/viewing-inventory-settings.png)

Attraverso il pulsante 'Colonne' a destra della tabella, puoi scegliere quali campi visualizzare e modificare.&#x20;

![](../../.gitbook/assets/columns-1.png)

### Modificare Codice ID, prezzi e disponibilità per i prodotti nella tua vetrina

Le modifiche che apporterai qui saranno visibili nel tuo negozio dove sovrascriveranno i dettagli impostati dal produttore. Puoi modificare i seguenti campi: &#x20;

* **Codice ID** – se desideri utilizzare un codice ID alternativo per un prodotto, puoi sovrascrivere il codice ID inserito dal produttore, digitandone uno qui.
* **Prezzo** – Puoi impostare un prezzo differente da quello originale da mostrare nel tuo negozio. Le 'unità' del prodotto rimarranno però le stesse, quindi se un prodotto è venduto al kg non potrai impostare un prezzo ad articolo.&#x20;
* **Disponibile** – Se la disponibilità per il tuo negozio di questo prodotto differisce da quella generica del produttore, puoi indicare qui la quantità disponibile per te. Questi prodotti non saranno più visibili nel tuo negozio quando la disponibilità arriverà a zero.

{% hint style="info" %}
Questo potrebbe esserti utile se ad esempio ricevi un pacco di 50 pezzi al mese ed hai bisogno di tenere traccia delle relative vendite prima della consegna successiva. &#x20;
{% endhint %}

* **A richiesta?** – Puoi selezionare se ereditare le quantità disponibili dal produttore (in questo caso il numero nella colonna "disponibile" rimarrà grigio e non modificabile), se avere disponibilità illimitata, selezionando 'Sì' (quindi il prodotto non si esaurirà mai e sarà sempre disponibile se aggiunto ad un ciclo di richieste attivo), o se definire le tue proprie quantità disponibili, selezionando "no" (quindi il numero nella colonna "disponibile" avrà sfondo grigio e sarà modificabile).&#x20;

![](../../.gitbook/assets/inventorystock.jpg)

Puoi ripassare i campi 'disponibile' e 'a richiesta' [qui](products.md#adding-products).

{% hint style="warning" %}
Non è possibile modificare il nome, le proprietà, la descrizione o l'immagine di un prodotto.
{% endhint %}

### Permetti Reset Disponibilità?

The **enable stock level reset** column allows you to reset the 'In Stock' amount to a default value, **** for example at the start of each new order cycle. The **default amount** is the number entered in this column next to the check box. The checkbox allows you to select only those items that you want to reset at any give time.&#x20;

To reset the default stock for these products, click 'Actions' at the top left of the inventory table and then 'Reset stock levels to defaults'. Only products for which the enable stock reset box has been checked will be affected by this action.&#x20;

![](../../.gitbook/assets/inventorystockreset.jpg)

> In this example the default stock level of baked beans is 5. There are currently 2 left in stock. If the user, at the beginning of an order cycle wishes to reset to 5 then they must click on 'Reset stock levels to defaults' under 'Actions'

{% hint style="info" %}
This is a useful feature for hubs who may receive deliveries of specific products once a month or on a regular schedule.&#x20;
{% endhint %}

### Inherit?

If you have not changed any of the values in the Inventory table for a product, the check box "inherit?" will be, by default, checked. This means that the information entered by the producer and visible in grey will be displayed on your shopfront.

![](../../.gitbook/assets/inventoryinherit.jpg)

By modifying one or more of the fields, this check box will be automatically de-selected. To reset values (price, stock, SKU etc) to the producer's master copy values, you can re-select this box at any time.

### Hide

As in the **New Products** list, you can also **hide** products from your **Inventory List**. Clicking on the hide button will move the product to your **Hidden Products** list. If you have your inventory profile set up as '**New products must be added to my inventory before they can be added to my shopfront'** (see [here](inventory-tool.md#profile-settings-for-the-inventory)) then the product you just hid will no longer be available for selection in your hub's order cycle and thus will not be visible on your shopfront.

## Hidden Products

This is a list of all the products you have chosen to hide:

![](../../.gitbook/assets/hidden-products.png)

When viewing your list of hidden products you can choose to make them visible once more by clicking the '**Add**' button to the right of the item.

![](../../.gitbook/assets/inventoryhidden.jpg)

## Inventory and Order Cycles

When setting up order cycles you can on a case by case basis choose between selecting from all available products or only those which are in your shop/hub inventory.&#x20;

This is controlled by visiting 'Advanced Settings' (top right of order cycle page):

![](../../.gitbook/assets/advanced-oc-settings.png)

This option has the same effect as changing our enterprise [profile settings for your inventory](inventory-tool.md#profile-settings-for-the-inventory), but unlike the latter it applies only to the order cycle in question.

{% hint style="danger" %}
After making any changes always remember to click 'Update' or 'Save' before moving on!
{% endhint %}
