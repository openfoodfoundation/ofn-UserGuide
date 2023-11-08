# Unternehmensberechtigungen

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

Wenn ein Benutzer der Hauptmanager (Eigentümer) mehrerer Unternehmen auf der Plattform ist, werden die [Berechtigungen](enterprise-to-enterprise-permissions-e2es.md#die-vier-erlaubnisse) automatisch für jedes Unternehmen erstellt. Dies ist nicht der Fall, wenn Unternehmen von verschiedenen Benutzern verwaltet werden.

## Perspektive der Hubs

Die folgenden häufigen Szenarien veranschaulichen die Berechtigungen für Unternehmen, die Sie möglicherweise für Ihren Hub einrichten müssen.

> **Ich habe** [**für jeden meiner Lieferanten ein Herstellerprofil erstellt**](create-or-connect-with-your-supplying-producers.md#der-lieferant-verfuegt-nicht-ueber-ein-ofn-profil.)**. Welche Berechtigungen muss ich einrichten, bevor ich ihre Produkte in meinem Hub-Schaufenster anbieten kann?**

Das System ist so konfiguriert, dass Hubs, die Produzentenprofile erstellen, _standardmäßig über die richtigen Berechtigungen verfügen_, so dass sie sofort mit dem Hinzufügen von Produkten und dem Handel mit diesen Produzentenprofilen beginnen können.

> **Mein**[ **Lieferant hat bereits ein bei OFN registriertes Unternehmen**](create-or-connect-with-your-supplying-producers.md#supplyingproducer)**. Ich möchte seine Produkte in mein Hub-Schaufenster aufnehmen.**

Sie müssen Ihren Lieferanten persönlich kontaktieren. Die Kontaktdaten (Telefonnummer, Adresse und E-Mail-Adresse) finden Sie in seinem OFN-Profil.

Wenn Sie nur beabsichtigen, **die Produkte des Herstellers zu lagern** und ihm nicht bei der Verwaltung des übrigen OFN-Profils helfen wollen, bitten Sie den Hersteller um die Erlaubnis, **den Bestellzyklus zu ergänzen** und **den Bestand zu ergänzen**.

Wenn der Anbieter möchte, dass Sie als Hub-Manager ihm bei der Organisation seines OFN-Unternehmens helfen, kann er Ihnen alle vier Berechtigungen erteilen. In diesem Fall können Sie sein Profil bearbeiten und seine Produkte verwalten.

> **Mein Hub vertreibt über Einkaufsgemeinschaften. Welche Berechtigungen benötigt die Einkaufsgemeinschaft mit meinem Hub und meinen Produzenten?**

{% hint style="warning" %}
Dies ist ein Beispiel dafür, dass sich die Drehscheibe, die einen Auftragszyklus verwaltet (koordiniert), von dem Unternehmen unterscheidet, bei dem die Kunden ihre Einkäufe abholen.

_Wenn Hub A einen Auftragszyklus für eine Einkaufsgemeinschaft (Hub B) verwaltet (koordiniert), wird der Auftragszyklus auf dem OFN-Schaufenster von Hub B angezeigt._
{% endhint %}

Die Einkäufergruppe (Hub B oben) muss dem Koordinator des Auftragszyklus (Hub A oben) die Erlaubnis erteilen, dem Auftragszyklus etwas hinzuzufügen (und idealerweise die Erlaubnis, etwas zum Bestand hinzuzufügen).

Produzenten, die Hub A mit Produkten beliefern, die auch von der Einkaufsgemeinschaft (Hub B) verkauft werden sollen, müssen sowohl Hub A als auch Hub B die Erlaubnis erteilen, den Auftragszyklus zu erweitern (und idealerweise die Erlaubnis, den Bestand zu erweitern).

## Die Perspektive des Produzenten

Wenn ein Produzent seine Produkte über andere Unternehmen (Hubs oder Einkaufsgemeinschaften) verkaufen möchte, muss er die entsprechenden Berechtigungen von Unternehmen zu Unternehmen einrichten. Es gibt verschiedene Berechtigungsstufen, die ein Produzent erteilen kann, je nachdem, wie viel Befugnis er dem Hub bei der Verwaltung seiner Produkte und seines Profils einräumen möchte ([siehe oben auf der Seite](enterprise-to-enterprise-permissions-e2es.md#die-vier-erlaubnisse)).

Diese Beispiele zeigen einige gängige Szenarien.

> **Ich bin Produzent und möchte, dass ein lokales OFN-Zentrum meine Produkte lagert und verkauft.**

**Unerlässlich:** Damit der Hub Ihre Produkte zu seinem Schaufenster hinzufügen kann, müssen Sie ihm die "_Erlaubnis zum Hinzufügen zum Bestellzyklus_" erteilen.

**Optional:** Sie können dem Hub auch die Erlaubnis erteilen, Ihre Produkte zu verwalten, Ihr Profil zu bearbeiten oder zum Inventar hinzuzufügen.

> **Eine von mir belieferte Drehscheibe vertreibt über Einkaufsgemeinschaften.**

Damit Ihre Produkte von den Einkaufsgemeinschaften vertrieben werden können, müssen Sie sowohl für das Unternehmen der Einkaufsgemeinschaft als auch für den Hub, den Sie direkt beliefern, mindestens die Berechtigung "zum Bestellzyklus hinzufügen" hinzufügen.

> **Ich bin ein Producer Shop, der ein lokales Hub beliefert und auch mein eigenes Schaufenster betreibt. Die Drehscheibe würde gerne die Lagerbestände und Preise meiner Produkte verwalten. Ich möchte auch die Lagerbestände und Preise meiner Produkte verwalten.**

Dieses Szenario kann gelöst werden, indem man dem Hub die Erlaubnis erteilt, die Produkte zum Inventar hinzuzufügen, sowie die Erlaubnis, sie dem Bestellzyklus hinzuzufügen.

Dadurch kann der Hub Ihre Produkte in seinem Shop lagern, aber seine eigenen Preise und Lagerbestände festlegen. Wenn Sie Ihren eigenen Shop mit Ihren Produkten bestücken, werden diese weiterhin die von Ihnen festgelegten Preise und Lagerbestände widerspiegeln.
