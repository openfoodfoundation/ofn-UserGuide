# Permessi Aziende

## Permessi Aziende

In OFN i Permessi regolano le relazioni tra le aziende che hanno un profilo: fornitori e distributori. E' necessario impostare queste regole prima che un'azienda \(con un Profilo Produttore - Semplice profilo, Negozio o Hub\) possa diventare fornitrice di un'altra \(Profilo Hub\). Un permesso è assegnato da un'azienda ad un'altra per accedere o modificare un profilo o i relativi prodotti. Questa pagina spiega i diversi tipi di "permessi" e come fare ad assegnarli. 

Per accedere ai permessi della tua azienda: 

![](../../.gitbook/assets/permissions.gif)

Infine, questo argomento può essere considerato da due punti di vista: 

* [un Hub](enterprise-to-enterprise-permissions-e2es.md#hub-perspective) \(il distributore\)
* [un Produttore](enterprise-to-enterprise-permissions-e2es.md#producers-perspective) \(il fornitore\)

## I quattro Permessi

Ci sono 4 diversi tipi di Permessi aziendali, che si possono combinare in vari modi per dare alle aziende più o meno diritti.

![](../../.gitbook/assets/e2emenu2.jpg)

**Permesso di aggiungere prodotti ai cicli di richieste**: il fornitore \(produttore\) permette al distributore \(Hub\) di aggiungere i propri prodotti ai suoi cicli di richieste. Quindi i prodotti del fornitore potranno essere visualizzati nella vetrina del distributore.

**Permesso di gestire i prodotti**: il fornitore autorizza un'altra azienda registrata su OFN \(tipicamente un Hub\) a creare, modificare ed eliminare i prodotti direttamente sul proprio catalogo aziendale.

{% hint style="danger" %}
Questo può avere conseguenze su tutti gli hub che il produttore rifornisce attraverso OFN. 
{% endhint %}

> _Per esempio, se il contadino Giovanni fornisce la propra frutta all'Hub A e B, ma assegna ad A il permesso di gestire i propri prodotti, allora se l'Hub A modifica il prezzo della frutta di Giovanni, questo prezzo cambierà anche nella vetrina dell'Hub B \(a meno di impostazioni di inventario personalizzate\)._

**Permesso di modificare il profilo:** un'azienda permette ad un'altra di modificare i dettagli del proprio  [Profilo Aziendale](./) \(contatti, indirizzo, descrizione...\)

**Permesso di aggiungere prodotti all'inventario**: il fornitore \(produttore\) autorizza il distributore \(hub\) ad aggiungere i propri prodotti al suo [Inventario](../products-1/inventory-tool.md).

{% hint style="info" %}
Se un produttore rifornisce più hub con i propri prodotti, suggeriamo che utilizzi quest'ultimo permesso, per consentire a ciascun hub di gestire i prezzi e le disponibilità dei prodotti autonomamente,dal proprio inventario. Gli Hub dovranno modificare le proprie [Impostazioni inventario](enterprise-settings.md#inventory-settings).
{% endhint %}

## Garantire e gestire Permessi

Per modificare, aggiungere o eliminare permessi, accedi al pannello di controllo e poi clicca su "Aziende" nel menu blu e su "Permessi nel sottomenù verde.

![](../../.gitbook/assets/e2emenu.jpg)

Per assegnare permessi:

* Seleziona la tua azienda dalla prima tendina a sinistra \(sei un produttore che rifornisce altri soggetti\) 
* Seleziona il nome dell'azienda \(hub\) che intendi rifornire dalla tendina di destra.
* Seleziona i permessi che indendi assegnare all'hub che stai autorizzando. Per garantirgli tutti i permessi, puoi selezionare "tutti". 
* Clicca su "Crea". 

 Nota che puoi eliminare o modificare questi permessi in qualsiasi momento. 

{% hint style="warning" %}
Solo gli utenti presenti nella lista dei [Referenti](enterprise-settings.md#users) di un'azienda possono modificare i suoi permessi. 
{% endhint %}

Se hai bisogni che un'altra azienda ti dia i permessi, contattala direttamente. Non c'è una funzionalità per farlo da sistema. 

## Permessi generati automaticamente

Quando un utente è il referente principale di varie aziende sulla piattaforma, [i 4 permessi ](enterprise-to-enterprise-permissions-e2es.md#the-four-permissions)sono generati automaticamente tra le aziende che gestisce. Questo non avviene se le aziende sono gestite da utenti diversi.

## La prospettiva dell'Hub

Gli scenari seguenti mostrano i permessi azienda-azienda di cui potresti aver bisogno per il tuo hub.

> **Ho** [**creato i Profili Produttore di ciascuno dei miei fornitori.** ](create-or-connect-with-your-supplying-producers.md#supplier-does-not-have-an-ofn-profile)**Quali permessi ho bisogno di impostare prima di poter vendere i loro prodotti nel mio negozio?**

Il sistema è configurato in modo da _assegnare automaticamente i permessi corretti_ agli hub che creano i profili dei propri fornitori. Non avrai dunque bisogno di ulteriori impostazioni. 

> **I miei** [**fornitori hanno già un profilo registrato su OFN**](create-or-connect-with-your-supplying-producers.md#supplyingproducer)**. Vorrei aggiungere i loro prodotti al mio negozio.**

Devi contattare i tuoi fornitori di persona. I loro contatti \(numero di telefono, mail e indirizzo\) sono indicati nel loro profilo OFN.  

Se vuoi solo **mostrare i loro prodotti** nella tua vetrina e non intendi aiutarli a gestire il resto del loro profilo OFN, allora richiedi loro di assegnarti i permessi di _**aggiungere al ciclo di richieste**_ e di _**aggiungere all'inventario**_.  _****_

Se il fornitore volesse che tu, in quanto gestore di un hub, lo aiutassi ad organizzare il suo profilo OFN, potrebbe concederti tutti e 4 i permessi. Allora saresti abilitato anche a modificare il loro profilo e i loro prodotti.

> **Il mio Hub distribuisce attraverso altri gruppi di acquisto \(negozi o hub\). Di quali permessi avrà bisogno ciascun gruppo sa parte del mio hub e dei miei fornitori?**

{% hint style="warning" %}
Questo è un esempio per i casi in cui l'Hub che coordina un ciclo d'ordine differisce dall'azienda dove i consumatori recuperano la proria spesa. 

_Se l'Hub A coordina un ciclo d'ordine a cui partecipa anche l'Hub B , allora il ciclo d'ordine sarà visibile nella vetrina dell'Hub B ._
{% endhint %}

L'Hub B dovrà concedere all'Hub A, coordinatore del ciclo di richieste, il permesso di _aggiungere al ciclo di richieste_ \(e, idealmente, anche quello di _aggiungere all'inventario_\).

I Produttori che forniscono all'Hub A prodotti che devono poter essere venduti anche tramite l'Hub B devono concedere sia all'Hub A che all'Hub B il permesso  di _aggiungere al ciclo di richieste_ \(e, idealmente, anche quello di _aggiungere all'inventario_\).

## La prospettiva del produttore

Quando un produttore vuole iniziare a vendere i propri prodotti tramite altre aziende \(hub o negozi\) deve impostare i corretti permessi azienda-azienda. Ci sono diversi livelli di permessi che un produttore può concedere, a seconda di quanto potere vuole dare al referente dell'hub nella gestione dei propri prodotti e del proprio profilo\(vedi [qui in alto](enterprise-to-enterprise-permissions-e2es.md#the-four-permissions)\).

Questi esempi mostrano alcuni scenari comuni.

> **Sono un produttore vorrei che un Hub potesse immagazzinare e vendere i miei prodotti.**

**Fondamentale:** Per permettere ad un Hub di aggiungere i tuoi prodotti alla sua vetrina, devi concedergli il permesso di _aggiungere al ciclo di richieste_. 

**Opzionale:** Potresti anche dare all'hub i permessi di _gestire i tuoi prodotti_, _modificare il tuo profilo_ o _aggiungere all'inventario_. 

> **Un hub che rifornisco distribuisce attraverso altri hub.**

Dovrai concedere almeno il permesso di _aggiungere al ciclo di richieste_ a tutti gli hub coinvolti nella distribuzione, sia all'hub che rifornisci direttamente, sia agli altri hub attraveso cui avviene nei fatti la distribuzione.

> **Sono un Produttore con profilo Negozio, rifornisco un Hub, ma allo stesso tempo vendo i miei prodotti attraverso il mio proprio Negozio su OFN. L'Hub vorrebbe gestire le disponibilità e i prezzi dei miei prodotti. Anche io vorrei gestire le disponibilità ed i prezzi dei miei prodotti.**

Questo caso può essere risolto garantendo all'hub il permesso di _aggiungere all'inventario_ e quello di _aggiungere al ciclo di richieste_. 

Questo permette all'hub di creare un proprio inventario con i tuoi prodotti, impostando autonomamente disponibilità e prezzi, che saranno mostrati nella vetrina dell'HUb. La tua vetrina continuerà così a mostrare invece le disponibilità e i prezzi che imposti tu nel tuo profilo. 

