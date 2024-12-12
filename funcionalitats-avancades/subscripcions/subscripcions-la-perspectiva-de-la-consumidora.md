# Subscripcions - la perspectiva de la consumidora

Aquesta pàgina detalla què pot esperar una consumidora d'una subscripció. També destaca algunes coses de les quals han de ser conscients les botigues que ofereixen subscripcions.

## Registrar-se a Katuma

Les consumidores necessiten tenir un compte a Katuma abans que els pugueu configurar comandes de subscripció.

Per registrar-se poden anar a [https://app.katuma.org/register](https://app.katuma.org/register).

Només necessiten el seu correu electrònic i crear una contrasenya.

Després de registrar-se rebran un correu electrònic de confirmació. Una vegada han fet clic a l'enllaç que confirma el nou compte, podran iniciar sessió.

## Desar dades de la targeta de crèdit i autoritzar els càrrecs

{% hint style="info" %}
Aquest cas només serà possible sempre que la botiga tingui el pagament amb targeta de crèdit entre els seus mètodes de pagament.
{% endhint %}

Les consumidores que vulguin pagar les seves comandes de subscripció via càrrecs automatitzats a les seves targetes de crèdit necessiten a) desar la targeta que prefereixen al seu compte de Katuma i b) permetre que la botiga carregui els imports de les comandes a la targeta. Només després que hagin fet això la botiga podrà configurar-los una subscripció amb càrrecs a la seva targeta de crèdit.

### a) Desar les dades de la targeta de crèdit al compte de la consumidora

La consumidora pot desar una o més targetes en el seu compte, a la taula de **targetes de crèdit**.

![](<../../.gitbook/assets/imatge (83).png>)

La targeta que es determina com a 'predeterminada' o per defecte serà la targeta en la qual es carregarà automàticament per Stripe si té una subscripció amb Stripe com a mètode de pagament escollit. Si cap se selecciona com a predeterminada no es processaran els seus pagaments amb targeta de crèdit.

Si les vostres consumidores desen targeta de crèdit al seu compte, també podran seleccionar ràpidament en qualsevol botiga quan facin una compra i confirmin la seva comanda.

![](<../../.gitbook/assets/imatge (86).png>)

### b) Autoritzar una botiga a carregar l'import de les comandes de  subscripcions a la targeta de crèdit predeterminada

A més de desar una targeta de crèdit al seu compte, la consumidora necessita autoritzar la vostra botiga per carregar-li els imports a la seva targeta de crèdit predeterminada.

**Haureu d'afegir les vostres consumidores a la** [**Llista de Consumidores** ](https://guia.katuma.org/funcionalitats-avancades/configuracio-de-la-botiga/consumidores)**abans de demanar-los que desin els detalls de la seva targeta i us autoritzin a fer els cobraments a la seva targeta.** Si heu afegit una consumidora a la vostra llista, quan creï un compte a Katuma, iniciï sessió i carregui les dades de la seva targeta podrà veure la vostra botiga i podrà atorgar-vos el permís per cobrar-li a la targeta (vegeu l'exemple avall).

![](<../../.gitbook/assets/imatge (28).png>)

Si no l'heu afegit a la vostra llista de consumidores, en el moment en què vagi a desar la seva targeta de crèdit no veurà la vostra botiga per atorgar-vos el permís per cobrar-li (vegeu més avall). Si passa això, necessitareu afegir-la a la vostra llista de consumidores i ella necessitarà tornar a iniciar sessió per donar-vos l'autorització.

![](<../../.gitbook/assets/imatge (70).png>)

Sota hi ha un exemple d'una consumidora que ha donat permisos a una granja perquè li cobri les subscripcions a la targeta.

![](<../../.gitbook/assets/imatge (15).png>)

## Notificacions per correu electrònic

La funcionalitat de les subscripcions inclou una sèrie de correus electrònics generats automàticament que s'envien a les consumidores cada vegada que una de les seves comandes de subscripció s'ha processat.

#### Correu electrònic 1 - quan la comanda s'ha processat

El primer correu electrònic es desencadena en el moment en què obre un cicle de comanda en la programació subscritpa per la consumidora. Aquest correu permet la consumidora saber que la seva comanda de subscripció 'sha obert. Podrà veure-hi quins articles hi ha a la comanda i quina quantitat se li carregarà. El correu electrònic també inclou la seva informació d'enviament i pagament.

