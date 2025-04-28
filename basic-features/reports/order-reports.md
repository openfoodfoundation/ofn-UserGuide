# Bestellberichte

## Bericht über Bestellungen und Vertriebspartner

{% hint style="success" %}
Dieser Bericht ist eine nützliche Methode, um Kundenbestellungen detaillierter als in der [Bestellliste](../orders/view-orders.md) zu betrachten.
{% endhint %}

Die Datenfelder, die Sie in diesem Bericht sehen können, sind

* Datum und Uhrzeit der Bestellung zusammen mit der Bestell-ID
* Versandart (und -kosten), Zahlungsart, Kundenhinweise
* Kundenname, E-Mail, Telefonnummer, Stadt (aber keine vollständige Adresse)
* Für jedes Produkt innerhalb einer Bestellung gibt es den Namen des Produkts, den Variantennamen, die Menge (und die maximale Menge bei Großbestellungen), die Kosten
* Adresse des Hubs (Verteiler)

![Orders and Distributors Report](../../.gitbook/assets/orders-and-distributors.jpg)

{% hint style="info" %}
Filtern Sie nach Datum und Uhrzeit, um ein schnelles Herunterladen zu ermöglichen.
{% endhint %}

## Berichte zu Aufträgen und Auftragsabwicklung

Unter Bestellungs- & Erfüllungsberichte finden Sie vier Optionen: Lieferantengesamtsummen, Lieferantengesamtsummen nach Verteilstelle, Verteilstellengesamtsummen nach Lieferanten und Kundengesamtsummen.

### Lieferantengesamtsummen&#x20;

{% hint style="success" %}
Als **Hersteller, der eine oder mehrere Verteilstellen beliefert**, sind diese drei Berichte eine gute Möglichkeit, den Überblick über die Bestellungen Ihrer Produkte zu behalten, die **während eines offenen Auftragszyklus eingehen**.
{% endhint %}

Wenn Sie nicht gleichzeitig der Koordinator oder Verteiler des Bestellzyklus sind, erscheinen diese Aufträge nicht in Ihrer [Auftragsliste](../orders/view-orders.md), aber Sie sollten mit der Planung Ihres Backens/Kommissionierens beginnen, bevor Sie die[ E-Mail mit der Lieferantenbenachrichtigung ](../shopfront/order-cycle/order-cycles-for-hubs.md#notify-producers-button)vom Verteilerzentrum erhalten.

Nachstehend finden Sie eine Zusammenfassung der in den einzelnen Berichten enthaltenen Daten:

| Bericht                 | Lieferantengesamtsummen | Lieferantengesamtsumme nach Verteilstelle | Verteilstellengesamtsummen nach Lieferanten |
| ----------------------- | ----------------------- | ----------------------------------------- | ------------------------------------------- |
| Produzent               | J                       | J                                         | J                                           |
| Hub                     | N                       | J                                         | J                                           |
| Produkt                 | J                       | J                                         | J                                           |
| Variante                | J                       | J                                         | J                                           |
| Betrag                  | J                       | J                                         | J                                           |
| Gesamte Einheiten       | J                       | N                                         | N                                           |
| Aktuelle Einheit Kosten | J                       | J                                         | J                                           |
| Gesamtkosten            | J                       | J                                         | J                                           |
| Status                  | J                       | N                                         | N                                           |
| Versandart              | J                       | J                                         | J                                           |
| Gesamtversandkosten     | N                       | N                                         | J                                           |

{% hint style="warning" %}
Beachten Sie, dass die Gesamtkosten nicht einfach ein Vielfaches der laufenden Kosten pro Einheit und des Betrags sind.&#x20;

* Die aktuellen Kosten pro Einheit können innerhalb des gewählten Zeitrahmens variieren.
* Der in diesen Berichten aufgezeichnete Wert ist der aktuelle Preis pro Einheit zum Zeitpunkt der letzten Bestellung.
* Die Gesamtkosten sind die Summe der Produktkosten zu dem Zeitpunkt, zu dem die einzelnen Artikel gekauft wurden.
{% endhint %}

![Lieferantengesamtsummen](../../.gitbook/assets/oc-supplier-totals.jpg)

![Lieferantengesamtsummen nach Verteilstelle](../../.gitbook/assets/oc-supplier-totals-by-distributor.jpg)

![Verteilstellengesamtsummen nach Lieferanten](../../.gitbook/assets/oc-distributor-totals-by-supplier.jpg)

{% hint style="success" %}
Diese Berichte sind nützlich, um den Betrag zu berechnen, der einem Lieferanten für gelieferte Artikel zu erstatten ist
{% endhint %}

### Kundengesamtsummen

{% hint style="success" %}
Nützlich für:

* Erfüllung von Aufträgen auf individueller Basis
* Vorbereitung von Einzelaufträgen in großen Mengen
{% endhint %}

Dieser Bericht enthält die meisten Daten:

* Datum und Uhrzeit der Bestellung zusammen mit der Bestell-ID
* Kundenname, E-Mail, Telefonnummer, Rechnungs- und Lieferadresse
* Für jedes Produkt innerhalb einer Bestellung gibt es den Namen des Produkts, den Variantennamen, die Menge, den Preis, den vom Kunden gezahlten Preis (Artikelpreis + Gebühren), eine Aufschlüsselung der Gebühren (Unternehmens-, Zahlungs- und Versandartgebühren für jedes Produkt), den Hersteller
* Name des Hubs.
* Zahlungsart und Status (z. B. bezahlt, unbezahlt)
* Versandart, Lieferung oder Abholung

{% hint style="info" %}
Die Versandadresse, die für eine Bestellung angezeigt wird, bei der die Versandart "Abholung" gewählt wurde, ist die Adresse des Verteilzentrums.
{% endhint %}

Die folgende Abbildung zeigt die Informationen, die in einem Bericht über die Gesamtzahl der Kunden im Bestellzyklus enthalten sind.

![Kundengesamtsummen](../../.gitbook/assets/oc-customer-totals.jpg)
