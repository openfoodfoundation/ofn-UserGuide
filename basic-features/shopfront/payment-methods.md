# Metodi di Pagamento

{% hint style="danger" %}
**Devi** creare almeno un metodo di pagamento prima di poter aprire il tuo negozio. 
{% endhint %}

Prima di proseguire con la lettura, puoi dare un'occhiata a questa breve presentazione di come impostare il tuo primo metodo di pagamento:

![](../../.gitbook/assets/paymentmethod.gif)

## Impostare un Metodo di Pagamento

* Puoi accedere alla pagina "Metodi di Pagamento", cliccando su **Aziende** nel menù azzurro orizzontale e poi su **Impostazioni** vicino al nome della tua azienda. La voce **Metodi di Pagamento** si trova nel menù laterale a sinistra. 
* Clicca su **Crea un nuovo metodo di pagamento +**. Sarai indirizzato ad una pagina come questa:

![](../../.gitbook/assets/paymentmethods2.jpg)

* Seleziona la tua azienda nel riquadro a destra "Hub". Questo indica a quali aziende verrà applicato il metodo di pagamento che stai per creare. Puoi selezionare più di un'azienda.
* **Nome:** Scegli un nome per questo metodo di pagamento \(es. "Pagamento in contanti" o "Bonifico", ecc.\) Questo nome sarà visualizzato nella pagina di conferma della gentile richiesta e nella mail che riceveranno i clienti. 

![](../../.gitbook/assets/paymentmethod2.jpg)

* **Descrizione:** inserisci maggiori dettagli circa il metodo di pagamento. Per esempio, per un pagamento via bonifico, inserisci i dati bancari per effettuarlo. La descrizione sarà visibile in un riquadro grigio che appare quando viene selezionato il metodo di pagamento nella pagina di conferma della gentile richiesta, oltre che nella mail di conferma che riceveranno i clienti.
* **Visualizza:** puoi optare per "solo Backoffice" o "Entrambi Checkout e Backoffice"

{% hint style="info" %}
Se vuoi disattivare temporaneamente un metodo di pagamento ma potresti volerlo riattivare in seguito \(ad esempio se per il COVID dovessi temporaneamente non permettere il pagamento in contanti\) allora cambialo in "Solo Backoffice". 
{% endhint %}

{% hint style="warning" %}
Se scegli "Solo Backoffice" per tutti i tuoi metodi di pagamento, otterrai una [Vetrina di sola visualizzazione](display-only-order-cycles.md) per i cicli di richiesta attivi.
{% endhint %}

* **Attivo:** Scegli se il metodo di pagamento sarà visibile e disponibile o no. 
* **Tag:** Usa le regole di tag se vuoi rendere un determinato metodo di pagamento disponibile/non disponibile per determinati consumatori \(per esempio potresti voler permettere solo ai rivenditori di pagare con bonifico bancario e ai consumatori al dettaglio permettere solo il pagamento con carta di credito o PayPal\). Per maggiori informazioni, leggi [qui](customer-management-and-conditional-displays-prices/).
* **Provider**: Seleziona l'opzione adatta al metodo di pagamento che stai creando. Al momento ci sono 5 opzioni: 
  * MasterCard Internet Gateway Service \(MIGS\) 
  * PayPal Express 
  * Stripe
  * Stripe SCA
  * Contanti o altri metodi di pagamento per cui non è richiesta una validazione automatica \(Contanti, bonifico, ecc.\)  

![](../../.gitbook/assets/payment-methods1.jpg)

