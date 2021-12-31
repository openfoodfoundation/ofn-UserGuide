# Etichette e Regole di Etichette

Una volta che i clienti sono stati raggruppati in categorie tramite le etichette, potrai personalizzare la loro esperienza di acquisto nei modi seguenti:

* Rendendo visibili/invisibili determinate varianti
* Rendendo visibili/invisibili determinati metodi di spedizione
* Rendendo visibili/invisibili determinati metodi di pagamento
* Rendendo visibili/invisibili determinati cicli di richieste

Questa funzionalità generalmente è utile per i 'negozi' che hanno impostazioni differenti per soci/non soci o per clienti al dettaglio/all'ingrosso.&#x20;

## Come impostare una Regola di Etichette

Per accedere alle Regole di Etichette vai su Azienda --> Impostazioni --> Regole To access Tag Rules go to Enterprises -> Settings -> Regole Etichette

![](../../../.gitbook/assets/newtagrule1.jpg)

## Predefinito

Di default, _**tutti i prodotti**_ sono visibili per _**tutti i clienti**_, con o senza etichette.  \
Puoi modificare le regole predefinite di visualizzazione selezionando **+ Aggiungi nuova regola predefinita**. Nell'esempio di seguito, per impostazione predefinita, tutti i Cicli di Richieste che hanno l'etichetta 'Ingrosso' saranno invisibili. (In questo esempio, solo i clienti con l'etichetta 'clienteingrosso' potranno visualizzare i cicli di richieste che hanno l'etichetta 'ingrosso')&#x20;

![](../../../.gitbook/assets/defaulttag.jpg)

## Regole Etichette

Una volta impostate le regole predefinite, puoi impostare le eccezioni per determinati gruppi di clienti.&#x20;

* Innanzitutto stabilisci il gruppo di clienti a cui applicare l'eccezione. Nell'esempio precedente, l'eccezione è stata applicata a tutti i clienti con l'etichetta 'clientiingrosso'.&#x20;
* Poi, per questo gruppo di clienti, puoi personalizzare l'esperienza di acquisto in uno dei seguenti quattro modi:&#x20;

![](../../../.gitbook/assets/rule-typess.png)

{% hint style="warning" %}
Dopo aver impostato regole ed eccezioni per le etichette, ricorda di aggiungere le etichette citate sia ai clienti sia alle varianti, ai metodi di spedizione o pagamento o ai cicli di richieste.
{% endhint %}

Analizziamo tutte le opzioni, una per una:

### **Mostrare o Nascondere Varianti nella mia vetrina**

Questa regola ti permette di rendere determinate varianti visibili o invisibili per una categoria di clienti. Per rendere operativa questa regola, devi aver inserito le etichette menzionate nella regola, sia ai clienti che alle varianti dei prodotti **nel tuo inventario** (non nel listino del produttore).&#x20;

Nell'esempio seguente, alla variante di 1 kg del muesli delux è stata associata l'etichetta "socio". Sarà quindi possibile impostare una regola che preveda che di default sia visibilie solo la variante da 500g (senza etichetta), a meno che al cliente non sia associata l'etichetta "socio". Solo per questi clienti sarà allora visibile anche la variante da 1 kg.&#x20;

![](<../../../.gitbook/assets/varianttags (1).jpg>)

### **Mostrare o Nascondere Metodi di spedizione**

Questa regola ti permette di rendere disponibili o indisponibili determinati metodi di spedizione a determinate categorie di clienti. Per rendere operativa questa regola, dovrai assegnare la stessa etichetta sia al gruppo di clienti che al metodo di spedizione. Per assegnare un'etichetta ad un metodo di spedizione, vai su Aziende-->Impostazioni-->[Metodi di spedizione](../shipping-methods.md)-->Modifica.&#x20;

![](../../../.gitbook/assets/tagshipping.jpg)

In questo esempio, il metodo di spedizione 'Ritira di persona' è stato assegnato ai clienti con l'etichetta 'socio'. Si può poi impostare:&#x20;

* una regola etichette predefinita: il metodo di spedizione con l'etichetta 'socio' è invisibile
* un'eccezione alla regola: per i clienti con l'etichetta 'socio' il metodo di spedizione con l'etichetta 'socio' è visibile.&#x20;

In questo caso, solo i soci potranno scegliere di ritirare la propria spesa di persona.&#x20;

### **Mostrare/Nascondere Metodi di pagamento**

Questa regola ti permette di rendere disponibili o indisponibili determinati metodi di pagamento a determinate categorie di clienti.&#x20;

