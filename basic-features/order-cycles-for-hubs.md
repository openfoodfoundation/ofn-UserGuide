# Cicles de comandes (per a grups)

_\*No ets un grup sinó una productora? Ves a_ [_Cicles de comanda (per a productores)_](order-cycles-for-producers.md)_._

Obrireu les vostres botigues creant un cicle de comanda. Quan feu un cicle de comandes seleccionareu quan la botiga està oberta (des de i fins quan), quins productes hi apareixeran i quants recàrrecs o despeses s’hi s'aplicaran.

**Per què els cicles de comandes?** És possible que alguns grups desitgin tenir una botiga en línia oberta permanentment i que preparin les comandes d'una en una, a mesura que es rebin. Tanmateix, molts grups o xarxes operen amb un sistema periòdic de comandes que els permet preparar-les conjuntament, fent que les seves activitats d'empaquetatge i distribució siguin més eficients. Utilitzarem un exemple per il·lustrar una estructura d’un cicle periòdic comú:

**Exemple de cicle de comandes**

Per exemple, cada dilluns al matí, un grup obre la seva botiga i incorpora els seus productes segons la disponibilitat dels seus proveïdors i del seu estoc per a la setmana. A partir d'aquesta informació, crearan un cicle de comandes el dilluns a la tarda i obriran la seva botiga. Les consumidores poden fer comandes a la seva botiga fins que el cicle de comandes es tanqui el dimecres a la mitjanit. El dijous totes les comandes es podran empaquetar o distribuir a les cistelles i es preparen per lliurar el divendres. La següent setmana començarà de nou el cicle amb la creació d'un nou cicle de comandes. En estructurar els cicles de comandes d'aquesta manera i tractar comandes a granel o en grup, els grups poden fer que les seves tasques de repartiment, classificació, empaquetatge o transport siguin molt més eficients que si processen les comandes de forma individual a mesura que es es reben.

### Accediu als cicles de comandes

Podeu crear un cicle de comandes i veure els cicles de comanda anteriors fent clic a ‘**Gestiona los ciclos de pedido**’ al tauler d’administració:

![](../.gitbook/assets/order_cycle.png)

O des del menú horitzontal que hi ha a la part superior de la pàgina:

![Accediu als cicles de comandes](../.gitbook/assets/access_order_cycle.png)

### Creeu un nou cicle de comanda

A continuació es mostren els primers passos en la creació d'un cicle de comandes.

\*Recordeu, no podeu crear un cicle de comandes fins que hàgiu configurat els mètodes de pagament i enviament.

![Seleccioneu el coordinador del cicle de comandes](../.gitbook/assets/set_coordinator.png)

Seleccioneu el coordinador del cicle de comandes. El grup que que coordina un cicle de comandes té plens poders i permisos per editar i gestionar-lo. Altres grups que participin en el cicle de comandes (com ara proveïdors o distribuïdors) han restringit les capacitats per editar un cicle de comandes. Un cop seleccionat el coordinador, el següent cicle de comandes es restringirà d’acord amb qui ha concedit permís a aquest coordinador per afegir-los a un cicle de comanda (P-OC).

**Nom (**_**requerit**_**):** doneu al vostre cicle de comanda un nom que us resulti significatiu. Recomanem que seguiu un patró sistemàtic, per exemple, GrupLaCistella\_Setmana3\_2018. També us recomanem que inclogueu el nom del grup al nom del cicle de comanda, de manera que el suport de de Katuma pugui identificar els vostres cicles si necessiteu ajuda.

**Comandes obertes:** aquesta és la data en què la vostra botiga estarà oberta a Katuma i començarà a acceptar comandes.

**Comandes tancades:** aquesta és la data en què es tanca la vostra botiga a Katuma i deixeu d'acceptar comandes. Si teniu previst un cicle de comandes que estigui obert contínuament, seleccioneu una data de tancament que sigui bastant avançada en el temps.

