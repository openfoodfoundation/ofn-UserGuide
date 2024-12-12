# Posar preu a productes indivisibles o irregulars

Quan s'enumeren els productes carnis o d'altres amb una mida i un preu estàndard (per exemple: 1 paquet de salsitxes - 9€) o productes que són divisibles (per exemple, carn picada), afegir els preus dels productes és senzill. Tanmateix, quan es tracta d'afegir productes de mida irregular que no es poden dividir, com pollastres o cuixes de xai, posar els preus es torna una mica més complex. Hi ha un parell de maneres amb què els productors poden solucionar aquests reptes.

Vegem un exemple. Un productor ven cuixes de xai. Solen tenir un pes d'entre 1,5 i 2,5 kg i cobra 15€ per kg. Com que cada peça és única, no pot llistar el producte com una simple ‘cuixa de xai’, amb un preu fix. A continuació es detallen algunes opcions per front a aquests casos.

## Carrega pel preu mitjà i reemborsa

Podeu carregar el preu mitjà del producte i, a continuació, reemborsar o carregar al client el preu addicional, si el pes real es desvia d'aquest pes mitjà. Per tant, en aquest exemple, cobraria 30€ per cuixa, basant-se en una mitjana de 2 quilograms. Quan es pesa i es carrega la cuixa real, es pot calcular una desviació de 500g, que requereix que reemborsin 7,50€.

Quan coneixeu el pes real dels vostres productes, podeu actualitzar les comandes a la [Gestió de comandes en bloc](https://guia.katuma.org/funcionalitats-avancades/comandes). Cerqueu la cuixa de xai i veureu totes les comandes que contenen aquest producte. Feu que la columna "pes / volum" sigui visible. Els valors d'aquesta columna es poden editar per reflectir els pesos reals de les potes de xai assignades a cada client. L'exemple següent mostra que quan la comanda de la Claire s'ajusta a una cuixa de xai d’1,5 kg, el preu es recalcula automàticament. Feu clic a l'actualització per desar aquest canvi.

![](<../../.gitbook/assets/imatge (18).png>)

Ara, quan vegeu la comanda de la Claire, es mostrarà el total correcte i tots els informes reflectiran aquest canvi. També podeu tornar a enviar la confirmació de la comanda al client.

## Indiqueu el producte en intervals de pes

Aquest és un enfocament semblant a l'anterior, però en comptes de llistar el preu d’un producte segons la mitjana de pes, podeu classificar intervals de pes per augmentar la probabilitat que el client obtingui un producte de la mida que prefereixi. Per exemple, podeu donar al client una elecció entre una cuixa més petita (1,5-2 kg) i una cuixa més gran (2-2,5 kg). Es poden crear com a 2 variants del mateix producte. El preu de cada mida es pot calcular en funció de la mitjana, l'extrem superior o inferior del rang de pes. Si el preu es basa en el límit superior, és probable que hagi de reemborsar la diferència al client. Si el preu es basa en el valor inferior, és probable que hàgiu de sol·licitar un pagament addicional. Podeu crear tants increments de pes que vulgueu i pugueu atendre.

## Enumeren cada elements com a únics i individuals (per exemple: productes congelats)

Si teniu els articles únics disponibles podeu enumerar cada element individual amb el seu pes i preu exactes. Per exemple, l'exemple següent mostra les cuixes congelades de bestiar pre-pesades i envasades que figuren com a variants úniques, amb un valor de disponibilitat d’1. La imatge següent mostra com s'introdueixen les variants del producte i com es mostraran a la botiga.

![](<../../.gitbook/assets/imatge (71).png>)

## Subministrament irregular

Pot ser complicat que els productors de carn puguin predir els productes exactes que tindran fins després del processament. Per exemple, un productor d'aus de corral pot esperar tenir 12 pollastres mitjans, però després d'un atac de guineu, li'n poden quedar només 6 de mitjans, i 6 més petits. Per tant, el productor ha de poder ajustar les comandes, alertar els clients de l'escassetat i del canvi corresponent en la seva comanda. El producte pot ser eliminat de la seva comanda o substituït per alguna cosa semblant.

Les comandes es poden ajustar en el[ Llistat de comandes](https://guia.katuma.org/funcionalitats-avancades/comandes). Alerteu el client a qualsevol canvi en la seva comanda.

## Reemborsament o recaptació de pagament addicional a Katuma

Reemborsar o cobrar un pagament addicional és el més senzill quan el Mètode de pagament és efectiu en el moment de la recollida o lliurament de la comanda.

Una alternativa al reemborsament és demanar que els clients paguin només un 80% en el moment de fer la comanda i l'altre 20% una vegada que es confirmi. Aquest 20% pot canviar segons els preus finals. Open Food Network no té cap eina automatitzada per a això. En lloc d'això, haureu de posar aquestes instruccions a la descripció del Mètode de pagament, que es mostrarà al client en fer la compra i en el correu electrònic de confirmació de la comanda. No obstant això, estigueu preparats perquè els clients ometin aquestes instruccions.

En el futur, Open Food Network té previst desenvolupar comptes de clients, mitjançant els quals es podrà realitzar el seguiment de reemborsaments i permetre que les botigues generin "crèdits de la botiga".

## Alertes a les consumidores de la vostra política de preus

Cada botiga de Katuma té l'opció de posar un missatge a la part superior de la seva botiga. Aquest és un lloc adequat perquè els clients sàpiguen que els preus poden variar després de la comanda. Les instruccions per fer-ho estan [aquí](https://guia.katuma.org/basic-features/configuracio-de-lorganitzacio), a la **Configuració de la botiga**.

El quadre de descripció del Mètode de pagament és un altre lloc per enviar un missatge al client, com ara "el preu final pot variar en un 10% màxim a causa de la variabilitat del producte, ens posarem en contacte amb vostè per variacions superiors a això".
