# Subscripcions - preguntes freqüents

#### Si elimino un cicle de comandes d'una programació quan ja té comandes de subscripció obertes, què passarà amb aquestes comandes? Se suprimiran aquestes subscripcions?&#x20;

Aquestes comandes romandran obertes. Al tancament del cicle de comandes, les comandes de subscripció es processaran com les comandes de subscripció normals. Si voleu cancel·lar totes les comandes de subscripció que s'adjuntaven a aquest cicle de comandes, haureu de fer-ho expressament amb les comandes.

#### Si afegeixo una subscripció nova enmig d'un cicle de comandes obertes, es generarà una subscripció per a aquest client?&#x20;

Sí, si creeu una subscripció mentre hi ha un cicle de comandes obert en aquesta programació, es generarà una comanda per a aquest client. Si no voleu que la subscripció s'apliqui al cicle actual de comandes obertes, haureu d'establir la data d'inici de la subscripció després del tancament d'aquest cicle de comandes.

#### Què passa si no hi ha prou estoc per a servir totes les comandes d'una subscripció? Quins clients obtenen l'estoc limitat?&#x20;

En el cas que l'estoc d'un producte no permeti satisfer totes les comandes de subscripció, l'estoc limitat no s'assignarà de manera uniforme entre els clients, sinó que complirà les comandes dels clients amb l'estoc disponible fins que s'esgoti. Alguns clients rebran la seva comanda completa, altres no rebran cap.

#### Què passa si canvio la subscripció mentre està “oberta”?&#x20;

No és possible afegir articles a l'ordre de subscripció mentre estigui obert un cicle de comanda que la conté. Qualsevol producte addicional s'haurà d'afegir quan es tanquin els cicles de comanda (és a dir, per a les subscripcions setmanals assignades a la programació  "Setmanal", en el període de temps entre el tancament del cicle de comandes A i l'obertura del cicle de comandes B, on tant A com B pertanyen a l'horari 'Semanal').&#x20;

En el cas de què editeu la subscripció bàsica d'un client per eliminar productes mentre hi ha un cicle de comandes obert, aquest canvi afectarà la comanda realitzada en el cicle de comandes vigent.

#### Què passa si hi ha estoc limitat, però després un client cancel·la la seva comanda, aquest estoc s'assignarà automàticament a altres subscriptors que volien aquest producte però que no el poguessin tenir a causa d'un estoc insuficient?&#x20;

No, si un client cancel·la la seva comanda generada per una subscripció o n'elimina un producte, la quantitat alliberada  retornarà a l'estoc dels productes però no s'assignarà automàticament a altres clients. Podeu afegir aquest estoc a la comanda d'un altre client manualment.&#x20;

#### Puc (jo o el client) editar una comanda que s'ha fet mitjançant un sistema de subscripció?&#x20;

Això depèn de si voleu afegir o eliminar productes:&#x20;

* Com a gestor de l'empresa, podreu eliminar productes (o cancel·lar una comanda) que hagi fet el sistema de subscripció a través del tauler d'administració de l'OFN com amb qualsevol altra comanda.
* Com a gestor de l'empresa, si afegiu productes a una comanda realitzada pel sistema de subscripció mitjançant el panell de control de Katuma-OFN, això invocarà a un segon pagament que no es processarà automàticament al final del cicle de la comanda.&#x20;
* Si permeteu que els clients puguin fer-ho mentre el cicle de comandes està obert, podran eliminar articles de la seva comanda generada des de la subscripció. Si volen  afegir articles no ho poden fer a la comanda generada per la subscripció, ho hauran de fer creant una segona comanda de forma manual.
