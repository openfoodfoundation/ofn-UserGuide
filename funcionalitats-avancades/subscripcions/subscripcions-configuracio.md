# Subscripcions - configuració

## 1) Permetre subscripcions

Per permetre l'eina de Subscripcions necessitareu activar la funcionalitat a la configuració de l'organització. Un cop activades, les taules i controls addicionals per a les subscripcions esdevindran visibles. Podeu trobar aquestes configuracions a la taula de [Configuració de la botiga](https://guia.katuma.org/basic-features/configuracio-de-lorganitzacio#configuracio-de-la-botiga).

**Subscripcions**: Per activar les subscripcions, seleccioneu 'Habilitar'.

**Comandes de convidats**: Recomanem que les botigues que ofereixen la possibilitat de subscripcions també demanin a les consumidores l'inici de sessió abans de poder fer la compra. Això us assegurarà que qualsevol consumidora amb una subscripció iniciarà sessió i veurà la seva subscripció existent i no realitzarà accidentalment una comanda per duplicat.

**Canviar comandes**: Les organitzacions poden escollir si permeten a les consumidores editar o no les seves comandes mentre el cicle de comanda està obert.

* Si permeteu que les consumidores canvïin les seves comandes, podran esborrar articles de la seva subscripció o cancel·lar la comanda. Si les consumidores volen afegir alguna cosa a les seves comandes necessitaran realitzar una nova comanda.
* Si no permeteu a les consumidores modificar les seves comandes, necessitaran contactar amb vosaltres si volen treure articles de la seva comanda o cancel·lar-la. Amb aquesta configuració, les consumidores podent igualment escollir fer una nova comanda.

## 2) Assegureu-vos de tenir els mètodes d'Enviament i Pagament configurats  <a href="#id-2-make-sure-you-have-shipping-and-payment-methods-setup" id="id-2-make-sure-you-have-shipping-and-payment-methods-setup"></a>

Quan arribi el pas de crear la subscripció de la consumidora, necessitareu seleccionar quin mètode d'enviament utilitzarà i amb quin mètode de pagament se li facturarà.

#### **Mètodes d'enviament**  <a href="#shipping-methods" id="shipping-methods"></a>

Podeu aplicar qualsevol mètode d'enviament a una subscripció. Vegeu aquí les instruccions per [configurar un mètode d'enviament](https://guia.katuma.org/basic-features/metodes-denviament).

#### **Mètodes de pagament**  <a href="#payment-methods" id="payment-methods"></a>

Només podeu assignar dos tipus de mètodes de pagament a les subscripcions. Vegeu aquí les instruccions per configurar un mètode de pagament.

**1) Mètode de pagament manual**: el qual inclou el pagament en efectiu o per transferència bancària, ambdós fora de la plataforma.

**2) Stripe:** Stripe és una passarel·la de pagament que accepta pagaments amb targeta de crèdit. Quan apliqueu Stripe com a mètode de pagament per a la subscripció d'una consumidora, Stripe carregarà a la targeta de crèdit automàticament l'import cada vegada que es processi una de les seves comandes de subscripció. L'import que es carregarà reflectirà qualsevol canvi que hagi fet a la comanda subscrita, i no es carregarà si es cancel·la o pausa la subscripció.

Abans que una botiga pugui carregar exitosament una consumidora, aquesta ha d'iniciar sessió a Katuma, desar una targeta de crèdit al seu compte i donar permisos a la vostra botiga per carregar-li l'import de les subscripcions a la targeta de crèdit. Podeu consultar més detalls sobre aquests passos a la pàgina [Subscripcions - la perspectiva de la consumidora](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-la-perspectiva-de-la-consumidora).

Tingueu en compte que quan configureu Stripe per usar-lo a les subscripcions és bo que el nom i la descripció del mètode de pagament siguin aclaridors.

