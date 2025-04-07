# Stichwörter und Stichwort-Regeln

Sobald die Kunden in Kategorien mit Stichwörtern gruppiert wurden, können Sie ihr Einkaufserlebnis auf folgende Weise anpassen:

* Bestimmte Produktvarianten sichtbar/unsichtbar machen
* Bestimmte Lieferoptionen sichtbar/unsichtbar machen
* Bestimmte Zahlungsarten sichtbar/unsichtbar machen
* Bestimmte Auftragszyklen sichtbar/unsichtbar machen

Meistens wird diese Funktion von Unternehmen benötigt, die unterschiedliche Shop-Konfigurationen für Mitglieder/Nicht-Mitglieder oder unterschiedliche Kundengruppen wie Groß-/Einzelhandelskunden haben. Weitere Beispiele finden Sie in unserem Abschnitt [Anleitungen](../../../hub-management-tips/how-tos/).

## Wie man eine Stichwort-Regel einrichtet

Um auf Stichwort-Regeln zuzugreifen, gehen Sie zu Unternehmen -> Einstellungen -> Stichwort-Regeln

![](../../../.gitbook/assets/newtagrule1.jpg)

## Standardmäßig

Standardmäßig sind **alle Artikel** für **alle Kunden** sichtbar, unabhängig davon, ob sie markiert sind oder nicht. Sie können die Standard-Anzeigeregeln ändern, indem Sie **+neue Standardregel** hinzufügen wählen. Im folgenden Beispiel sind standardmäßig alle Bestellzyklen, die mit "Großhandel" gekennzeichnet sind, unsichtbar. (In diesem Beispiel können nur die Kunden, die mit dem Stichwort "Großhandelskunde" gekennzeichnet sind, die Bestellzyklen mit dem Stichwort "Großhandel" sehen (und folglich dort einkaufen).

![](../../../.gitbook/assets/defaulttag.jpg)

## Stichwort-Regeln

Sobald Sie Standardregeln definiert haben, können Sie für bestimmte Kundengruppen Ausnahmen von diesen Regeln einrichten.

* Definieren Sie zunächst die Kundengruppe, für die die Ausnahme gelten soll. Im obigen Beispiel wurde die Ausnahme auf alle Kunden mit dem Stichwort "Großhandelskunde" angewendet.
* Dann können Sie für diese Kundengruppe eine von vier Möglichkeiten wählen, ihr Einkaufserlebnis individuell zu gestalten:

![](../../../.gitbook/assets/rule-typess.png)

{% hint style="warning" %}
Denken Sie daran, die entsprechenden Stichwörter zu Varianten, Versand- oder Zahlungsarten oder Bestellzyklen sowie zu Kunden hinzuzufügen, nachdem Sie eine Standard- oder bedingte Stichwort-Regel eingerichtet haben!
{% endhint %}

Im Folgenden werden wir jede Option einzeln betrachten:

### Varianten in meinem Schaufenster anzeigen oder ausblenden

Mit dieser Regel können Sie bestimmte Varianten für markierte Kunden sichtbar/unsichtbar machen. Damit diese Regel funktioniert, müssen Sie den Kunden und die Produktvariante **in Ihrem Bestand** (nicht in der Produktliste des Herstellers) mit demselben Stichwort versehen haben.

Im folgenden Beispiel wurde die 1 kg-Variante von delux muesli mit dem Stichwort "Mitglied" versehen. Es wäre also möglich, Stichwort-Regeln so einzurichten, dass standardmäßig nur die kleinere (nicht getaggte) 500-g-Variante des Delux-Müslis auf der Shop-Front erscheint, es sei denn, der Kunde gehört zu einer Gruppe von Käufern, die alle mit dem Stichwort "Mitglied" versehen sind (in diesem Fall würde er auch die 1 kg-Variante sehen können).

![](<../../../.gitbook/assets/varianttags (1).jpg>)

### Lieferoptionen anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Lieferoptionen für bestimmte Kunden spezifisch verfügbar oder nicht verfügbar machen. Damit diese Regel funktioniert, müssen Sie den Kunden und die Lieferoption mit demselben Stichwort versehen haben. Um eine Lieferoption zu kennzeichnen, gehen Sie zu [Lieferoption](../shipping-methods.md) bearbeiten und wenden Sie die entsprechende Kennzeichnung an.

![](../../../.gitbook/assets/tagshipping.jpg)

In diesem Beispiel wurde die Versandart "Selbstabholung" den Kunden mit dem Stichwort "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Stichwort-Regel: Lieferoptionen mit dem Stichwort "Mitglied" sind unsichtbar
* eine bedingte Stichwort-Regel: für Kunden mit StichwortTag "Mitglied" ist die Lieferoption mit dem Stichwort "Mitglied" sichtbar

Nur die Mitglieder können sich also dafür entscheiden, ihre Einkäufe persönlich abzuholen.

### Zahlungsarten anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Zahlungsarten für bestimmte Kunden gezielt verfügbar oder nicht verfügbar machen.

{% hint style="info" %}
Diese Stichwort-Regel kann nützlich sein, wenn Sie nur Mitgliedern die Möglichkeit bieten möchten, bei Abholung bar zu bezahlen (Nichtmitglieder aber im Voraus per Karte oder PayPal), oder wenn Sie Ihren Großhandelskunden nur die Möglichkeit bieten möchten, per BACS zu bezahlen.
{% endhint %}

Damit diese bedingte Stichwort-Regel funktioniert, müssen Sie zunächst den Kunden und die Zahlungsart mit demselben Stichwort versehen. Um ein Stichwort auf eine [Zahlungsart](../payment-methods.md) anzuwenden, gehen Sie zu Unternehmen-> Einstellungen -> Zahlungsarten und wählen Sie Bearbeiten.

![](../../../.gitbook/assets/tagspayment.jpg)

In diesem Beispiel wurde die Zahlungsart "Bargeld" den Kunden mit dem Stichwort "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Stichwort-Regel: Zahlungsmittel mit dem Stichwort "Mitglied" sind unsichtbar
* eine bedingte Stichwort-Regel: für Kunden mit dem Stichwort "Mitglied" ist die Zahlungsart mit dem Stichwort "Mitglied" sichtbar

So können nur Mitglieder ihre Einkäufe bei der Abholung bar bezahlen.

### Bestellzyklen in meinem Schaufenster anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Bestellzyklen nur für bestimmte Kunden sichtbar machen.

{% hint style="info" %}
Diese Stichwort-Regel kann nützlich sein, wenn Sie zwei Bestellzyklen gleichzeitig öffnen möchten, denen jeweils unterschiedliche Unternehmensgebühren zugeordnet sind. Ein Zyklus könnte beispielsweise für Großhandelskunden bestimmt sein, die Waren in großen Mengen und mit niedrigeren Unternehmensgebühren kaufen, während der andere für die Öffentlichkeit sichtbar wäre und Produkte in kleineren Mengen, aber mit einer höheren Gewinnspanne auflisten würde.
{% endhint %}

Damit diese Regel funktioniert, müssen Sie den Kunden und den Bestellzyklus mit demselben Stichwort versehen haben. Um einen Bestellzyklus zu kennzeichnen, sehen Sie sich die Registerkarte "Stichwörter" im Abschnitt "Ausgehende Produkte" eines Bestellzyklus an (Seite 3 des [Bestellzyklus](../order-cycle/order-cycles-for-hubs.md#3-ausgehende-produkte)).

![](../../../.gitbook/assets/tagsorder.jpg)

In diesem Beispiel wurde der obige Bestellzyklus den Kunden mit dem Stichwort "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Stichwort-Regel: Bestellzyklen mit dem Stichwort "Mitglied" sind unsichtbar
* eine bedingte Stichwort-Regel: für Kunden mit dem Stichwort "Mitglied" ist ein Bestellzyklus mit dem Stichwort "Mitglied" sichtbar

Somit können nur Mitglieder Waren aus diesem Bestellzyklus erwerben.

## Kundenspezifische Preisgestaltung

Manchmal möchten unsere Nutzer unterschiedliche Preise für verschiedene Kunden berechnen, oft auf der Grundlage ihres Status als Mitglied oder Nicht-Mitglied (oder Großhändler oder Einzelhändler). Derzeit gibt es keine Möglichkeit, automatisch unterschiedliche Preise für Mitglieder und Nicht-Mitglieder zu berechnen, aber es gibt einige Umwege, um das Gleiche zu erreichen.

Sie können die **Kundenkennzeichnung mit Stichwort-Regeln** verwenden, um dies zu erreichen:

* Machen Sie bestimmte [Varianten](tags-and-tag-rules.md#varianten-in-meinem-schaufenster-anzeigen-oder-ausblenden) nur für bestimmte Kundengruppen verfügbar: z. B. "Großeinkäufe" zu einem reduzierten Preis pro Gewicht, die nur für Kunden mit einer Großhandels-Kennzeichnung erhältlich sind.
* Führen Sie mehr als einen [Bestellzyklus](tags-and-tag-rules.md#bestellzyklen-in-meinem-schaufenster-anzeigen-ausblenden) gleichzeitig aus, wobei nur Mitglieder (oder Großhandelskunden) den Bestellzyklus mit einer niedrigeren Unternehmensgebühr einsehen und daraus kaufen können.
* Sie könnten die Gebühren für die [Lieferoption](tags-and-tag-rules.md#versandmethoden-anzeigen-ausblenden) verwenden, um unterschiedliche Preise für verschiedene Kunden zu berechnen. Um sicherzustellen, dass nur Mitglieder den ermäßigten "Mitgliedertarif" wählen, müssen Sie dieser Lieferoption ein Stichwort hinzufügen (sonst könnte jeder "schummeln" und den günstigeren Versandtarif wählen).
* Wenn Sie eine [Zahlungsart](tags-and-tag-rules.md#zahlungsarten-anzeigen-ausblenden), nämlich Barzahlung bei Abholung, nur Mitgliedern zur Verfügung stellen, würden Sie einen Aufschlag auf alle anderen Zahlungsmethoden erheben, so dass Nicht-Mitglieder mehr für ihre Waren bezahlen müssen.

{% hint style="info" %}
Abgesehen von der Verwendung von Stichwörtern entscheiden sich einige Unternehmen dafür, zwei Hubs einzurichten: einen nur für Großhandelskunden/Mitglieder (siehe [Privates Schaufenster](https://guide.openfoodnetwork.org/deutsch/basic-features/shopfront/private-shopfront)) und einen für alle anderen.

Mit der [Inventarisierungsfunktion](../../products-1/inventory-tool.md) können die beiden Shops die gleichen Produkte anbieten, aber Sie können die Preise für jeden Shop unabhängig voneinander festlegen.

Diese Methode bietet die größte Flexibilität: Die Preise können von Fall zu Fall auf die einzelnen Kundengruppen abgestimmt werden, anstatt einen pauschalen prozentualen oder festen Preisunterschied festzulegen.
{% endhint %}