* **Calcolatore:** Seleziona come desideri applicare eventuali tariffe legate al metodo di pagamento. Nota che le tariffe possono essere impostate a zero. Leggi qui sotto per maggiori informazioni sulle  [Tariffe dei metodi di pagamento](payment-methods.md#fee-calculators). 

Cliccando su "Crea", il metodo di pagamento verrà creato e saranno disponibili nuovi campi per definire le tariffe collegate. Questi campi dipendono dal "Calcolatore" selezionato in precedenza.  

{% hint style="info" %}
Se modifichi il campo "Calcolatore", per poter visualizzare i nuovi campi collegati, dovrai prima salvare le tue modifiche \(Aggiorna"\)
{% endhint %}

## Provider di Pagamenti Integrati con OFN

Qui sotto trovi ulteriori informazioni per i pagamenti con Paypal, MasterCard, Stripe.

{% tabs %}
{% tab title="Paypal" %}
Per impostare un metodo di pagamento, è necessario che tu abbia un account business o commerciale su PayPal. Puoi crearne uno [qui](https://www.paypal.com/au/webapps/mpp/merchant). Una volta creato, puoi impostare l'"accesso API" dentro PayPal, che abiliterà OFN a collegare i consumatori direttamente con il tuo account su PayPal. 

1. Accedi al tuo account PayPal
2. Sotto al nome del tuo account in alto a destra c'è un menù a tendina con "Impostazioni Account"

![](../../.gitbook/assets/paypalmay1.jpg)

3. Seleziona "Aggiorna" in "Accesso API"

![](../../.gitbook/assets/paypalmay2.jpg)

4. Seleziona "Gestisci credenziali API" dalla pagina di personalizzazione dell'esperienza del Checkout. 

![](../../.gitbook/assets/paypalmay3.jpg)

Da qui potrai accedere a username, password e firma delle tue API.

![](../../.gitbook/assets/paypalmay4.jpg)

**In OFN,** assicurati di aver effettuato l'accesso come Profilo Azienda. Vai su un Azienda e crea un Metodo di Pagamento. Seleziona PayPal ed inserisci i dettagli dal sito di PayPal. 

**Server:** Cambia il campo "Server" in "live".

**Accedi:** Digita lo username API.

**Password:** Digita la password API.

**Firma:** Digita la firma API. 

![](../../.gitbook/assets/paypal3.jpg)

**Soluzione:** Determina se un consumatore ha bisogno o no di un account PayPal per effettuare il checkout. 

Digita “Mark” se vuoi che i consumatori abbiano un account PayPal, o "Sole" se possono effettuare il checkout senza avere un account su PayPal \(con carta di credito\).

**Landing Page:** Puoi selezionare quale pagina mostrare ai consumatori quando verranno ridiretti su PayPal.

Digita "login" per indirizzare i consumatori alla pagina di accesso \(se hai selezionato "Mark" precedentemente\). O dicita "Billing" per mostrare ai consumatori il modulo dove inserire i dati della propria carta di credito ed eventualmente registrare un account su PayPal \(se hai selezionato "Sole" precedentemente\).
{% endtab %}

{% tab title="MIGS" %}
 MasterCard Internet Gateway Service \(MIGS\)

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.
{% endtab %}

{% tab title="Stripe" %}
[Stripe](https://stripe.com/au) is an online payment platform similar to Paypal. It will allow you to accept credit card payments from your customers. Stripe is a global platform, but is only available on certain OFN instances. Contact your [local OFN team](https://openfoodnetwork.org/ofn-local/) to see whether it’s available on your OFN.

#### Why use Stripe?

Stripe is simple to setup for shop owners and is reasonably priced. The fees charged by Stripe vary in each country; [Australia](https://stripe.com/au/pricing), [Canada](https://stripe.com/ca/pricing), [France](https://stripe.com/fr/pricing), [UK](https://stripe.com/gb/pricing), [USA](https://stripe.com/us/pricing).

Stripe is also easy for customers to use. Unlike Paypal, when the customer checks out, they don’t need to login with Paypal to place their order, rather they just need to enter their card details and then complete their order.

Stripe is the recommended payment method for shops who wish to use [**subscriptions** ](../subscriptions/)on OFN, as Stripe allows customers to give permission to a shop to automatically bill their credit card for subscription orders. This isn’t offered by Paypal, Pin or MIGS payment platforms.

#### Setup

**Connect with Stripe**

Before you can setup a payment method that uses Stripe, you’ll need to Connect with Stripe. To do this, click on the ‘Connect with Stripe’ button.

![](../../.gitbook/assets/connect-with-stripe.png)

You’ll be taken to a form to fill in your details. If you already have an account with Stripe, you can login, if not, fill in the form to create a Stripe account.

The information you’ll be asked for includes: country, a description of your business, your Business address and ABN, your personal details and your bank account \(where received payments will be deposited\).

**Create a New Payment Method**

Once you’ve connected with Stripe, you can then create a payment method which will work with your connected account.

Treat the **Name**, **Description**, **Active** and **Tags** fields as you would with any payment method.

**Provider:** Select Stripe.

Once you select Stripe, ‘Provider Settings’ will be shown.

**Stripe Account Owner:**

Select the enterprise that has a Stripe account connected.

If you select an enterprise that is not Connected to Stripe \(see above\) , you will get the error shown below. Either click ‘Connect One’ or return to your Payment Methods tab to Connect with Stripe. See instructions above.

![](../../.gitbook/assets/stripe-connect.png)

#### Stripe Payments for Customers

When customers checkout in a shop and pay with a Stripe payment method, they’ll have the options of selecting a tickbox allowing their credit card details to be stored against their account \(if they are logged in\).

Customer can also save a credit card in their Account, or delete saved ones.

![](../../.gitbook/assets/add-card.png)

When the customer next shops with an OFN shop offering Stripe as a payment method, they’ll be able to select from their saved credit cards.

**Viewing and redeeming your payments via Stripe**

When a customer pays for their order with Stripe, the funds \(minus Stripe's fees\) will go to your stripe account. Depending on your setting in Stripe the funds will be automatically transferred to your chosen bank account periodically.

**Taking further payment**

If you need to take additional payment from a customer because they have further balance due,  you can create an invoice in Stripe. The customer will get sent an email asking for them to pay with Credit/Debit card. This won't be communicated to OFN, so you'll need to mark the payment off manually.

![](../../.gitbook/assets/image%20%2831%29.png)
{% endtab %}

{% tab title="Pin Payments" %}
For Pin Payments you only require your API key. You need to set up an account with Pin Payments first, and can get a discount by signing up as an OFN member \([https://pinpayments.com/partners/openfoodnetwork/signup](https://pinpayments.com/partners/openfoodnetwork/signup)\)

**API Key:**Enter your “Live Secret API Key’ here – you can find this in your PinPayments account \(see below\). First from your account, select API Keys. Then once you have generated an API key, copy the ‘Live Secret API Key’ and paste it into the API key field in OFN.

![](../../.gitbook/assets/api-keys.png)

![](../../.gitbook/assets/api-2.png)

**Server:**Type ‘live’ – this is case sensitive.
{% endtab %}
{% endtabs %}

## Tariffe per i Metodi di Pagamento

![](../../.gitbook/assets/fee-calculators.png)

Puoi inserire una tariffa per i metodi di pagamento. Solitamente è utilizzato per attribuire ai consumatori l'eventuale ricarico richiesto dal portale di pagamento. Ad esempio puoi caricaricare sul consumatore che sceglie PayPal come metodo di pagamento la commissione richiesta da PayPal.

{% hint style="danger" %}
Le tariffe per i Metodi di Pagamento NON includono imposte \(IVA\)
{% endhint %}

### Calcolatore Tariffe

**Percentuale fissa:** Questa tariffa è calcolata come percentuale sull'importo totale della gentile richiesta. ****

**Tariffa fissa \(per gentile richiesta\):** Questa tariffa è applicata indistintamente a tutte le gentili richieste, indipendentemente dalla dimensione dell'importo. ****

**Tariffa Flessibile:** Questo tipo di tariffa è particolarmente utile se intendi incoraggiare i consumatori a fare gentili richieste sostanziose: ad esempio il costo del pagamento può essere ridotta a zero quando viene raggiunto un numero minimo di articoli richiesti. 

* Costo Primo Articolo: la tariffa applicata al primo articolo richiesto.
* Costo Articoli successivi: la tariffa applicata agli articoli successivi al primo. 
* ‘Max Articoli’: In numero massimo di articoli a cui verrà applicata la tariffa. Gli articoli acquistati oltre questo numero non saranno considerati nel calcolo della tariffa. 

![](../../.gitbook/assets/paymentflex.jpg)

> Per esempio: Se il "Costo Primo Articolo" è impostato a 0,20€, il "Costo Articoli Aggiuntivi" a 0,10€ e il "Max Articoli" è 3, un consumatore che acquista 5 articoli pagherà una tariffa di 0,40€ \(0,20€ per il primo articolo, 0,10€ per il secondo, 0,10€ per il terzo e 0€ per i due articoli successivi\).

**Tariffa Fissa \(per articolo\):** Questa tariffa viene applicata a tutti gli articoli elencati al "pezzo". Non viene applicata agli articoli venduti a peso o a volume. Dunque un consumatore che acquisti solo prodotti al kg non pagherà alcuna triffa. 

**Tariffa flessibile \(per importo totale\):** Questa tariffa si applica all'_importo monetario totale_ invece che al numero di articoli acquistati \(Tariffa Flessibile qui sopra\) 

* ‘Importo Minimo’: Valore monetario soglia tra la "Tariffa Normale" e la "Tariffa Scontata". 
* 'Tariffa Normale': Tariffa applicata per importi minori dell'"Importo Minimo". 
* ‘Tariffa Scontata": Tariffa applicata per importi maggiori dell'"Importo Minimo". 

![](../../.gitbook/assets/paymentpc.jpg)

{% hint style="info" %}
I portali di pagamento generalmente applicano alle imprese un importo fisso per transazione più una piccola percentuale dell'importo totale. Dunque le tariffe dovute da Hub o Negozi i cui clienti effettuano molti piccoli acquisti saranno maggiori rispetto a quelle applicate a Hub o Negozi i cui clienti facciano un unico acquisto con lo stesso importo totale. 

Le tariffe flessibili applicate ai metodi di pagamento possono essere utili a stimolare acquisti più sostanziosi, per controbilanciare questo squilibrio.
{% endhint %}

## Rimborsi

Gestire eventuali rimborsi dipende dal metodo di pagamento utilizzato in origine dal consumatore per pagare la propria gentile richiesta. [Qui](../orders/refund-payments.md) maggiori dettagli.

