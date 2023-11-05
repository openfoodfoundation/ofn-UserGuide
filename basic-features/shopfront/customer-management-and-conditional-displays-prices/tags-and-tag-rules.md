# Tags und Tag-Regeln

Sobald die Kunden in Kategorien mit Tags gruppiert wurden, können Sie ihr Einkaufserlebnis auf folgende Weise anpassen:

* Bestimmte Varianten sichtbar/unsichtbar machen
* Making certain shipping methods visible/invisible
* Bestimmte Zahlungsarten sichtbar/unsichtbar machen
* Auftragszyklen sichtbar/unsichtbar machen

Meistens wird diese Funktion von Unternehmen benötigt, die unterschiedliche Shop-Konfigurationen für Mitglieder/Nicht-Mitglieder oder unterschiedliche Kundengruppen wie Groß-/Einzelhandelskunden haben. Weitere Beispiele finden Sie in unserem Abschnitt [How To](../../../hub-management-tips/how-tos/).

## Wie man eine Tag-Regel einrichtet

Um auf Tag-Regeln zuzugreifen, gehen Sie zu Unternehmen -> Einstellungen -> Tag-Regeln

![](../../../.gitbook/assets/newtagrule1.jpg)

## Standardmäßig

Standardmäßig sind **alle Artikel** für **alle Kunden** sichtbar, unabhängig davon, ob sie markiert sind oder nicht. Sie können die Standard-Anzeigeregeln ändern, indem Sie **+neue Standardregel** hinzufügen wählen. Im folgenden Beispiel sind standardmäßig alle Bestellzyklen, die mit "Großhandel" gekennzeichnet sind, unsichtbar. (In diesem Beispiel können nur die Kunden, die mit dem Etikett "Großhandelskunde" gekennzeichnet sind, die Bestellzyklen mit dem Etikett "Großhandel" sehen (und folglich dort einkaufen).

![](../../../.gitbook/assets/defaulttag.jpg)

## Tag-Regeln

Sobald Sie Standardregeln definiert haben, können Sie für bestimmte Kundengruppen Ausnahmen von diesen Regeln einrichten.

* Definieren Sie zunächst die Kundengruppe, für die die Ausnahme gelten soll. Im obigen Beispiel wurde die Ausnahme auf alle Kunden mit dem Tag "Großhandelskunde" angewendet.
* Dann können Sie für diese Kundengruppe eine von vier Möglichkeiten wählen, ihr Einkaufserlebnis individuell zu gestalten:

![](../../../.gitbook/assets/rule-typess.png)

{% hint style="warning" %}
Denken Sie daran, die entsprechenden Tags zu Varianten, Versand- oder Zahlungsarten oder Bestellzyklen sowie zu Kunden hinzuzufügen, nachdem Sie eine Standard- oder bedingte Tag-Regel eingerichtet haben!
{% endhint %}

Im Folgenden werden wir jede Option einzeln betrachten:

### Varianten in meinem Schaufenster anzeigen oder ausblenden

Mit dieser Regel können Sie bestimmte Varianten für markierte Kunden sichtbar/unsichtbar machen. Damit diese Regel funktioniert, müssen Sie den Kunden und die Produktvariante **in Ihrem Bestand** (nicht in der Produktliste des Herstellers) mit demselben Tag versehen haben.

Im folgenden Beispiel wurde die 1 kg-Variante von delux muesli mit dem Tag "Mitglied" versehen. Es wäre also möglich, Tag-Regeln so einzurichten, dass standardmäßig nur die kleinere (nicht getaggte) 500-g-Variante des Delux-Müslis auf der Shop-Front erscheint, es sei denn, der Kunde gehört zu einer Gruppe von Käufern, die alle mit dem Tag "Mitglied" versehen sind (in diesem Fall würde er auch die 1 kg-Variante sehen können).

![](<../../../.gitbook/assets/varianttags (1).jpg>)

### Versandmethoden anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Versandmethoden für bestimmte Kunden spezifisch verfügbar oder nicht verfügbar machen. Damit diese Regel funktioniert, müssen Sie den Kunden und die Versandmethode mit demselben Tag versehen haben. Um eine Versandart zu kennzeichnen, gehen Sie zu [Versandart](../shipping-methods.md) **bearbeiten** und wenden Sie die entsprechende Kennzeichnung an.

![](../../../.gitbook/assets/tagshipping.jpg)

In diesem Beispiel wurde die Versandart "Selbstabholung" den Kunden mit dem Tag "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Tag-Regel: Versandmethoden mit dem Tag 'Mitglied' sind unsichtbar
* eine bedingte Tag-Regel: für Kunden mit dem Tag 'Mitglied' ist die Versandmethode mit dem Tag 'Mitglied' sichtbar

Nur die Mitglieder können sich also dafür entscheiden, ihre Einkäufe persönlich abzuholen.

### Zahlungsarten anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Zahlungsmethoden für bestimmte Kunden gezielt verfügbar oder nicht verfügbar machen.

{% hint style="info" %}
Diese Tag-Regel kann nützlich sein, wenn Sie nur Mitgliedern die Möglichkeit bieten möchten, bei Abholung bar zu bezahlen (Nichtmitglieder aber im Voraus per Karte oder PayPal), oder wenn Sie Ihren Großhandelskunden nur die Möglichkeit bieten möchten, per BACS zu bezahlen.
{% endhint %}

Damit diese bedingte Tag-Regel funktioniert, müssen Sie zunächst den Kunden und die Zahlungsmethode mit demselben Tag versehen. Um ein Tag auf eine [Zahlungsmethode](../payment-methods.md) anzuwenden, gehen Sie zu Unternehmen-> Einstellungen -> Zahlungsmethoden und wählen Sie Bearbeiten.

![](../../../.gitbook/assets/tagspayment.jpg)

In diesem Beispiel wurde die Zahlungsmethode "Bargeld" den Kunden mit dem Tag "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Tag-Regel: Zahlungsmittel mit dem Tag "Mitglied" sind unsichtbar
* eine bedingte Tag-Regel: für Kunden mit dem Tag "Mitglied" ist die Zahlungsmethode mit dem Tag "Mitglied" sichtbar

So können nur Mitglieder ihre Einkäufe bei der Abholung bar bezahlen.

### Bestellzyklen in meinem Schaufenster anzeigen/ausblenden

Mit dieser Regel können Sie bestimmte Auftragszyklen nur für bestimmte Kunden sichtbar machen.

{% hint style="info" %}
Diese Tag-Regel kann nützlich sein, wenn Sie zwei Bestellzyklen gleichzeitig öffnen möchten, denen jeweils unterschiedliche Unternehmensgebühren zugeordnet sind. Ein Zyklus könnte beispielsweise für Großhandelskunden bestimmt sein, die Waren in großen Mengen und mit niedrigeren Unternehmensgebühren kaufen, während der andere für die Öffentlichkeit sichtbar wäre und Produkte in kleineren Mengen, aber mit einer höheren Gewinnspanne auflisten würde.
{% endhint %}

Damit diese Regel funktioniert, müssen Sie den Kunden und den Auftragszyklus mit demselben Tag versehen haben. Um einen Auftragszyklus zu kennzeichnen, sehen Sie sich die Registerkarte "Tags" im Abschnitt "Ausgang" eines Auftragszyklus an (Seite 3 des [Auftragszyklus](../order-cycle/order-cycles-for-hubs.md#3-ausgehende-produkte)).

![](../../../.gitbook/assets/tagsorder.jpg)

In diesem Beispiel wurde der obige Auftragszyklus den Kunden mit dem Tag "Mitglied" zugewiesen. Man könnte dann Folgendes einrichten:

* eine Standard-Tag-Regel: Auftragszyklen mit dem Tag "Mitglied" sind unsichtbar
* eine bedingte Tag-Regel: für Kunden mit dem Tag "Mitglied" ist ein Auftragszyklus mit dem Tag "Mitglied" sichtbar

Somit können nur Mitglieder Waren aus diesem Bestellzyklus erwerben.

## Kundenspezifische Preisgestaltung

Manchmal möchten unsere Nutzer unterschiedliche Preise für verschiedene Kunden berechnen, oft auf der Grundlage ihres Status als Mitglied oder Nicht-Mitglied (oder Großhändler oder Einzelhändler). Derzeit gibt es keine Möglichkeit, automatisch unterschiedliche Preise für Mitglieder und Nicht-Mitglieder zu berechnen, aber es gibt einige Umwege, um das Gleiche zu erreichen.

Sie können die **Kundenkennzeichnung mit Tag-Regeln** verwenden, um dies zu erreichen:

* Machen Sie bestimmte [Varianten](tags-and-tag-rules.md#varianten-in-meinem-schaufenster-anzeigen-oder-ausblenden) nur für bestimmte Kundengruppen verfügbar: z. B. "Großeinkäufe" zu einem reduzierten Preis pro Gewicht, die nur für Kunden mit einer Großhandelsmarke erhältlich sind.
* Führen Sie mehr als einen [Bestellzyklus](tags-and-tag-rules.md#bestellzyklen-in-meinem-schaufenster-anzeigen-ausblenden) gleichzeitig aus, wobei nur Mitglieder (oder Großhandelskunden) den Bestellzyklus mit einer niedrigeren Unternehmensgebühr einsehen und daraus kaufen können.
* Sie könnten die Gebühren für die [Versandart verwenden](tags-and-tag-rules.md#versandmethoden-anzeigen-ausblenden), um unterschiedliche Preise für verschiedene Kunden zu berechnen. Um sicherzustellen, dass nur Mitglieder den ermäßigten "Mitgliedertarif" wählen, müssen Sie dieser Versandart eine Kennzeichnung hinzufügen (sonst könnte jeder "schummeln" und den günstigeren Versandtarif wählen).
* Wenn Sie eine [Zahlungsmethode](tags-and-tag-rules.md#zahlungsarten-anzeigen-ausblenden), nämlich Barzahlung bei Abholung, nur Mitgliedern zur Verfügung stellen, würden Sie einen Aufschlag auf alle anderen Zahlungsmethoden erheben, so dass Nicht-Mitglieder mehr für ihre Waren bezahlen müssen.

{% hint style="info" %}
Abgesehen von der Verwendung von Tags entscheiden sich einige Unternehmen dafür, zwei Hubs einzurichten: einen nur für Großhandelskunden/Mitglieder (siehe Front des Private Shop) und einen für alle anderen.

Mit der [Inventarisierungsfunktion](../../products-1/inventory-tool.md) können die beiden Shops die gleichen Produkte anbieten, aber Sie können die Preise für jeden Shop unabhängig voneinander festlegen.

Diese Methode bietet die größte Flexibilität: Die Preise können von Fall zu Fall auf die einzelnen Kundengruppen abgestimmt werden, anstatt einen pauschalen prozentualen oder festen Preisunterschied festzulegen.
{% endhint %}
