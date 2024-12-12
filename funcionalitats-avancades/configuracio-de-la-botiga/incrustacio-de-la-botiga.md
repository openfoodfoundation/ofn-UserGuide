---
description: >-
  (La possibilitat d'incrustar una botiga de moment no està disponible però està
  en la llista de millores futures de Katuma)
---

# Incrustació d'una pàgina de grup a una pàgina web

Aquesta funcionalitat permet usuàries que tenen botigues a Katuma incrustar la seva botiga dins les seves pàgines web. Això dona a les consumidores una experiència més fluïda i evita la necessitat de redirigir-los entre diversos llocs web. També permet les usuàries conservar la seva marca visual a la botiga. Quan incrusteu una botiga de Katuma a la vostra pàgina web, la vostra botiga dins la plataforma roman, es manté, així que les consumidores poden escollir on us volen comprar. Aquesta pàgina detalla els requisits per utilitzar botigues incrustades i els passos que cal seguir per configurar-les. També hi ha un enllaç a un exemple sobre com es veu una botiga incrustada.

## Requisits

### Plataformes

Aquesta funcionalitat és relativament nova i encara l'estem testant, però hauria de funcionar en qualsevol tipus de lloc web, sempre que pugueu afegir un codi HTML personalitzat a la pàgina on vulgueu la botiga. Tant si la vostra web està creada a WordPress, Squarespace, Wix o una altra plataforma hauria de ser possible configurar-hi la incrustació de la vostra botiga.&#x20;

Sota hi ha recursos específics per a algunes plataformes:

Squarespace us permet ‘add customer html’ per via dels seus “codeblocks” – vegeu aquí.&#x20;

#### Seguretat

Com que Katuma (OFN) és una plataforma de comenrç online, i maneja transaccions monetàries, té uns requisits de seguretat més alts que les webs només de text. Per tant, necessitareu configurar els certificats de seguretat SSL/TLS al web on vulgueu incrustar-hi la botiga si no ho havíeu fet anteriorment.&#x20;

Podeu obtenir aquest certificat de seguretat de forma gratuïta de [Let's Encrypt](https://letsencrypt.org/) o per al voltant de 10-30€ per un servei de pagament.

### Botiga a Katuma (OFN)

És clar, l'últim requisit és que tingueu una botiga configurada a Katuma. Necessiteu saber quin és l'URL de la vostra botiga en les passes següents, descrites a continuació.

Passes de configuració

**1) Contacteu amb la vostra instància local d'Open Food Network**&#x20;

Primer de tot necessiteu contactar amb la vostra instpancia local d'Open Food Network (en aquest cas, Katuma) i fer-los saber que voleu incrustar la vostra botiga a Katuma al vostre lloc web. Haureu de proporcionar-los el vostre domini extern, per exemple: www.happyhensfarm.com, perquè puguem concedir el permís perquè el vostre lloc web es comuniqui amb Katuma.

**2) Afegir la personalització HTML al vostre lloc web**

Incrustar la vostra botiga és tant fàcil com insertar una línia de codi a la vostra web. Aquesta és la línia d'html que haureu d'inserir a la pàgina on vulgueu la botiga:

```
<iframe src=" https://openfoodnetwork.org.au/happy-hens-farm/shop?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

En l'html anterior assegureu-vos de reemplaçar 'happy-hens-farm' pel permalink únic de la vostra botiga a Katuma (el podreu trobar a **Configuració de l'Organització**).

Una vegada heu fet això hauríeu de veure la vostra botiga a Katuma a la vostra pàgina web.&#x20;

**3) Estilisme**

Depenent de l'estil del vostre lloc web necessitareu afegir alguns ajustaments de CSS (colors, tipus de lletra, espai entre els elements...) Es pot necessitar per evitar tenir dues barres de desplaçament, i assegurar-se que la longitud i l'amplada de la botiga incrustada sembla atractiva visualment. Assegureu-vos de provar la visualització de la vostra botiga incrustada en un dispositiu mòbil. Si la pantalla del mòbil està mal composta, és possible que necessiteu més ajustaments CSS. Els ajustaments requerits seran diferents per a cada lloc web, però l'administrador del vostre lloc web hauria de poder ajudar-vos a fer-ho.

**Exemple**

Tenim configurat un [exemple de botiga incrustada](https://openfoodnetwork.org/user-guide/advanced-features/demo-embedded-shop/) perquè veieu com funciona i hi pugueu jugar.

## Instruccions per a consumidores

### Cookies

La majoria de gent té activades cookies als seus navegadorss web. Però si una consumidora no té activades cookies no podran comprar en una botiga incrustada. El missatge d'error que veuran es mostra en la imatge inferior. Tingueu en compte que poden comprar a la versió de la vostra botiga allotjada a Katuma sense necessitat de tenir activades les cookies.

![](<../../.gitbook/assets/imatge (64).png>)
