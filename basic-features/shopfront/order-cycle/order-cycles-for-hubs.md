# Bestellzyklen (für Hubs)

{% hint style="warning" %}
Lesen Sie weiter, wenn Sie das Unternehmenspaket '[Laden](../../../your-quick-start-on-ofn-given-who-you-are.md#produzentenladen)' gewählt haben.

Besuchen Sie diese [Seite](order-cycles-for-producers.md), wenn Sie sich als '[Produzentenladen](../../../your-quick-start-on-ofn-given-who-you-are.md#laden)' registriert haben und einen Bestellzyklus für Ihre Schaufensterfront einrichten möchten.
{% endhint %}

Sie eröffnen Ihren Hub, indem Sie einen Bestellzyklus erstellen. Wenn Sie einen Bestellzyklus erstellen, wählen Sie aus, wann Ihr Hub geöffnet ist (von und bis), welche Produkte in den Hub aufgenommen werden und welche Gebühren Sie erheben möchten.

**Warum in Bestellzyklen bestellen?**  \
Einige Hubs möchten vielleicht einen ständig geöffneten Online-Shop haben und die Bestellungen einzeln nach Eingang bearbeiten. Viele Hubs arbeiten jedoch mit einem periodischen Bestellsystem, das es ihnen ermöglicht, Aufträge in großen Mengen zu bearbeiten, was ihre Produktions-, Verpackungs- und Vertriebsaktivitäten effizienter macht (und die damit verbundenen Gemeinkosten senkt).

Ein Bestellzyklus kann zum Beispiel zwei Wochen lang offen sein. Am Ende der zwei Wochen werden alle Bestellungen verpackt und am folgenden Mittwoch zur gleichen Zeit ausgeliefert. Sobald dieser Stapel von Bestellungen ausgeliefert wurde, kann ein neuer Bestellzyklus eröffnet werden.

Eine kurze Demonstration der Einrichtung eines neuen Bestellzyklus:

![](../../../.gitbook/assets/ordercyclehub.gif)

## Bestellzyklen anzeigen

Sie können einen Bestellzyklus erstellen und frühere Bestellzyklen einsehen, indem Sie in Ihrem [Dashboard](../../dashboard.md) auf Bestellzyklen verwalten klicken.

![](../../../.gitbook/assets/ordercycledash.jpg)

Oder über das horizontale Menü am oberen Rand der Seite.

![](<../../../.gitbook/assets/ordercycle1 (2) (2) (2).jpg>)

{% hint style="warning" %}
Sie können erst dann einen laufenden Bestellzyklus veröffentlichen, wenn Sie mindestens eine [Zahlungs](../payment-methods.md)- und [Versandmethode](../shipping-methods.md) für Ihr Unternehmen eingerichtet haben.
{% endhint %}

## Einen neuen Bestellzyklus erstellen

Der erste Schritt besteht darin, einen Koordinator für Ihren Bestellzyklus auszuwählen. Nur das Unternehmen, das einen Bestellzyklus koordiniert, ist berechtigt, **alle** Aspekte des Bestellzyklus zu ändern und zu verwalten. Andere Unternehmen, die an einem Bestellzyklus beteiligt sind (nur als Lieferanten oder Händler), haben nur eingeschränkten Zugriff.\
Weitere Informationen zum unternehmensübergreifenden Management im Rahmen von Bestellzyklen finden Sie [hier](permissions-in-multi-enterprise-order-cycles.md).

![](../../../.gitbook/assets/ordercycle2.jpg)

Nach der Auswahl des Koordinators für den Bestellzyklus ist der Einrichtungsprozess in drei Schritte unterteilt:

### 1) Allgemeine Einstellungen

![](<../../../.gitbook/assets/ordercycle3 (1).jpg>)

**Name (erforderlich):** Geben Sie dem Bestellzyklus einen für Sie aussagekräftigen Namen. Wir empfehlen Ihnen, ein einheitliches Namensprotokoll zu verwenden, z. B. FoodHub\_Woche27\_2014. Wir empfehlen Ihnen auch, den Namen Ihres Hubs in den Namen des Bestellzyklus aufzunehmen, damit der OFN-Support Ihre Bestellzyklen identifizieren kann, falls Sie Hilfe benötigen.

**Bestellungen öffnen um:** Dies ist das Datum und die Uhrzeit, zu der Ihr OFN-Hub geöffnet und sichtbar ist und Bestellungen von Kunden annimmt.

**Bestellungen schließen:** Dies ist das Datum (und die Uhrzeit), an dem Ihr OFN-Hub schließt und keine Bestellungen mehr annimmt. Wenn Sie beabsichtigen, einen Bestellzyklus zu haben, der ständig geöffnet ist, wählen Sie ein Schließungsdatum, das weit in der Zukunft liegt.

**Zeitpläne:** Leer lassen, es sei denn, Sie verwenden [Abonnements](../../subscriptions/).

