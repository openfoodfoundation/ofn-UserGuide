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

## Abilitare Acquisto di gruppo per un prodotto

Dal pannello di controllo, vai alla voce "**Prodotti**" nel menu blu orizzontale. Clicca sull'icona con carta e penna a destra del prodotto che vuoi modificare: &#x20;

![](../../.gitbook/assets/productedit.jpg)

Seleziona "**Opzioni acquisti di gruppo**" nel menu a destra.&#x20;

![](../../.gitbook/assets/groupbuy.jpg)

Seleziona "**Sì**" sotto "**Acquisto di gruppo?**" per attivare questa funzionalità per il prodotto.&#x20;

La "**Quantità minima per Acquisto di Gruppo**" è la quantità che l'ordine collettivo di gruppo deve raggiungere.&#x20;

{% hint style="warning" %}
Per la quantità minima per l'acquisto di gruppo si considerano le unità già selezionate per la vendita del prodotto. &#x20;

Se il prodotto è venduto a:

* **Peso**: le unità sono i grammi (quindi se il totale collettivo deve essere di 5 kg, inserisci "5000" in questo campo)
* **Volume**: le unità sono i litri (quindi se il totale collettivo deve essere di 10 l, inserisci 10 in questo campo)
* **Pezzi**: es. se le lattughe sono vendute a cespo ma è necessario raggiungere 100 cespi in totale, allora inserisci "100" in questo campo.
{% endhint %}

## Adeguamento degli ordini per creare lotti completi

Sotto Ordini --> [gestione massiva ordini](../orders/view-orders.md#bulk-order-management) puoi vedere e modificare gli ordini per i prodotti con "acquisto di gruppo" per far sì che l'ordine collettivo raggiunga il minimo richiesto.&#x20;

1. Seleziona il ciclo di richieste o l'intervallo di date di tuo interesse.
2. Cerca il prodotto (ad esempio Susine).
3. Assicurati che la colonna "Max" sia visualizzata, di modo che tu possa visualizzare le quantità massime che il consumatore è disposto ad acquistare.
4. Poi, clicca sul valore della colonna **Prodotto: unità** ("Susine" nell'esempio qui sotto), per visualizzare il riquadro (azzurro) con il totale degli ordini per quel prodotto. &#x20;
5. Usando l'informazione nella colonna **Max**, puoi aumentare le quantità ordinate per raggiungere il lotto completo richiesto.&#x20;
6. Clicca "Aggiorna" per salvare le modifiche agli ordini dei consumatori.&#x20;

![](../../.gitbook/assets/bulkorder2.jpg)

**Unità attualmente raggiunte** suddivide le quantità totali ordinate nelle unità dell'acquisto di gruppo. Se questo valore è maggiore di 1, indica che gli ordini attuali raggiungono o eccedono la quantità minima richiesta. Se questo valore è inferiore a 1, significa che gli ordini non raggiungono collettivamente il minimo richiesto. All'aumentare degli ordini individuali, questo valore aumenterà.&#x20;

**Unità massime raggiunte** indica la somma di tutte le quantità MASSIME ordinate dai consumatori diviso la quantità minima per l'acquisto di gruppo. Se questo valore è inferiore a 1, significa che nemmeno la somma delle quantità MASSIME raggiunge la quantità minima richiesta.&#x20;