**Afegiu una comissió de l’organització:** com a grup, és probable que els coordinadors del cicle sigueu vosaltres. Aquí podeu aplicar una comissió per a l’organització que actua com a marge. La comissió es calcula d'acord amb la calculadora seleccionada a Comissions de l’organització. Només podeu aplicar una comissió que s'hagi creat prèviament.

![Camps d'un nou cicle de comanda](../.gitbook/assets/new_order_cycle.png)

#### Entrant: seleccionar productora i productes

La secció d'entrada és on podeu seleccionar els productors i els seus productes que estaran disponibles en aquest cicle de comandes. Al menú desplegable veureu totes les productores que us han concedit permís per afegir els seus productes al vostre cicle de comandes (vegeu la secció _Relacions amb productores_ per obtenir més informació). Després de seleccionar un proveïdor i fer clic a ‘**Agregar proveïdor**’, tots els productes associats amb aquest proveïdor estaran visibles. Comproveu els productes que voleu afegir a la botiga o feu clic a '**Seleccionar tots**'.

{% hint style="info" %}
Els productes que tenen un valor ‘disponibilitat' de zero (sense existències disponibles) encara seran visibles, així que ves amb compte de comprovar que hi ha un inventari adequat per als productes seleccionats.
{% endhint %}

![Entrant](../.gitbook/assets/incoming.png)

Els camps **Detalls de recepció** són opcionals. Si voleu utilitzar el botó ‘**Notificar a les productores**’, per enviar comandes a les productores, haureu d'escriure aquí les instruccions de recepció d’estic. (més informació a la secció ‘Notificar a les productores’ al final d'aquesta pàgina).

El botó ‘**Afegeix tarifa**’ és on podeu aplicar un recàrrec d'organització pertanyent a aquest proveïdor. Seleccioneu el nom de l'organització al primer quadre desplegable i, a continuació, feu clic al nom del recàrrec al segon quadre desplegable.

Aquest recàrrec s'aplicarà a tots els productes que es comprin del productor seleccionat. El recàrrec es calcula d'acord amb la calculadora de recàrrecs que es va seleccionar quan es va crear la Comissions de l’organització.