Per exemple, en lloc d'anomenar un mètode de pagament 'Targeta de crèdit' potser l'hauríeu d'anomenar 'facturació automàtica a targetes de crèdit per a subscripcions'. Una possible descripció podria ser 'A la targeta de crèdit desada per defecte al teu compte de Katuma se li carregarà l'import de la teva subscripció quan la comanda es confirmi automàticament els divendres a la nit'. Aquest nom i aquesta descripció es mostraran al correu electrònic de confirmació a les consumidores subscrites (vegeu l'exemple de sota), i és bo tenir en compte aquests detalls perquè la consumidora sàpiga què ha d'esperar que passi.

![](<../../.gitbook/assets/imatge (12).png>)

## 3) Recopilar informació de les vostres consumidores  <a href="#id-3-gather-information-from-your-customers" id="id-3-gather-information-from-your-customers"></a>

Per configurar una subscripció per a una consumidora necessiatreu obtenir alguna informació seva, com la que es detalla a continuació. Podeu fer això un dia que us trobeu, o bé per correu electrònic o un [formulari de google](https://www.google.com.au/forms/about/).

**Nom, número de telèfon i correu electrònic** de preferència. Tal i com es detalla a continuació, heu d'afegir les direccions de correu electrònic a la vostra [Llista de Consumidores](https://guia.katuma.org/funcionalitats-avancades/configuracio-de-la-botiga/consumidores) abans de crear una subscripció per a elles, i necessitareu aquesta informació.

**Adreça de facturació i lliurament**: necessitareu aquesta informació quan configureu una subscripció.

**Productes:** quins articles es volen incloure a la subscripció. Necessitareu aquesta informació quan configureu una subscripció.

**Mètode d'enviament:** necessitareu assignar a la subscripció un mètode d'enviament.

**Mètode de pagament:** les consumidores poden triar entre els mètodes de pagament manuals (en efectiu, transferència bancària) o pagar amb targeta de crèdit a través del compte d'Stripe de la vostra botiga. En aquest cas que esteu oferint càrrecs automatitzats a targetes de crèdit a través de la passarel·la de pagament Stripe necessitareu que les vostres consumidores afegeixin la informació de la seva targeta de crèdit al seu compte de Katuma (vegeu més avall).

**Dates que volen que la subscripció abasti:** Recordeu, per fer una comanda de subscripció en un cicle de comandes determinat, la data d'inici de la subscripció ha de ser anterior o posterior a la de l'obertura del cicle de comandes i la data de finalització de la subscripció, posterior a la de tancament del cicle de comandes.

## 4) Afegiu les subscriptores a la vostra Llista de Consumidores  <a href="#id-4-add-your-subscribers-to-your-customer-list" id="id-4-add-your-subscribers-to-your-customer-list"></a>

Abans de poder configurar una subscripció per a una consumidora necessiten estar a la vostra Llista de Consumidores. Vegeu aquí les instruccions per mantenir la vostra [Llista de Consumidores](https://guia.katuma.org/funcionalitats-avancades/configuracio-de-la-botiga/consumidores).

**Després d'haver afegit les consumidores a la llista comenta'ls-hi o envia'ls-hi un correu electrònic** i demana'ls que es registrin per tenir un compte a Katuma. _\*\*_&#x4C;es instruccions per fer-ho es poden trobar [aquí](https://guia.katuma.org/basic-features/register-and-create-your-profile). Si planegeu cobrar les consumidores a través de la passarel·la de pagament Stripe, necessiteu també demanar-los que [desin els detalls de les seves targetes de crèdit i autoritzin la teva botiga a fer els càrrecs corresponents](https://guide.openfoodnetwork.org/advanced-features/subscriptions/subscriptions-the-customers-perspective).

Podeu afegir consumidores a la Llista de consumidores abans o després que tinguin creat un compte a Katuma. Sigui com sigui, tingueu en compte que abans de poder completar amb èxit la configuració d'una comanda amb subscripció la consumidora la consumidora ha de registrar-se i confirmar el correu electrònic.

A més, si voleu usar Stripe per fer els cobraments amb targeta de crèdit a les vostres subscriptores, haureu d'afegir a la llista de consumidores abans que us pugui donar permisos perquè els pugueu carregar els imports.

Per tant un suggerim el següent procés: a) contacteu amb les consumidores de la vostra botiga perquè us donin les seves dades b) afegiu-les a la llista de consumidores c) demaneu-los en persona o per correu electrònic que es registrin a Katuma (i que us donin permisos per cobrar-los amb targeta, si la vostra botiga té habilitat el mètode de pagament per Stripe) i després [d) creeu la subscripció](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-crear-i-gestionar-comandes#6-crear-subscripcions).

## 5) Programacions

{% hint style="info" %}
Si sou nous a Katuma us animem a familiaritzar-vos amb la configuració dels [cicles de comanda](https://guia.katuma.org/basic-features/order-cycles-for-hubs) abans de configurar les programacions de les subscripcions.
{% endhint %}

### Sobre les programacions

Les subscripcions s'han configurat així que cada vegada que una botiga obre un cicle de comanda, les comandes es generaran automàticament per a les consumidores que tenen una subscripció amb aquesta botiga. Malgrat això, el sistema té la flexibilitat afegida de permetre decidir a les botigues en quins cicles de comanda aplica o no la subscripció. Això permet a les botigues tenir cicles de comanda en les quals activen les comandes de subscripció i alguns en els que no ho fan.

En quins cicles de comanda s'activen les subscripcions es controla a trtavés d'un element addicional en el procés de configuració d'un Cicle de Comanda, anomenat 'programacions'. Les programacions són grups als quals es pot assignar un cicle de comanda. Una vegada s'ha creat una programació, les programacions de la consumidora s'apliquen a la programació, de manera que només es generarà una comanda per a nous cicles de comanda inclosos en aquesta programació.

Clarifiquem-ho amb alguns exemples:

**Exemple 1**

La Cooperativa de Consum La Pastanaga té un cicle de comanda setmanal. Les consumidores poden decidir subscriure's a una comanda setmanal o bé quinzenal.

En aquest cas hi haurà dues programacions. Una que conté tots els cicles de comanda - els subscriptors setmanals tindran les seves subscripcions assignades a aquesta programació. La segona programació contindrà només un de cada dos cicles de comanda - els subscriptors setmanals tindran la seva subscripció assignada a aquesta programació.

#### Exemple 2  <a href="#example-2" id="example-2"></a>

La granja Delta té dos cicles de comanda setmanals, un per al lliurament dels dilluns i un per al lliurament dels dijous.

La majoria de les seves consumidores es subscriuen per un dels lliuraments a la setmana, però algunes de les seves subscriptores del sector de l'hostaleria es subscriuen als dos lliuraments, tant el de dilluns com el de dijous.

En aquest cas hi haurà dues programacions, una per a les consumidores de dilluns i una per a les consumidores de dijous. Aquelles consumidores que volen una subscripció per als dos dies poden tenir una subscripció aplicada a les dues programacions.

### Crear una programació

Una vegada heu [habilitat a funcionalitat de les subscripcions](https://guia.katuma.org/funcionalitats-avancades/subscripcions/subscripcions-configuracio#1-permetre-subscripcions), veureu l'opció de Programacions a la interfície del cicle de comandes. Per crear una programació feu clic al botó **+Nova programació**.

> Nota: Heu de tenir com a mínim un cicle de comanda que pugui ser afegit a la programació abans de poder-la crear.

![](<../../.gitbook/assets/imatge (68).png>)

**Nom:** Doneu a la programació un nom lògic el qual descrigui aquest grup de cicles de comanda. Per exemple: 'setmanal', 'mensual', 'lliurament dels dijous', 'a l'engròs' o 'al detall'. Aquest nom només és visible per a vosaltres al _backend_, no a les consumidores.

Podeu afegir cicles de comanda existents dins i fora de la nova programació fent clic als botons < i >.

Quan hagueu acabat feu clic a **crear**.

### Editar o eliminar una programació

Per editar o eliminar una programació, feu clic al nom de la programació al costat del corresponent cicle de comanda, a la columna 'programacions'.

> Nota: aquesta columna ha d'estar configurada com a visible en el menú desplegable.

![](<../../.gitbook/assets/imatge (2).png>)

Podeu canviar el nom de la programació, afegir-hi o eliminar-hi cicles de comanda o esborrar la programació.

![](<../../.gitbook/assets/imatge (36).png>)

> Nota: No podeu esborrar una programació si té subscripcions associades.

### Afegir o eliminar cicles de comanda d'una programació

Poden afegir i eliminar cicles de comanda de les programacions tant editant la programació (al damunt) com editant el cicle de comanda i afegint/eliminant la programació a la casella 'programacions' (sota).

![](<../../.gitbook/assets/imatge (10).png>)

Els cicles de comanda poden formar part de més d'una programació. Sense anar més lluny, en l'exemple descrit més amunt de la Cooperativa de Consum La Pastanaga, cada segon cicle de comanda formarà part tant de la programació setmanal com de la quinzenal.