{% hint style="info" %}
Questa regola di etichette può essere utile ad esempio se desideri permettere solo ai tuoi soci di scegliere il pagamento in contanti alla consegna, mentre chiedere ai non soci di pagare in anticipo tramite carta o PayPal.&#x20;
{% endhint %}

Per rendere operativa questa regola, è necessario aver assegnato la stessa etichetta ai clienti ed al metodo di pagamento. Per assegnare un'etichetta ad un [metodo di pagamento](../payment-methods.md), vai su Aziende-->Impostazioni-->Metodi di pagamento-->Modifica.

![](../../../.gitbook/assets/tagspayment.jpg)

In questo esempio, il metodo "Contanti" è stato assegnato ai clienti con l'etichetta "socio". Si può poi impostare:&#x20;

* una regola etichette predefinita: il metodo di pagamento con l'etichetta 'socio' è invisibile
* un'eccezione alla regola: per i clienti con l'etichetta 'socio' il metodo di pagamento con l'etichetta 'socio' è visibile.&#x20;

In questo caso, solo i soci potranno scegliere di pagare la propria spesa in contanti alla consegna.

### **Mostrare/Nascondere cicli di richieste nella mia vetrina**

Questa regola ti permette di rendere determinati cicli di richieste visibili solo a determinate categorie di clienti.&#x20;

{% hint style="info" %}
Questa regola può essere utile ad esempio se desideri aprire contemporaneamente due cicli di richieste applicando diverse tariffe aziendali. Potresti voler aprire un ciclo per i clienti all'ingrosso, mostrando prodotti in pacchi grandi, con tariffe aziendali più basse, ed un ciclo pubblico, visibile a tutti, con prodotti in confezioni più piccole e con tariffe aziendali più alte.&#x20;
{% endhint %}

Per rendere operativa questa regola, devi aver prima applicato la stessa etichetta ai clienti ed ai cicli di richieste in questione. Per applicare un'etichetta ad un ciclo di richieste, vai alla sezione "[Prodotti in uscita](../order-cycle/order-cycles-for-hubs.md#3-outgoing-products)" (pagina 3) del Ciclo di richieste.

![](../../../.gitbook/assets/tagsorder.jpg)

In questo esempio, il Ciclo di richieste è stato assegnato ai clienti con l'etichetta "socio". Si può poi impostare:&#x20;

* una regola etichette predefinita: il ciclo di richieste con l'etichetta 'socio' è invisibile
* un'eccezione alla regola: per i clienti con l'etichetta 'socio' il ciclo di richieste con l'etichetta 'socio' è visibile.&#x20;

In questo caso, solo i soci potranno visualizzare questo ciclo di richieste.

## Prezzi specifici in base al cliente

A volte ci può essere l'esigenza di applicare prezzi differenti a seconda della categoria di clienti, per esempio a soci o non soci, o a clienti all'ingrosso o al dettaglio. Attualmente, non è possibile attribuire automaticamente prezzi diversi a diverse categorie di clienti, ma vi elenchiamo alcuni suggerimenti per ottenere lo stesso risultato, usando le **etichette** dei clienti e le relative regole:

* Rendere alcune varianti disponibili solo a determinati clienti: ad esempio prodotti "all'ingrosso" con un prezzo inferiore visibili solo ai clienti con l'etichetta "ingrosso".&#x20;
* Aprire più di un Ciclo di Richieste contemporaneamente e rendere visibile il ciclo con tariffe aziendali più basse solo ai soci (o ai clienti all'ingrosso)
* Usare le [tariffe collegate ai metodi di spedizione](tags-and-tag-rules.md#show-hide-shipping-methods) visibili solo a determinate categorie di clienti per applicare sconti solo a loro.
* Usare i [metodi di pagamento](tags-and-tag-rules.md#show-hide-payment-methods) disponibili solo a determinate categorie di clienti per applicare loro tariffe aziendali più basse.&#x20;

{% hint style="info" %}
Alcune aziende preferiscono creare direttamente due diversi hub: uno solo per i soci o i clienti all'ingrosso (vedi [Vetrina privata](../private-shopfront.md)) ed uno pubblico, per tutti gli altri.&#x20;

Utilizzando la funzionalità [Inventario](../../products-1/inventory-tool.md), i due hub possono offrire gli stessi prodotti ma puoi impostare i prezzi in modo differenziato.&#x20;

Questo metodo offre la maggiore flessibilità: i prezzi possono essere personalizzati uno a uno piuttosto che con una regola generale di differenza percentuale o fissa.
{% endhint %}