![Aplica recàrrecs d'organització al proveïdor entrant](https://openfoodnetwork.org/wp-content/uploads/2015/05/Enterprise-Fee.png)

#### Sortint: seleccioneu distribuïdor

El(s) distribuïdor(s) seleccionat(s) a la secció sortint, tindrà una botiga obert d'aquest cicle de comanda. En models de grup senzills, només hi ha un distribuïdor, el propi grup. Així que seleccioneu el grup al menú desplegable i, a continuació, seleccioneu tots els productes que haurien de ser visibles a la botiga en línia durant aquest cicle de comandes. Els grups o xarxes més complexos podrien tenir grups de compra, en aquest cas cadascun és seleccionat com a distribuïdor i, per tant, tindrà la seva pròpia botiga creada. A continuació, teniu la capacitat de seleccionar productes específics que estaran disponibles a cada botiga de grups de compra.

![Secció sortint](../.gitbook/assets/outgoing.png)

La columna d'**etiquetes** és on podeu etiquetar els cicles de comanda per personalitzar si són visibles o invisibles per a determinats clients.

El quadre **‘Llest per a (és a dir, Data / Hora)’ (**_**requerit**_**):** indica el consumidor quan la seva comanda estarà preparada per a la seva recollida o lliurament. Si el vostre cicle de comanda és permanent i atén les comandes de manera individual i no en grup, hauríeu d'introduir un missatge semblant a "Dos dies després de la recepció de la comanda", per exemple. L'exemple següent mostra com es mostra el 'divendres 9' en una botiga:

![Quadre llest per a](https://openfoodnetwork.org/wp-content/uploads/2015/05/Ready-for.png)

La nota també es mostra mentre confirma la comanda, quan la consumidora selecciona el mètode d'enviament (vegeu més avall) i s'inclou en el correu electrònic de confirmació de comanda.

![Ready for info in email](https://openfoodnetwork.org/wp-content/uploads/2015/05/shipping-info.png)

El missatge **Instruccions de recollida** s'inclourà al correu electrònic de confirmació de comanda de la consumidora, a sota del missatge que correspon al mètode d'enviament escollit (vegeu més avall). Aquesta nota està dissenyada per ser visible només per als clients, de manera que podeu incloure informació més sensible, com ara adreces o números de telèfon, etc. Consulteu a continuació un exemple del correu electrònic de confirmació de comanda.

![collection details message](https://openfoodnetwork.org/wp-content/uploads/2015/05/Collection-details.png)

**Afegiu comissió:** de nou, es pot assignar una comissió d’organització creada anteriorment es pot afegir a aquest distribuïdor.

#### Obriu la botiga

Feu clic a ‘**Crea**’ per desar aquest cicle de comandes.

{% hint style="info" %}
Quan creeu un cicle de comandes i les dates d'obertura i de tancament en el present o futur, es podrà consultar. Si no esteu preparats per obrir la botiga, poseu temporalment les dates d'obertura i de tancament en el passat (això es pot editar quan estigui llesta per obrir).
{% endhint %}

Per als cicles de comandes periòdics i repetitius, podeu copiar un cicle de comandes existent i canviar les dates per fer el procés més ràpid. Vegeu la imatge.

![dupliqueu un cicle de comandes](https://openfoodnetwork.org/wp-content/uploads/2015/05/copy-order-cycle.png)

{% hint style="info" %}
Pot ser temptador utilitzar sempre el mateix cicle de comandes i simplement editar les dates cada vegada que el torneu a obrir. No obstant això, és millor crear un nou cicle de comanda, o duplicar i editar un cicle cada vegada. Si sempre feu servir el mateix cicle de comandes, us trobareu que no es poden filtrar els vostres informes. Això pot limitar amb quina eficàcia podeu utilitzar els informes de Katuma.
{% endhint %}

Els cicles de comanda es mostraran de color verd quan estiguin actius, grocs quan es programen per a una data futura i grisos quan hagin tancat. Quan un cicle està tancat des de fa més d'un mes ja no es mostra en aquesta llista. Per veure tots els cicles del vostre passat, feu clic a "mostrar més" a la part superior de la llista.

**Botó ‘Notificar a la productora’**

Algunes organitzacions utilitzen aquesta eina com una manera de notificar als seus proveïdors quins productes s'han demanat, en quines quantitats i també per donar-los instruccions de recepció. En fer clic en aquest botó s'enviarà un correu electrònic a l’adreça de contacte del perfil de la productora. S’enviarà a totes les productores incloses en aquest cicle de comandes i sumarà totes les comandes incloses en aquest cicle de comandes:

Benvolgut \<nom de la productora>,

Tenim totes les comandes per a la proper cicle.

Instruccions de recollida / lliurament d'accions: \<Instruccions de recepció>.\


**Resum de comandes**

Aquí teniu un resum de les comandes dels vostres productes:

\<Comandes totals de productes en aquest cicle de comandes (exemple a continuació)>

\- El Pomer Fruites i Verdures (1,5 kg) (Quant: 1) @ 3,60€ = 4,90€

\- Productor de carn - Embotits (100 g) (Quant: 3) @ 2,50€ = 2,50€

Gràcies,\
\<Nom del grup, adreça, número de telèfon, correu electrònic>

### Funcionalitats avançades:

Funcionalitats avançades relacionades:

* L'eina d'_Inventari_ permet a una botiga "anul·lar" el preu inherent i el nivell d'existències d'un producte. Podeu utilitzar aquesta eina si voleu fer un seguiment dels nivells d'existències separadament per a dues botigues o tenir preus diferents per al mateix producte en diferents botigues.
* Creació de cicles de comanda "only display"
* Permisos en els cicles de comanda de múltiples organitzacions

\