**Koordinator-Gebühr hinzufügen:** Als Hub sind Sie höchstwahrscheinlich der Koordinator. Hier können Sie Ihre Unternehmensgebühr anwenden, die als Aufschlag dient. Die Gebühr wird anhand des unter Unternehmensgebühren ausgewählten Rechners berechnet. Sie können nur eine [Unternehmensgebühr](../enterprise-fees.md) anwenden, die zuvor erstellt wurde.

### 2) Eingehende Produkte

![](../../../.gitbook/assets/ordercycle4.jpg)

Auf dieser Seite können Sie die Produzenten und ihre Produkte auswählen, die in diesem Bestellzyklus verfügbar sein sollen. Im Dropdown-Menü sehen Sie alle Produzenten, die Ihnen die Erlaubnis erteilt haben, ihre Produkte zu Ihrem Bestellzyklus hinzuzufügen (siehe Abschnitt [Unternehmensberechtigungen](https://guide.openfoodnetwork.org/deutsch/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es)).\
Nachdem Sie einen Lieferanten ausgewählt und auf **Lieferant hinzufügen** geklickt haben, werden alle mit diesem Lieferanten verbundenen Produkte angezeigt. Markieren Sie die Produkte, die Sie dem Hub hinzufügen möchten, oder klicken Sie auf **Alle auswählen**.

{% hint style="info" %}
Produkte, die nicht vorrätig sind (d.h. deren "auf Lager"-Wert gleich Null ist), sind in dieser Liste enthalten. Wenn sie zu einem Bestellzyklus hinzugefügt werden, erscheinen sie nicht auf der Startseite unseres Shops. Es ist immer gut, die Lagerbestände zu überprüfen.
{% endhint %}

Das Feld **Empfangsdetails** ist optional. Die in dieses Feld eingegebenen Informationen werden automatisch in jede E-Mail eingefügt, die am Ende eines Bestellzyklus an die Erzeuger gesendet wird (nachdem Sie auf "Erzeuger benachrichtigen" geklickt haben). Es könnte eine gute Idee sein, hier eine genaue Lieferadresse für die Produkte vor der Verteilung an die Kunden anzugeben.

Mit der Schaltfläche "**Gebühr hinzufügen**" können Sie den verschiedenen Anbietern unterschiedliche [Unternehmensgebühren](../enterprise-fees.md) zuweisen. Zum Beispiel kann der Transport von Mehl oder schweren Gütern zu den Kunden für einen Hub teurer sein als für Salat. Daher kann ein Hub auf transparente Weise eine etwas höhere Unternehmensgebühr auf alle vom Mehlmüller gelieferten Waren aufschlagen als der Salatbauer.

Wählen Sie den Namen des Unternehmens in der ersten Dropdown-Box und klicken Sie dann auf den Namen der Unternehmensgebühr in der zweiten Dropdown-Box. Im folgenden Beispiel wird eine Unternehmensgebühr mit dem Namen OrderAdmin auf den Erzeuger von Obst angewandt.

![Apply enterprise fee to incoming supplier](../../../.gitbook/assets/enterprise-fee.png)

{% hint style="warning" %}
Diese Gebühr wird auf alle gekauften Erzeugnisse des Obsterzeugers erhoben. Die Gebühr wird anhand des Gebührenrechners berechnet, der bei der Erstellung der [Unternehmensgebühr](../enterprise-fees.md) ausgewählt wurde.
{% endhint %}

### 3) Ausgehende Produkte

Hier können Sie einen oder mehrere Hub-Vertriebspartner auswählen. Alle Hubs, die in diesem Bestellzyklus als Händler ausgewählt werden, haben für die Dauer des Bestellzyklus eine offene Schaufensterfront.\
In einem **einfachen Modell** ist nur ein Hub als einziger Händler für den Bestellzyklus aufgeführt. Wählen Sie den Hub aus, und markieren Sie das Kästchen "Alle auswählen", um alle eingehenden Produkte zur Shopfront hinzuzufügen.\
Für mehr Flexibilität kann derselbe **Bestellzyklus mehrere Hub-Vertriebspartner** haben. In diesem Fall möchten Sie vielleicht für jeden Verteiler eine andere Teilmenge der verfügbaren eingehenden Produkte auswählen und/oder für jeden Verteiler unterschiedliche Liefertermine hinzufügen.

![](../../../.gitbook/assets/oc3.jpg)

In der Spalte **Stichwörter** können Sie Ihre Auftragszyklen kennzeichnen, um festzulegen, ob sie für bestimmte Kunden sichtbar oder unsichtbar sind. Weitere Informationen finden Sie unter [Stichwörter und Stichwort-Regeln](../customer-management-and-conditional-displays-prices/tags-and-tag-rules.md).

**Bereit für (d.h. Datum/Uhrzeit)" (erforderlich):** In diesem Feld wird dem Kunden mitgeteilt, wann seine Bestellung entweder zur Abholung oder zur Lieferung bereit ist. Wenn es sich bei Ihrem Bestellzyklus um einen immerwährenden Zyklus handelt, bei dem Aufträge auf individueller Basis und nicht in großen Mengen ausgeführt werden, sollten Sie etwas wie "Zwei Tage nach Auftragseingang" eingeben. Das nachstehende Beispiel zeigt, wie ein Kunde zwischen verschiedenen Auftragszyklen wechseln kann, um das für ihn am besten geeignete Datum auszuwählen.

![](../../../.gitbook/assets/multipleoc3.jpg)

{% hint style="info" %}
Wenn Sie mit einer ständig geöffneten Ladenfront arbeiten (d.h. Sie haben das Datum für den Abschluss des Bestellzyklus auf mehr als 3 Monate im Voraus festgelegt), dann wird das blaue Feld "Bereit für" auf Ihrer Ladenfront den Text "Bestellungen sind derzeit offen" anzeigen.
{% endhint %}

Der Hinweis wird auch an der Kasse angezeigt, wenn der Kunde seine Versandart auswählt (siehe unten), und ist in der E-Mail zur Bestellbestätigung enthalten.

![](../../../.gitbook/assets/readyfor2.jpg)

Die Nachricht mit den **Abholanweisungen** wird in der Bestellbestätigungs-E-Mail des Kunden unter der Nachricht für die von ihm gewählte Versandart eingefügt (siehe unten). Dieser Hinweis ist nur für den Kunden sichtbar, so dass Sie auch sensiblere Informationen wie Adressen, Telefonnummern usw. angeben können. Unten sehen Sie ein Beispiel für eine Bestellbestätigungs-E-Mail.

![collection details message](../../../.gitbook/assets/collection-details.png)

**Gebühr hinzufügen:** Auch diesem Verteiler kann eine zuvor erstellte Unternehmensgebühr zugewiesen werden. Bei einfachen Modellen (mit einem Hub-Vertriebspartner, der auch der Koordinator des Bestellzyklus ist) ist das Hinzufügen einer Gebühr in diesem Stadium dasselbe wie das Hinzufügen einer "Koordinatorgebühr" (sie gilt für alle Produkte). Bei komplexen Modellen kann der Koordinator für alle Produkte, die über jeden Vertriebshändler verkauft werden, unterschiedliche Gebühren festlegen. Diese Funktion lässt sich am besten hier implementieren.

### Öffnen Sie das Schaufenster

Klicken Sie auf **Speichern**, um den Bestellzyklus zu planen. Wenn das Eröffnungsdatum bereits überschritten ist, ist Ihr Shop sofort geöffnet! Wenn Sie nicht sofort eröffnen wollen, geben Sie Termine in der Zukunft ein, die Sie später ändern können.

Für periodische, sich wiederholende Bestellzyklen können Sie einen bestehenden Bestellzyklus kopieren und die Daten ändern, um den Prozess zu beschleunigen. Siehe unten.

![](../../../.gitbook/assets/occpy.jpg)

Bestellzyklen werden grün angezeigt, wenn sie aktiv sind, gelb, wenn sie für ein zukünftiges Datum geplant sind, und grau, wenn sie geschlossen wurden. Wenn ein Bestellzyklus vor mehr als einem Monat geschlossen wurde, wird er in dieser Liste nicht mehr angezeigt. Um alle Ihre vergangenen Bestellzyklen zu sehen, klicken Sie oben in der Liste auf "Mehr anzeigen".

## Schaltfläche "Produzenten benachrichtigen

Wenn Sie diese Schaltfläche oben auf der Seite verwenden, erhalten alle mit dem Bestellzyklus verbundenen Produzenten eine E-Mail mit einer Liste der bisher bestellten Produkte für diesen Bestellzyklus.

![](../../../.gitbook/assets/notifyproducers.jpg)

Wenn Sie die Schaltfläche Produzenten benachrichtigen auswählen, erscheint eine Bestätigungsaufforderung. Sobald diese bestätigt ist, wird automatisch eine E-Mail an alle betroffenen Produzenten gesendet. Die E-Mail enthält Lieferanweisungen (wenn dieses Feld im Abschnitt "Eingehende Produkte" ausgefüllt ist) sowie die folgenden Produktinformationen:

* SKUs (falls relevant)
* Name des Lieferanten
* Name des Produkts
* Bestellte Menge
* Preis pro Einheit
* Zwischensumme pro Produkt
* Eingeschlossene Steuer (falls zutreffend)\


## Hersteller-/Lieferantenberichte

Wenn Ihr Bestellzyklus Produkte von verknüpften Herstellern/Lieferanten enthält, können diese sich in ihr OFN-Konto einloggen und [Berichte](../../reports/) über den Bestellzyklus einsehen. Standardmäßig können sie in diesen Berichten keine Kundendetails sehen. Wenn Sie möchten, dass Ihre Lieferanten in ihren Berichten auf Kundennamen zugreifen können, können Sie diese Einstellungen in den Shop-Präferenzen in Ihren [Unternehmenseinstellungen](../../enterprise-profile/enterprise-settings.md) anpassen.
