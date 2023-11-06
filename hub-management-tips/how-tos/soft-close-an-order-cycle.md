# Soft Close eines Auftragszyklus

Von Zeit zu Zeit kann es vorkommen, dass in Ihrem Unternehmen mehr Aufträge eingehen, als Sie physisch bearbeiten können (z. B. während der Panikkäufe im März 2020 oder zu Weihnachten).

{% hint style="success" %}
Es ist immer besser, die Grenzen Ihres Geschäfts zu kennen und Ihren Auftragszyklus frühzeitig zu schließen, als zu viel zu verkaufen und dann die Kunden enttäuschen zu müssen.
{% endhint %}

Produkte verschwinden aus Ihrem Shop, wenn[ ihr Lagerbestand auf Null sinkt](../../basic-features/products-1/), aber es kann eine Grenze für die Anzahl der Bestellungen geben, die Sie innerhalb des Zeitrahmens Ihrer Versandmethoden verpacken und ausliefern können, und diese wird nicht allein durch den Lagerbestand berücksichtigt (die Bearbeitung von 100 Bestellungen, die jeweils einen Artikel enthalten, dauert länger als eine Bestellung mit 100 Artikeln).

{% hint style="danger" %}
Wenn Sie das Enddatum und die Endzeit eines [Bestellzyklus](../../basic-features/shopfront/order-cycle/) auf die aktuelle Uhrzeit ändern, bedeutet dies, dass Kunden, die sich in der Abmeldephase befinden, ihre Bestellungen nicht erhalten.
{% endhint %}

Daher empfehlen wir die folgende Methode - auf diese Weise werden die Bestellungen von Kunden, die zu diesem Zeitpunkt bezahlen, trotzdem angenommen, während andere Bestellungen nicht angenommen werden.

## Prozess

* Ihr Unternehmen kann 100 Aufträge pro Woche bearbeiten - das ist das absolute Maximum.
* Die Seite mit den [Aufträgen für Ihr Angebot](../../basic-features/orders/view-orders.md#auflistung-der-auftraege) zeigt an, dass Sie in diesem Auftragszyklus 95 Aufträge erhalten haben und noch 2 Tage Zeit haben.

{% hint style="info" %}
Gehen Sie in Ihrem Verwaltungsbereich auf "Bestellungen" und filtern Sie die Ergebnisse nach Händler und Bestellzyklus (unten grün hervorgehoben). Die Anzahl der eingegangenen Bestellungen wird unter der Überschrift "Filterergebnisse" angezeigt (rot hervorgehoben).
{% endhint %}

![](../../.gitbook/assets/orders.jpg)

* Fügen Sie eine neue [Standard-Tag-Regel](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) hinzu, indem Sie **Unternehmen -> Einstellungen -> Tag-Regeln** aufrufen.\
  Standard: Auftragszyklen mit der Kennzeichnung "**Geschlossen**" sind nicht sichtbar.

![](../../.gitbook/assets/closedtagrule.jpg)

\
Weitere Tag-Regeln sind nicht erforderlich.

* Bearbeiten Sie den derzeit offenen [Auftragszyklus](../../basic-features/shopfront/order-cycle/order-cycles-for-hubs.md) und fügen Sie auf Seite 3 ("Ausgehende Produkte") die Markierung "Geschlossen" hinzu.

![](../../.gitbook/assets/softcloseoc.jpg)

**Aktualisieren** Sie und Ihr Bestellzyklus wird geschlossen, ohne dass die Kunden beim Auschecken gestört werden.

{% hint style="danger" %}
Dieses Verfahren ist derzeit nur für Unternehmen möglich, die als Drehscheibe registriert sind.
{% endhint %}