![](<../../.gitbook/assets/imatge (3).png>)

#### Modificar la comanda

Si la consumidora pot o no fer canvis en la seva comanda de subscripció dependrà de la [configuració de la botiga](https://guia.katuma.org/basic-features/configuracio-de-lorganitzacio#configuracio-de-la-botiga), dins de la Configuració de l'organització.

Si la botiga **no permet que les seves consumidores canviïn les comandes** el seu correu serà el mateix que el mostrat anteriorment. Si volen cancel·lar la comanda, o fer-hi canvis, necessitaran contactar directament amb la botiga per demanar aquests canvis. _\*\*_

Si la botiga permet a les consumidores canviar les seves comandes, el text de la capsa de text blava serà una mica diferent del correu mostrat anteriorment i hi haurà un enllaç que portarà les consumidores a la seva comanda (vegeu més avall). Actualment les consumidores només poden treure articles de les comandes o canviar les quantitats d'articles existents. Si volen afegir nous articles a la comanda necessitaran realitzar una nova comanda o demanar a la botiga que faci aquest canvi per elles.

![](<../../.gitbook/assets/imatge (66).png>)

#### Productes no disponibles

En el cas que un producte de la subscripció d'una consumidora no estigui disponible a causa d'existència limitada o perquè no està dins del cicle de comanda, seran alertades en el primer correu (exemple a sota).

![](<../../.gitbook/assets/imatge (56).png>)

#### Correu electrònic 2 - Quan tanca el cicle de comanda

El correu electrònic final arriba a la consumidora quan tanca el cicle de comanda. Aquest correu confirma la comanda final, incloent-hi els ajustaments que s'hi han fet.

![](<../../.gitbook/assets/imatge (69).png>)

#### No és possible carregar la targeta de crèdit

Al tancament del cicle de comanda, es carrega a les targetes de crèdit de les consumidores que han escollit pagar a través d'Stripe. Si hi ha algun problema amb el cobrament se'ls alertarà en el segon correu electrònic. Tingueu en compte que en cas d'un càrrec no exitós a la targeta, la comanda consta com a confirmada, però l'import constarà com a saldo adeutat.

Possibles motius per un càrrec fallit:

* Fons insuficient.
* Targeta caducada
* La consumidora ha revocat el permís a la botiga per fer els cobraments al a targeta de crèdit.&#x20;
* La consumidora ha esborrat l'estatus de 'predeterminada' a la seva targeta de crèdit.&#x20;

A la botiga també se l'alertarà de qualsevol càrrec fallit.

## Preguntes freqüents de les consumidores

#### Com puc pausar la meva subscripció?

Si necessiteu pausar la vostra subscripció necessitareu contactar amb la botiga i demanar-los que pausin la vostra subscripció. Estigueu segures de fer-los saber quan voleu començar a parar la subscripció.

#### Els preus de la meva subscripció romandran igual fins i tot si els preus de la botiga s'han modificat?  <a href="#will-the-price-of-my-subscription-remain-the-same-even-if-prices-change-in-the-shop" id="will-the-price-of-my-subscription-remain-the-same-even-if-prices-change-in-the-shop"></a>

No, si els preus dels productes canvien després que vosaltres hagueu configurat una subscripció, se us cobrarà d'acord amb els preus actualitzats.

#### Com puc cancel·lar tota la meva subscripció?  <a href="#how-can-i-cancel-my-whole-subscription" id="how-can-i-cancel-my-whole-subscription"></a>

Si una consumidora vol esborrar la subscripció, necessitarà contactar amb el gestor de la botiga i fer-li saber. Només el gestor de la botiga pot esborrar una subscripció.

#### Com puc cancel·lar només una comanda de la meva subscripció?  <a href="#how-can-i-cancel-a-single-order-of-my-subscription" id="how-can-i-cancel-a-single-order-of-my-subscription"></a>

Si una consumidora vol cancel·lar una comanda individual, hi ha dues maneres de fer-lo depenent de les configuracions de la botiga.

Si la botiga **no permet** a les consumidores fer canvis a les comandes, les consumidores necessitaran contactar amb la botiga i fer-los saber quina comanda volen cancel·lar.

Si la botiga permet a les consumidores fer canvis a les seves comandes, la consumidora pot esperar a rebre el primer correu electrònic de confirmació (quan el cicle de comanda obre) i des d'allà poden editar i/o cancel·lar la seva comanda.
