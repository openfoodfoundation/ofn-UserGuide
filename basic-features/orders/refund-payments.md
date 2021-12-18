# Rimborsi ed Aggiustamenti nei Pagamenti

Occasionalmente, ti può capitare di dover aggiustare l'importo pagato da un cliente per la sua gentile richiesta. Alcuni scenari comuni sono:&#x20;

* Richieste contenenti prodotti con peso variabile non noto al momento della richiesta (come [carne o grandi ortaggi](../products-1/pricing-irregular-items-kg.md), con prezzo al kg ma venduti al pezzo intero)&#x20;
* Prodotto richiesto non consegnato dal produttore.&#x20;
* Richiesta da parte del cliente di aggiunte di prodotti dopo l'avvenuto pagamento.&#x20;
* Uno o più prodotti di qualità inferiore alle aspettative per cui desideri procedere ad un rimborso.&#x20;

&#x20;Generalmente si possono verificare due casi:

* Al cliente è richiesto il **pagamento alla consegna** e dunque non si effettuano pagamenti in anticipo. In questo caso, puoi correggere la gentile richiesta, reinviare la mail di conferma e  richiedere il pagamento corretto il giorno della consegna.
* Il **pagamento avviene al momento della conferma della richiesta** (Stripe, PayPal..). In questo caso ci sono tre opzioni:&#x20;
  1. Il saldo è in CREDITO (tu devi un importo al cliente) e desideri rimborsarlo.&#x20;
  2. Il saldo è in CREDITO e desideri che il cliente possa utilizzare il suo credito per i suoi acquisti futuri.&#x20;
  3. Il saldo è in DEBITO (il cliente ti deve un importo)&#x20;

## Come rimborsare un Pagamento

### Rimborsare un pagamento Stripe

_Se il cliente ha effettuato il pagamento sul tuo account business di Stripe, puoi ettuare un rimborso parziale o totale dall'interfaccia amministrativa di OFN._&#x20;

Assicurati che la richiesta che desideri rimborsare sia contrassegnata come 'PAGATA':&#x20;

![](<../../.gitbook/assets/image (17).png>)

Correggi la richiesta come da necessità (leggi [qui](view-orders.md#editing-an-order) per come modificare una gentile richiesta, oppure approfondisci la [gestione tabellare delle richieste](view-orders.md#bulk-order-management) per i casi di [mancanza di prodotti](view-orders.md#example-1-you-have-a-stock-shortage-and-must-reduce-customer-order-quantities-for-a-certain-product) o di [prodotti dal prezzo indefinito nel momento della richiesta](../products-1/pricing-irregular-items-kg.md)).

Ti comparirà quindi un CREDITO nella richiesta modificata. Clicca sulla spunta a destra per effettuare il rimborso via Stripe:&#x20;

![](../../.gitbook/assets/capture-du-2019-02-27-20-04-19.png)

Il rimborso sarà registrato sul tuo account business di Stripe:&#x20;

![](../../.gitbook/assets/stripecredit.png)

{% hint style="info" %}
I rimborsi impiegano dai 5 ai 10 giorni per apparire nell'account del cliente.&#x20;
{% endhint %}

{% hint style="warning" %}
Le tariffe applicate da Stripe (1.4% - 2.9% + 0,20€ per transaction) non ti vengono rimborsate: sono calcolate in base all'importo originariamente pagato. \
Potrebbe dunque essere più vantaggioso offrire al cliente un credito per le sue future gentili richieste piuttosto che effettuare un rimborso.&#x20;
{% endhint %}

Se una richiesta è stata completamente cancellata, puoi effettuare un rimborso totale (se il cliente ha pagato via Stripe): [Modifica la richiesta](view-orders.md#editing-an-order) --> Pagamenti. Seleziona la croce a destra della tabella:&#x20;

![](../../.gitbook/assets/stripefullrefund.png)

### Rimborsare un pagamento PayPal

Rimborsi parziali o totali automatici per pagamenti via PayPal non sono al momento supportati da OFN. Dovrai accedere al tuo account business di PayPal ed effettuare il rimborso da lì. \
Questa è una funzionalità che speriamo di sviluppare in futuro.&#x20;

### Rimborsare un Pagamento via bonifico

_Un cliente ha pagato per i propri acquisti con un bonifico o qualsiasi altro metodo non automatizzato (qualsiasi altro metodo eccetto Stripe o PayPal) ed hai già registrato il pagamento. Successivamente è necessario modificare la sua gentile richiesta (un prodotto non è disponibile o è danneggiato). Dopo aver modificato la richiesta, la differenza tra l'importo pagato e l'importo dovuto viene visualizzata come CREDITO nella sua richiesta._\
__Per effettuare un rimborso, dovrai farlo attraverso la tua banca. __&#x20;

## Come considerare un CREDITO per le gentili richieste future

Un'alternativa al rimborso potrebbe essere sottrarre manualmente il credito dalla prossima gentile richiesta del cliente.&#x20;

{% hint style="info" %}
Attualmente, come gestore di un Negozio o di un Hub, occorre correggere manualmente il saldo di un consumatore per prendere in considerazione il suo credito precedente. In fuuro vorremmo automatizzare questo processo. Per favore  se credi possa essere una funzionalità utile per la tua azienda.&#x20;
{% endhint %}

## Come aggiungere importi al conto

Per esempio, un cliente ti chiede di aggiungere un prodotto ad una sua gentile richiesta già pagata, oppure un [prodotto venduto al pezzo ma pagato al peso](../products-1/pricing-irregular-items-kg.md) potrebbe essere risultato più grande della media prevista e dunque l'importo dovuto risulta maggiore dell'importo già pagato. \
Ogni importo aggiuntivo va registrato manualmente. Il cliente non potrà pagare importi aggiuntivi via Stripe o PayPal attraverso OFN.

{% hint style="info" %}
Se un cliente vuole aggiungere un articolo alla sua gentile richiesta già pagata via Stripe o PayPal, potrebbe essere più semplice chiedergli di creare una nuova richiesta, piuttosto che modificare quella già presente.&#x20;
{% endhint %}
