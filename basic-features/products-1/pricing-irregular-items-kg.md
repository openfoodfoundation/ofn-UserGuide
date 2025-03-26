# Preisgestaltung Fleisch und andere "vollständige" Produkte mit unbekanntem Gewicht

Hier bezeichnen wir Produkte als "**unregelmäßig**", wenn sie nach Gewicht/Volumen verkauft werden, die genaue Menge aber erst zum Zeitpunkt der Ernte/Verteilung bekannt ist.

Zum Beispiel Fleischstücke, Käsescheiben, großes Gemüse.

Auf der OFN-Plattform stehen verschiedene Tools zur Verfügung, um diese Verkäufe zu verwalten und zu organisieren.

## Option eins: Festsetzung eines Durchschnittsgewichts/-preises und Erstattung

Sie können den Durchschnittspreis des Produkts in Rechnung stellen und dem Kunden einen Aufschlag erstatten oder berechnen, wenn das tatsächliche Gewicht vom Mittelwert abweicht.

Wenn Sie das tatsächliche Gewicht der Produkte kennen (z. B. wenn Sie Bestellungen für die Abholung durch Kunden vorbereiten), melden Sie sich bei der Massenbestellungsverwaltung an (Bestellungen -> Massenbestellungsverwaltung) und fügen Sie der Tabelle die Spalte Gewicht/Volumen hinzu.

![](../../.gitbook/assets/bom1.jpg)

Sie können dann das für jeden Käufer angezeigte Gewicht für eine bestimmte Bestellung und ein bestimmtes Produkt ändern. Der Preis wird automatisch entsprechend der eingegebenen Menge neu berechnet.

{% hint style="info" %}
Vergessen Sie nicht, dem Kunden eine erneute Auftragsbestätigung per E-Mail zu schicken, um ihn über die Preisdifferenz und die eventuell noch ausstehenden Beträge zu informieren.
{% endhint %}

## Option Zwei: Anzeige von Preisspannen&#x20;

Gleiche Logik wie bei Option eins, aber statt eines Durchschnittspreises am Anfang wird einfach eine Preisspanne angegeben. Diese Lösung hat den Vorteil, dass sie dem Käufer deutlich signalisiert, dass der Endpreis wahrscheinlich geändert werden wird.&#x20;

Es können auch [Varianten](product-variants.md) verwendet werden, um verschiedene Sortimente zu schaffen.

> **Beispiel 1** (ein Produkt und eine Variante):\
> Produkt = Hähnchen (zwischen 8 und 12 kg mit Preis je nach Gewicht, CHF 10 / kg)
>
> **Beispiel 2** (zwei Varianten für ein Produkt):\
> Produkt = Huhn (CHF 10 / kg)
>
> Variante 1 = kleines Huhn (zwischen 8 und 12 kg, Preis nach tatsächlichem Gewicht)&#x20;
>
> Variante 2 = großes Huhn (zwischen 13 und 20 kg, Preis nach tatsächlichem Gewicht)

## Option Drei: Varianten mit Festpreisen erstellen&#x20;

Eine etwas einfachere Version von Option zwei besteht darin, Varianten für Ihre Produkte auf der Grundlage von Gewichtsspannen zu erstellen, aber einen **Festpreis** für alle Artikel zu berechnen, die in diese Spanne fallen.\
Wenn z. B. Butternusskürbis CHF 1/kg kostet, könnten Sie die Varianten mit den folgenden Festpreisen auflisten:

* Klein (0,7 - 0,9 kg) CHF 0.80
* Mittel (0,9 - 1,1 kg) CHF 1.00
* Groß (1,1 - 1,3 kg) CHF 1.20
* Extra groß (1,3 - 1,5 kg) CHF 1.40

## Option Vier: Varianten mit bekannten Gewichten erstellen

Wenn Sie z.B. das Gewicht aller Ihrer Steaks im Voraus kennen, können Sie die Variantenfunktion nutzen, um direkt den genauen Preis für jeden Artikel anzuzeigen. Beispiel:

![](../../.gitbook/assets/bom2.jpg)

## Bearbeiten von Aufträgen&#x20;

Für Fleischproduzenten kann es schwierig sein, im Voraus über die Verfügbarkeit von Produkten Bescheid zu wissen oder ihre Verpackungen entsprechend vorzubereiten. (Bis zur Schlachtung ist das Gewicht eines Huhns oder einer Lammkeule vielleicht nicht bekannt).

Dies stellt kein Problem dar, da Bestellungen bei Bedarf geändert werden können (durch Hinzufügen, Ändern oder Löschen von Produkten). Weitere Informationen finden Sie unter [Bestellungen](../orders/).

## Erstattung oder Verrechnung der Differenz an die Kunden: Wie funktioniert das?&#x20;

Wenn ein Kunde **seine Waren bei der Abholung** oder Lieferung **bezahlt**, kann der Hub-Manager die Bestellung vor der Zahlung entsprechend dem tatsächlichen Gewicht und den tatsächlich gelieferten Produkten ändern. Daher besteht in diesem Fall keine Notwendigkeit, dem Kunden die Kosten zu erstatten oder erneut in Rechnung zu stellen.

Wenn eine Bestellung vor der Lieferung online bezahlt wird, müssen Sie die Differenz zwischen den bereits erhaltenen Beträgen und den für die zu liefernden Produkte geschuldeten Beträgen erstatten oder in Rechnung stellen. Klicken Sie hier, um zu sehen, [wie](../orders/refunds-and-adjusting-payments.md).

{% hint style="danger" %}
Eine Alternative ist die Verwendung eines Online-Zahlungssystems, das den Betrag vorübergehend als "ausstehend" speichert, bis die Bestellung bestätigt wurde.

_Diese Funktion ist in Open Food Network noch nicht implementiert. Wir arbeiten auch an der automatischen Implementierung von "Gutschriften", die es einem Hub ermöglichen, in Form einer Gutschrift zu erstatten, die vom Kunden als Teilzahlung für seine nächste Bestellung verwendet werden kann._
{% endhint %}

## Informieren Sie den Käufer über Ihre Preispolitik&#x20;

Sie können Ihre Kunden über Ihre Preispolitik für Artikel mit variablem Gewicht (z. B. Fleisch) in dem [Nachrichtenfeld](../enterprise-profile/enterprise-settings.md#shop-einstellungen) informieren, das oben auf Ihrer Shop-Front angezeigt wird. Sie finden diese Funktion unter Unternehmenseinstellungen -> Shop-Einstellungen.

Es könnte sinnvoll sein, einen Hinweis auf diese Preispolitik in das Beschreibungsfeld der [Zahlungsarten](../shopfront/payment-methods.md) aufzunehmen. Zum Beispiel könnten Sie hinzufügen: "Beachten Sie, dass der Endpreis je nach Gewicht um 10 % variieren kann, wenn Sie nicht teilbare Artikel wie Fleisch oder großes Gemüse gekauft haben.".
