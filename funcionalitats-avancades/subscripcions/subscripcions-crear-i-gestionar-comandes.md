# Subscripcions - crear i gestionar comandes

Aquesta pàgina descriu com les botigues poden configurar subscripcions úniques per a consumidores individuals, incloent quins articles hi ha a la subscripció, quin programació s'apliquen i com pausar i editar una subscripció des del seu punt de vista.

{% hint style="info" %}
En aquesta primera versió de la funcionalitat de les subscripcions, les botigues hauran de configurar subscripcions en nom de les seves consumidores. No hi ha cap lloc on les consumidores puguin configurar la seva pròpia botiga.
{% endhint %}

**Llista de tasques per fer abans de crear subscripcions per a les vostres consumidores:**

* Habilitar subscripcions a la [Configuració de l'organització](https://guia.katuma.org/basic-features/configuracio-de-lorganitzacio).
* Configurar [mètodes de pagament i enviament](https://guia.katuma.org/basic-features/metodes-denviament).
* Haver contactar amb les consumidores per tenir [les dades necessàries](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-configuracio#3-gather-information-from-your-customers).
* Tenir afegits les consumidores que volen subscripció a la vostra [Llista de Consumidores](https://guia.katuma.org/funcionalitats-avancades/configuracio-de-la-botiga/consumidores).
* Haver contactar amb les consumidores per demanar-los que [registrin un compte a Katuma](https://guia.katuma.org/basic-features/register-and-create-your-profile) i en cas que vulguin pagar amb targeta de crèdit (i vosaltres tingueu disponible el mètode de pagament per Stripe) demanar-los que desin les dades de la seva targeta de crèdit i us autoritzin a carregar-los l'import de les subscripcions.
* Crear com a mínim una[ programació](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-configuracio#5-programacions)

## 6) Crear subscripcions

Feu clic a **Comandes** al menú horitzontal blau i després seleccioneu **Subscripcions** al submenú verd.

Feu clic a **+Nova Subscripció** per configurar una comanda recurrent per a les vostres consumidores.

![](<../../.gitbook/assets/imatge (62).png>)

**Consumidora:**

Seleccioneu una consumidora de la llista desplegable.

\* Només podeu crear una subscripció per a una consumidora que sigui a la vostra[ Llista de Consumidores.](https://guia.katuma.org/funcionalitats-avancades/configuracio-de-la-botiga/consumidores)

**Programació:** Seleccioneu la programació, o grup de cicles de comanda, al qual la vostra consumidora vol subscriure's.

{% hint style="info" %}
Heu de crear una programació de cicles de comanda abans de poder crear una subscripció. Podeu trobar les instruccions [aquí](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-configuracio).
{% endhint %}

**Mètode de pagament:** Seleccioneu el mètode de pagament que la consumidora prefereixi. Aquest haurà de ser o bé la passarel·la de pagament Stripe o bé un mètode de pagament manual com el pagament en efectiu. No es pot utilitzar Paypal per a les subscripcions.

**Mètode d'enviament:** Seleccioneu el mètode d'enviament preferit per la consumidora.

**Comença a:** Aquesta és la data en la qual es començarà a generar la subscripció. Si la data agafa enmig d'un cicle de comandes obert en la seva programació hi haurà ja una comanda generada per aquell cicle de comanda. Si no, la primera comanda aplicarà al següent cicle de comanda que obri dins d'aquesta programació.

**Acaba a:** Després d'aquesta data ja no es generaran les comandes recurrents de la consumidora. Aquest camp és opcional, si es deixa en blanc la comanda es continuara generant de manera indefinida.

Com interactua exactament la data de finalització de la subscripció amb les dates dels cicles de comanda? Si la data de finalització de la subscripció de la consumidora és posterior a la data d'obertura del cicle de comandes a la programació però abans del tancament del cicle, no es generarà la comanda. L'última comanda es generarà només per a l'últim cicle de comanda que tanqui abans de la data de finalització de la subscripció.

**Adreça:** Ompliu els detalls d'enviament i facturació de la consumidora. Si hi ha desats detalls d'enviament i facturació a la vostra pàgina de consumidores, aquesta informació es carregarà automàticament.

![](<../../.gitbook/assets/imatge (73).png>)

**Afegir productes**

Podeu afegir qualsevol producte que hi hagi en els Cicles de Comanda futurs inclosos en la programació. No podeu afegir productes a una subscripció si no estaran disponibles en cap cicle de comanda dins la programació al qual la consumidora s'està subscrivint.

![](<../../.gitbook/assets/imatge (76).png>)

#### Resum

{% hint style="info" %}
Vigileu! Si teniu un cicle de comanda que està obert i assignat a una programació, el moment en què creeu una subscripció per a una consumidora en aquesta programació, es generarà una comanda, i s'enviarà un correu electrònic de confirmació. Si només esteu configurant les subscripcions i no voleu que s'iniciï cap comanda, assegureu-vos que no teniu un cicle de comandes obert. Vegeu [8) Com es processen les subscripcions](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-crear-i-gestionar-comandes#8-com-es-processen-les-subscripcions) per a més detalls.
{% endhint %}

**Què passa si el preu d'un producte canvia després que s'hagi fet una subscripció?**

Els preus dels articles dins de la subscripció s'actualitzaran i la consumidora se li cobrarà d'acord amb aquestes actualitzacions.

**Què passa si un producte demanat en una subscripció no està disponible en un cicle de comanda?**

Quan un article d'una subscripció no està disponible en un cicle de comanda s'alertarà la consumidora en els correus electrònics de confirmació.

## 7) Editar una comanda d'una subscripció

### Editar la subscripció base

Dins la pàgina de **Subscripcions**, feu clic al botó **editar** al costat de la subscripció que voleu editar.

![](<../../.gitbook/assets/imatge (52).png>)

Des d'aquí podeu editar quins productes hi ha a la subscripció, el mètode preferit d'enviament i pagament, les dates d'inici i finalització i els detalls de la consumidora.

{% hint style="info" %}
No podeu canviar una programació d'una subscripció. Per contra, la subscripció s'haurà de crear novament a la nova programació que preferiu.
{% endhint %}

### Editar una comanda específica

Si voleu canviar una sola comanda en una subscripció podeu fer clic al número a la columna de les comandes d eles consumidores.

Això us mostrarà totes les comandes futures en la programació i, a continuació, podreu editar una comanda específica.

![](<../../.gitbook/assets/imatge (63).png>)

### Esborrar una subscripció

Des de la pàgina de **Subscripcions**, feu clic al botó de la **creu** del costat de la subscripció que vulgueu esborrar. Això previndrà que no es generi cap nova comanda i esborrarà la subscripció de manera permanent.

![](<../../.gitbook/assets/imatge (17).png>)

{% hint style="info" %}
Si esborreu una subscripció mentre hi ha un cicle de comandes obert se us demanarà si voleu mantenir la comanda que la consumidora té oberta o si vol esborrar la comanda actual.
{% endhint %}

### Pausar una subscripció

Des de la pàgina de **Subscripcions**, feu clic al botó de **pausa** al costat de la subscripció que vulgueu pausar. Això previndrà que es generin futures comandes fins que s'activi novament la subscripció. Per activar novament les subscripcions (desactivar la pausa) feu clic al botó de **play**.

{% hint style="info" %}
Si pauseu les subscripcions mentre un cicle de comanda encara està obert, se us demanarà si voleu mantenir la comanda actual o no.
{% endhint %}

{% hint style="info" %}
Si elimineu la pausa d'una subscripció (és a dir, la torneu a activar) mentre un cicle de comanda és obert, es generarà una comanda per a la consumidora si està subscrita a aquella programació.
{% endhint %}

![](<../../.gitbook/assets/imatge (79).png>)

## 8) Com es processen les subscripcions

Una vegada, doncs, que les subscripcions estan configurades, com es processen cada vegada que obre i tanca un cicle de comandes?

**1) Obre un cicle de comandes que està dins d'una programació:**

* Això provoca la creació de comandes de subscripció per a les consumidores que estan subscrites a la programació.

{% hint style="info" %}
**VIGILEU! En el moment que obriu un cicle de comanda que estigui inclòs dins d'una programació, es crearà una comanda per a cadascun dels subscriptors i se'ls enviarà un correu electrònic, així que assegureu-vos d'estar preparat. Comproveu dos cops que heu configurat correctament el cicle de comandes i heu actualitzat la disponibilitat del vostre producte abans d'obrir un cicle de comandes.**
{% endhint %}

* El nivell d'existències es descomptarà en aquest moment.
* Cada consumidora amb una comanda de subscripció rebrà un correu electrònic explicant que la seva comanda s'ha preparat.
* S'enviarà un correu electrònic a l'adreça de correu electrònic que tingueu configurada per la botiga resumint quantes subscripcions hi ha, i quantes incidències (per exemple: estoc insuficient).
* Durant el temps en què el cicle de comanda està obert les consumidores poden editar la seva comanda (depenent de les vostres [preferències de la botiga](https://guia.katuma.org/basic-features/configuracio-de-lorganitzacio)).&#x20;

{% hint style="info" %}
Tingueu en compte que si creeu una subscripció mentre hi ha un cicle de comanda obert en una programació es generarà automàticament una comanda per a la/les subscriptora/es.
{% endhint %}

**2) El cicle de comanda tanca**

* Quan el cicle de comanda tanca es confirmaran les comandes de subscripció.
* Si les consumidores paguen per Stripe, se'ls carregarà en aquest moment l'import de la comanda de subscripció.
* La consumidora rebrà un correu electrònic confirmant que la seva comanda s'ha completat.
* El correu electrònic de notificació de la botiga rebrà un correu electrònic confirmant quantes comandes de subscripció s'han processat. També mencionarà els errors com les targetes de crèdit a les quals no s'ha pogut carregar l'import.

### Planificar subscripcions futures

Hi ha dues maneres per planificar les obertures i tancaments de cicles de comanda en les vostres programacions.

Segons quina opció utilitzeu, recordeu que la freqüència que tinguin els vostres cicles de comanda en una programació dictarà cada quant es produeix una comanda de subscripció. Per exemple, si creeu un cicle de comanda cada setmana que obre els dilluns, les vostres consumidores tindran subscripció setmanal.

**Opció manual**

Podeu crear cicles de comanda a les vostres programacions d'un en un. Això funciona de la següent manera: quan esteu preparats per obrir un cicle de comanda comprovareu que heu actualitzat tot el que cal fora dels cicles de comanda, com la disponibilitat dels productes, qualsevol descripció de mètodes d'enviament, etcètera.

A continuació, quan estigueu preparats, creeu el cicle de comanda, ja sigui duplicant un cicle anterior ja existent o creant-ne un de nou. Afegireu el llistat de productes disponibles i comprovareu els camps de text (com la data en el camp 'llest per'). Comproveu també que heu actualitzat la disponibilitat dels productes. Ara ja podeu crear el cicle de comanda.

**Opció automàtica**

Podeu crear cicles de comanda futurs per avançat i configurar les seves dates d'obertura i tancament que corresponguin amb les dates de les subscripcions. Per fer això podeu crear sèries de cicles de comanda a través de la duplicació, i només ajustant les dates d'obertura i tancament, i els camps de text si és necessari (com la data en el camp 'llest per').

Després, a mesura que passi el temps, els vostres cicles de comanda s'aniran obrint i tancat automàticament, provocant la creació automàtica de les vostres comandes de subscripció.

Tan sols us heu d'assegurar abans de les dates d'obertura de cada cicle de comanda de revisar la disponibilitat dels productes, etc.

\*\*\*\*

\*\*\*\*
