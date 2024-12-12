# Incrustar una pàgina de grup

Aquesta funcionalitat us permet incrustar la pàgina de grup a un web extern a Katuma. Això us permet usar l'eina de directori de grup de Katuma a la vostra pròpia web. Aquesta pàgina detalla quins requisits es necessiten per incrustar una pàgina de grup, i les passes que configurar-la. Hi ha també un exemple de com es veu una pàgina de grup incrustada.&#x20;

## Requisits

### Plataforma

Aquesta funcionalitat és relativament nova i encara l'estem testant, però hauria de funcionar amb qualsevol tipus de pàgina, **sempre que pugueu afegir un html personalitzat** a la pàgina on vulgueu incloure la pàgina de grup.  Ja sigui la vostra web feta amb WordPress, Squarspace, Wix o alguna altra plataforma, hauria de ser possible configurar la incrustació de la pàgina de grup.

Sota hi ha alguns recursos específics segons la plataforma:&#x20;

* Squarespace us permet 'afegir customer html' via els seus 'codeblocks':[ vegeu aquí](https://support.squarespace.com/hc/en-us/articles/206543167).

### Seguretat

Donat que Open Food Network és una plataforma de comerç online i maneja transaccions monetàries, té uns requisits de seguretat més elevats que webs amb només text. Per aquesta raó, necessiteu configurar els protocols criptogràfics SSL/TLS a la pàgina on vulgueu incrustar la vostra pàgina de grup si no ho heu fet abans.&#x20;

Podeu obtenir aquest certificar de seguretat de manera gratuïta a [Let’s Encrypt](https://letsencrypt.org/) o per al voltant de 10-40€ per un servei de pagament.&#x20;

### Pàgina de grup a Katuma

Per suposat, l'últim requisit és que hagueu configurat una pàgina de grup a Katuma. Necessitareu saber quin és l'enllaç de la vostra pàgina de grup per als passos de configuració que veureu més avall.&#x20;

## Configuració

**1) Contacta amb la teva instància local d'Open Food Network**&#x20;

Primer de tot, necessitareu contactar amb el vostre equip local i fer-los saber que voleu incrustar la vostra pàgina de grup de Katuma al vostre web. Necessitareu donar-los el vostre domini extern i us donaran permisos per comunicar el vostre web amb Katuma.

**2) Afegir un HTML personalitzat al vostre web**

Incrustar la vostra botiga és tan simple com inserir una línia de codi a la vostra web. Aquesta és la línia d'html que hauríeu d'inserir a la pàgina on vulgueu la pàgina del grup:&#x20;

```
<iframe src="/groups/flavour-crusader?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

Al html de dalt estigueu segurs de reemplaçar 'flavour-crusader' amb l'enllaç permanent únic de la vostra pàgina de grup a Katuma.&#x20;

Una vegada heu fet això, hauríeu de veure la vostra pàgina de grup de Katuma a la vostra pàgina web. &#x20;

**3) Estilisme**

Depenent de l'estil del vostre web necessitareu fer algun ajustament del CSS. Es pot necessitar evitar tenir dues barres de desplaçament, o assegurar-se que la llargada i amplada de la pàgina incrustada es veu visualment atractiva. Estigueu segures de provar com es veu la vostra pàgina de grup en dispositius mòbils. Si la pantalla de mòbil està mal composta segurament necessiteu més ajustaments CSS. Els ajustaments CSS requerits seran diferents a cada lloc però el vostre administrador web hauria de poder ajudar-vos.&#x20;

### Exemple

Hem configurat un e[xemple d'una pàgina de grup incrustada](https://openfoodnetwork.org/user-guide/advanced-features/demo-embedded-group/), usant Flavour Crusader perquè vegeu i proveu com funciona. S'ha incrustat a la pàgina global d'Open Food Network, que és un lloc de Wordpress.

## Instruccions per a visitants

### Cookies

La majoria de gent té activades cookies als seus navegadors web. Però si un visitant no té activades les cookies no podrà veure la incrustació del grup.&#x20;

![](<../../.gitbook/assets/imatge (65).png>)
