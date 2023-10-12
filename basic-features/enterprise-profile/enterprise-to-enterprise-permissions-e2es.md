# Unternehmensberechtigungen

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Unternehmensberechtigungen&#x20;

Innerhalb der OFN-Unternehmensberechtigungen gibt es Regeln, die Handelsbeziehungen zwischen Unternehmen regeln: Lieferanten und Händler. Diese Regeln müssen aufgestellt werden, bevor ein Unternehmen (Herstellerprofil oder Herstellershop) Lieferant eines anderen (Hub) werden kann oder umgekehrt. Eine Erlaubnis (oder ein "Recht") wird von einem Unternehmen an ein anderes erteilt, was den Zugang / die Änderung von Produkten und Profilen betrifft. Auf dieser Seite werden die verschiedenen Berechtigungen und deren Zuweisung beschrieben.

So greifen Sie auf Ihre Unternehmensberechtigungen zu:

![](../../.gitbook/assets/permissions.gif)

Schließlich untersuchen wir dieses Thema unter dem Gesichtspunkt der:

* [ein Hub](enterprise-to-enterprise-permissions-e2es.md#perspektive-der-hubs) (der Verteiler)
* [ein Herstellerprofil oder ein Geschäft](enterprise-to-enterprise-permissions-e2es.md#die-perspektive-des-produzenten) (der Lieferant)

## Die vier Erlaubnisse

Es gibt 4 verschiedene Arten von Unternehmensberechtigungen. Sie können auf unterschiedliche Weise kombiniert werden, um Unternehmen je nach ihrem Profil mehr oder weniger Rechte zu geben.

![](../../.gitbook/assets/e2emenu2.jpg)

**Erlaubnis zum Hinzufügen zum Bestellzyklus:** Der Lieferant (Hersteller) erlaubt dem Händler (einem OFN Hub), Produkte zu dessen Bestellzyklen hinzuzufügen. Auf diese Weise können die Produkte des Lieferanten im Schaufenster des Hubs erscheinen.

**Berechtigung zur Verwaltung von Produkten:** Der Lieferant ermächtigt ein anderes im OFN registriertes Unternehmen (in der Regel ein Hub), Produkte direkt in seinem Lieferantenkatalog anzulegen, zu löschen und zu ändern.

{% hint style="danger" %}
Dies kann sich potenziell auf alle Drehkreuze auswirken, die der Hersteller über OFN mit Waren beliefert.
{% endhint %}

> Wenn Landwirt Jo beispielsweise Kartoffeln an die Hubs A und B liefert, aber Hub A die Erlaubnis erteilt, seine Produkte zu verwalten, dann wird sich diese Preisänderung (bei Standardeinstellungen) an den Schaufenstern der Hubs A und B widerspiegeln, wenn Hub A den Preis der Kartoffeln ändert.

**Berechtigung zur Profilbearbeitung:** Ein Unternehmen erlaubt einem anderen, Details in seinem [Unternehmensprofil](./) zu ändern (Kontaktdaten, Adresse, Beschreibung, ...).

Erlaubnis, Produkte zum Inventar hinzuzufügen: Der Lieferant (Hersteller) ermächtigt den Händler (Hub), seine Produkte in den Shop-Katalog (oder "[Inventar](../products-1/inventory-tool.md)") des Hubs aufzunehmen.

{% hint style="info" %}
Wenn ein Hersteller mehr als einen Hub mit Waren beliefert, empfehlen wir, diese Berechtigung zwischen den beiden Unternehmen einzufügen, damit jeder dieser Hubs die Preise und Lagerbestände seiner Produkte unabhängig verwalten kann und die Hubs ihre [Bestandseinstellungen](enterprise-settings.md#inventar-einstellungen) ändern können.
{% endhint %}

## Erteilen und Verwalten von Berechtigungen

Um Berechtigungen zu ändern, hinzuzufügen oder zu löschen, gehen Sie auf das Admin-Dashboard und dann auf "Unternehmen" im blauen Menü und "Berechtigungen" im grünen Untermenü.

![](../../.gitbook/assets/e2emenu.jpg)

Erlaubnis erteilen:

* Wählen Sie Ihr Unternehmen aus dem Dropdown-Menü in der ersten Spalte aus (Sie sind ein Hersteller, der andere beliefert)
* Wählen Sie in der zweiten Spalte den Namen des Unternehmens (Hub) aus, das Sie beliefern möchten.
* Kreuzen Sie die Berechtigungen an, die Sie dem Händler Ihrer Waren (Hub) erteilen möchten, oder wählen Sie "alles", um mehrere Berechtigungen zu erteilen.
* Klicken Sie auf "Erstellen".

&#x20;Beachten Sie, dass Sie diese Berechtigungen jederzeit löschen oder ändern können.

{% hint style="warning" %}
Nur Benutzer, die als [Manager](enterprise-settings.md#benutzer) eines Unternehmens aufgeführt sind, können dessen Berechtigungen ändern.
{% endhint %}

Wenn Sie von einem anderen Unternehmen Genehmigungen benötigen, müssen Sie dieses per E-Mail oder Telefon kontaktieren. Es gibt keine Online-Funktion, um dies zu tun.

## Automatisch generierte Berechtigungen

When a user is the main manager (owner) of several enterprises on the platform, [permissions](enterprise-to-enterprise-permissions-e2es.md#the-four-permissions) are created automatically between each enterprise. This is not the case when enterprises are managed by different users.

## Perspektive der Hubs

Die folgenden häufigen Szenarien veranschaulichen die Berechtigungen für Unternehmen, die Sie möglicherweise für Ihren Hub einrichten müssen.

> **I have** [**created Producer Profiles for each of my suppliers**](create-or-connect-with-your-supplying-producers.md#supplier-does-not-have-an-ofn-profile)**. Which permissions do I need to set up before I can stock their products on my Hub shopfront?**

The system is configured so that hubs creating producer profiles will have the _correct permissions installed as default_, so that they can start adding products and trading with these producer profiles right away.

> **My** [**supplier already has an enterprise registered with OFN**](create-or-connect-with-your-supplying-producers.md#supplyingproducer)**. I would like to add their products to my hub shopfront.**

You must contact your supplier in person. Their contact details (phone number, address and email address) will be located in their OFN profile. &#x20;

If you only intend to _**stock their products**_ and don't wish to help them manage the rest of their OFN profile then ask the producer to grant permission _**to add to order cycle**_ and permission _**to add to inventory.**_&#x20;

If the supplier wishes for you, as a Hub manager, to help them organise their OFN enterprise then they may grant you all four permissions.  Should this occur then you will be able to edit their profile and manage their products.

> **My Hub distributes through buying groups. Which permissions will the buying group need with my hub and my producers?**

{% hint style="warning" %}
This is an example of where the hub managing (co-ordinating) an order cycle differs from the enterprise from which customers collect their purchases.

_If Hub A manages (co-ordinates) an order cycle for a buying group (Hub B) then the order cycle will be displayed on Hub B's OFN shopfront._
{% endhint %}

The buying group (Hub B above) will need to grant the order cycle co-ordinator (Hub A above) permission to add to order cycle (and ideally permission to add to inventory).

Producers who supply Hub A with products that are to also be sold by the buying group (Hub B) must grant both Hubs A and B permission to add to order cycle (and ideally permission to add to inventory).

## Die Perspektive des Produzenten

When a producer wants to start selling their products through other enterprises (hubs or buying groups) the must establish the appropriate enterprise-to-enterprise permissions. There are different levels of permission that a producer can grant, depending on how much power they want to give the hub to manage their products and profile (see [top of page](enterprise-to-enterprise-permissions-e2es.md#the-four-permissions)).

These examples explore some common scenarios.

> **I am a producer and would like a local OFN hub to stock and sell my products.**

**Essential:** For the hub to add your products to their shopfront, you’ll need to grant them _'permission to add to order cycle'_.

**Optional:** You might also want to give the hub permission to manage your products, to edit your profile or to add to Inventory.

> **A hub that I supply distributes through buying groups.**

In order for your products to be distributed by the buying groups you will have to add a minimum of permission 'to add to order cycle' for the buying group enterprise _as well as_ the hub you supply directly.

> **I am a Producer Shop who supplies a local Hub as well as running my own shopfront.  The hub would like to manage the stock levels and prices of my products.  I would like to **_**also**_** manage stock levels and prices of my products.**

This scenario can be solved by granting the hub permission to add to Inventory as well as permission to add to order cycle.

This allows the hub to stock your products in their shop, but to set their own prices and inventory levels. When you stock your own shop with your products, they will continue to reflect the prices and stock levels that you have set.
