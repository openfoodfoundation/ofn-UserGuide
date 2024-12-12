# Importació de productes i inventari

{% hint style="info" %}
AQUESTA FUNCIONALITAT ESTARÀ DISPONIBLE MOLT AVIAT.
{% endhint %}

L'eina d'importació de productes i inventari us permet carregar un arxiu CSV (full de càlcul) per afegir i actualitzar el teu estoc de productes.

L'eina d'importació de productes i inventari es pot trobar fent clic a **Productes** al menú horitzontal blau, i després a **Importació de productes** al menú verd.

La importació de productes es pot utilitzar en relació a [productes](https://guia.katuma.org/basic-features/productes) o[ inventari](https://guia.katuma.org/funcionalitats-avancades/productes/eina-dinventari). Aquí hi ha quatres maneres com podeu utilitzar l'eina:

1. Importar nous productes
2. Actualitzar detalls de productes existents
3. Importar nou inventari
4. Actualitzar detalls de l'inventari existent

En totes els casos el procés implica descarregar-se una plantilla en format CSV, omplir les caselles i pujar novament l'arxiu CSV a Katuma.

#### Camps de producte que no estan inclosos en l'eina d'importació

A la primera versió d'aquesta eina hi ha uns quants camps que no es capturen. Desafortunadament mentrestant aquests camps s'hauran de configurar o actualitzar manualment. Vegeu [productes](https://guia.katuma.org/basic-features/productes) pels detalls.

* Imatge
* Propietats (Tots els productes actualitzats heretaran les propietats del perfil de la productora).&#x20;
* Descripció del producte
* Configuració de la compra grupal

{% hint style="info" %}
Si necessiteu aquesta funcionalitat sisplau feu-ho saber a la vostra instància local d'Open Food Network (info@katuma.org). El teu feedback és benvingut.
{% endhint %}

## 1) Importar Nous Productes

Utilitzeu aquestes instruccions si voleu afegir nous productes a un perfil de productora.

{% hint style="info" %}
Podeu simultàniament pujar nous productes i actualitzar productes ja existents amb un sol arxiu CSV. Les instruccions en aquesta guia estan separades per a més claredat però podeu combinar nous productes i actualitzacions en el mateix full de càlcul.
{% endhint %}

### Prepareu l'arxiu CSV per importar

Primer, descarrega l'arxiu **Plantilla de Llista de Productes CSV** des de la pàgina d'**Importació de Productes** i obre'l amb Excel (o equivalent).

Veuràs que la plantilla et dona tots els encapçalaments de les columnes requerides per aconseguir una importació de productes exitosa. Cada fila és per a un nou producte o variant. Sota hi ha una descripció de com omplir cada columna.

![Mostra dels títols de cada columna de l'arxiu CSV](<../../.gitbook/assets/imatge (39).png>)

{% hint style="info" %}
Aneu amb compte perquè és sensible a les minúscules i les majúscules. Per exemple: has d'utilitzar mL i no ml, o Làctic i no làctic.
{% endhint %}

| Títol de la columna                  | Obligatori? | Descripció                                                                                                                                                                                                                       | Exemple               |
| ------------------------------------ | ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| productora                           | sí          | Aquest és el nom del perfil de la productora a la qual s'assigna aquest producte.                                                                                                                                                | Granja Four Mile Farm |
| SKU (codi de referència de magatzem) | no          | El codi SKU que es dona a aquest producte.                                                                                                                                                                                       | AD001265              |
| nom                                  | sí          | Aquesta columna és per al nom del producte.                                                                                                                                                                                      | Yoghurt               |
| nom\_desplegat                       | no          | Aquest camp aplica si creeu variants de producte (vegeu instruccions més avall). Si no és el vostre cas, deixeu aquest camp en blanc.                                                                                            | Yoghurt de gerds      |
| categoria                            | sí          | A quina categoria pertany aquest producte? Les categories disponibles estan llistades a la Pàgina d'Importació de productes.                                                                                                     | Làctics               |
| unitat                               | sí          | El valor de la unitat de venda en pes, volum o quantitat.                                                                                                                                                                        | 500                   |
| unitat\_de\_mesura                   | potser      | En quina unitat de mesura es ven el producte (g, kg, mL, L)? Si es ven com a element (per exemple: manat / capsa / bossa...) deixeu en blanc.                                                                                    | g                     |
| nom\_de\_element                     | potser      | Si el producte es ven com a element (per exemple: manat / capsa / bossa...) escriu el nom de l'element aquí.                                                                                                                     | Manat                 |
| preu                                 | sí          | El preu del producte. Si el producte té impostos, aquesta camp haurà d'incloure el preu amb impostos.                                                                                                                            | 3.70                  |
| disponible                           | potser      | Si teniu un estoc limitat per al producte, escriviu el nivell d'existències aquí. Si teniu un estoc infinit disponible (sempre en podeu obtenir) escriviu 0 i utilitzeu la columna sota\_demanda.                                | 40                    |
| disponible\_a                        | no          | Deixeu en blanc.                                                                                                                                                                                                                 | ​                     |
| sota\_demanda                        | potser      | Si teniu un estoc infinit disponible per a aquest producte, escriviu 1, si esteu deixant en blanc la columna 'disponible'. Si entreu un número a la columna 'disponible' i 1 a 'sota\_demanda', el producte estarà sota demanda. | 1                     |
| tipus\_enviament                     | no          | Deixeu en blanc.                                                                                                                                                                                                                 | ​                     |
| tipus\_impost                        | sí          | Si el preu del producte inclou IVA com a impost, si no deixa en blanc.                                                                                                                                                           | IVA                   |

#### Com importar variants  <a href="#how-to-import-variants" id="how-to-import-variants"></a>

Les [variants](https://guia.katuma.org/funcionalitats-avancades/productes/variants-de-productes) són productes similars però de sabor, mida o varietats diferents. Pujant-los com a variants en comptes de com a productes individuals, la vostra botiga estarà menys atapeïda i serà més senzilla per a les consumidores navegar-hi.

En el procés d'importació, les variants es distingeixen per les 'unitats' (com llet venuda en 2 variants diferents de tamany) o pel 'nom\_desplegat' (com iogurt venut de molts sabors diferents) i agrupades pel nom del producte genèric del qual pengen (en aquest cas: 'llet' o 'iogurt'). Sempre que el nom del producte sigui el mateix, les files s'importaran com a variants.

L'exemple de sota mostra una bossa de fulles d'enciam que ve en variants 500g i 750g i un iogurt que es ven de diversos sabors.

| nom            | nom\_desplegat | preu | unitat | unitat\_de\_mesura |
| -------------- | -------------- | ---- | ------ | ------------------ |
| Bossa d'enciam | ​              | 3.50 | 500    | g                  |
| Bossa d'enciam | ​              | 5.50 | 750    | g                  |
| Yoghurt        | Banana         | 4    | 500    | g                  |
| Yoghurt        | Strawberry     | 4    | 500    | g                  |

La imatge de sota mostra com aquests productes es mostren a la botiga. Vegeu com el camp del 'nom' esdevé el nom principal, que encapçala el producte, i el camp de la columa 'nom\_desplegat' esdevé el nom secundari o de la variant. En el cas de la Bossa d'enciam, el camp 'nom\_desplegat' està en blanc, així que s'usa per defecte el camp que la columna 'nom', el nom genèric.

![](<../../.gitbook/assets/imatge (40).png>)

#### Exemples d'unitats de mesura  <a href="#unit-type-examples" id="unit-type-examples"></a>

Sota hi ha alguns exemples per mostrar com s'han de pujar productes en diferents unitats (g, ml, kg i elements).

| productora                     | **nom**             | **categoria**         | preu | **unitat** | **unitat\_de\_mesura** | **nom\_de\_element** |
| ------------------------------ | ------------------- | --------------------- | ---- | ---------- | ---------------------- | -------------------- |
| Enciams de la Su               | Bossa enciam        | Fruites i hortalisses | 3.50 | 500        | g                      |                      |
| Enric Vilaplana fruites i sucs | Suc de fruita       | Begudes               | 3.50 | 300        | ml                     |                      |
| Patates olotines sccl          | Patates             | Fruites i hortalisses | 9.50 | 5          | kg                     |                      |
| Forn ecològic El molí          | Pa de gra intengral | Producte fornejat     | 3.00 | 1          |                        | barra                |

### Importar l'arxiu CSV  <a href="#import-the-csv" id="import-the-csv"></a>

Una vegada heu omplert la **Plantilla de Llista de Productes CSV** esteu preparats per pujar-la a Katuma.

Aneu a **Productes** > **Importació de Productes.**

**Selecciuneu el tipus d'importació:** Seleccioneu Llista de Productes.

**Seleccioneu un full de càlcul per carregar:** trobeu l'arxiu csv que voleu pujar.

Com que esteu pujant nous productes, podeu deixar sense marcar la casella '_Estableix un estoc de 0 per a tots els productes que no estiguin presents en l'arxiu'._

Fes clic a **Carregar.**

Se us mostrarà un resum de la vostra càrrega, inclòs qualsevol error. També se us comunicarà quants productes esteu creant i quants esteu actualitzant. Si esteu satisfetes amb el resultat de la pujada, feu clic a **desar**. Posteriorment podeu carregar un nou full de càlcul o anar a la pàgina de productes per veure els nous productes.

{% hint style="info" %}
És una bona pràctica comprovar que els productes s'han carregat/actualitzat com esperàveu.
{% endhint %}

## 2) Actualitzar detalls de productes existents

Les instruccions de sota expliquen com actualitzar els detalls d'un producte ja existent en el perfil de la productora. Aquesta eina està destinada a actualitzar més ràpidament preus o nivells d'estoc.

Podeu simultàniament carregar nous productes i actualitzar productes ja existents utilitzant un sol arxiu CSV. Les instruccions d'aquesta guia estàn separades per a més claredat però podeu combinar nous productes i actualitzacions de productes existents en el mateix full de càlcul.

### Prepareu l'arxiu CSV per importar  <a href="#prepare-the-csv-file-for-import-1" id="prepare-the-csv-file-for-import-1"></a>

El proces per actualitzar detalls del producte és similar al de carregar nous productes. El primer pas és descarregar la **Plantilla de Llista de Productes** i omplir els noms dels productes i de les productores. Si teniu disponible aquest full de càlcul d'una càrrega anterior encara millor.

El sistema requereix omplir 7 camps, la qual cosa és necessària i s'utilitza per identificar correctament els productes quan s'actualitzen. Hi ha 4 camps que es poden actualitzar. 3 camps no es poden actualitzar amb l'eina d'importació de productes.

| Camps obligatoris (no es poden actualitzar) | Camps que es poden actualitzar       | Camps que no es poden actualitzar i  no són obligatoris |
| ------------------------------------------- | ------------------------------------ | ------------------------------------------------------- |
| \*productora                                | SKU (codi de referència de magatzem) | ^nom\_de\_element                                       |
| \*nom                                       | preu                                 | ^tipus\_impost                                          |
| ^categoria                                  | disponible                           | ^tipus\_enviament                                       |
| \*unitat                                    | sota\_demanda                        | ​                                                       |
| ^unitat\_de\_mesura (si és aplicable)       | ​                                    | ​                                                       |
| ^nom\_de\_element (si és aplicable)         | ​                                    | ​                                                       |
| \*nom\_desplegat                            | ​                                    | ​                                                       |

_^ si intenteu actualitzar aquests camps veure un missatge d'error_

_\*si intenteu actualitzar aquests camps en realitat creareu nous productes o variants enlloc d'actualitzar productes ja existents_

Les columnes verdes són obligatòries, les taronges es poden actualitzar i les blanques no es poden actualitzar i no són obligatòries.

![](<../../.gitbook/assets/imatge (27).png>)

### **Importeu l'arxiu CSV**  <a href="#import-the-csv-1" id="import-the-csv-1"></a>

Una vegada heu omplert la **Plantilla de la Llista de Productes CSV** esteu preparades per carregar-la a Katuma.

Aneu a **Productes** > **Importació de Productes.**

**Seleccioneu tipus d'importació:** Seleccioneu Llista de Productes.

**Seleccioneu un full de càlcul per carregar:** Busqueu l'arxiu csv que voleu pujar.

**Establiu l'estoc a zero per a totes els productes no existents a l'arxiu:** si seleccioneu aquesta casella el sistema establirà el valor 'disponible' a zero per a tots aquells productes. Si un producte estava 'Sota demanda' es mantindrà 'Sota demanda'. Els productes en aquesta importació retindran el nivell d'estoc que havieu estalbert al full de càlcul.

Feu clic a **actualitzar.**

Se us mostrarà un resum de l'actualització, incloent-hi errors. També se us dirà quants productes esteu creant i quants esteu actualitzant. Si preteníeu només actualitzar productes però veieu que heu creat productes nous, podeu veure quina línia està, tornar enrere i arreglar el full de càlcul. Si, enc anvi, esteu satisfetes amb el resultat de la pujada, feu clic a **desar**. Posteriorment podeu carregar un nou full de càlcul o anar a la pàgina de productes per veure els nous productes.

## Importar Nou Inventari  <a href="#import-new-inventory" id="import-new-inventory"></a>

Molt aviat.

## Actualitzar detalls d'un Inventari existent

Molt aviat.
