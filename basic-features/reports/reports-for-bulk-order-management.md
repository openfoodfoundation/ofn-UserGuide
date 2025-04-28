# Berichte für die Verwaltung von Großaufträgen

Die im Bereich Gruppenkäufe verfügbaren Berichte sind ideal für Unternehmen auf der OFN-Plattform, z. B. Einkaufsgemeinschaften, die die [Funktion Gruppenkauf](../products-1/group-buy-for-bulk-ordering.md) nutzen.

Es gibt vier Berichte in diesem Abschnitt:

|                 | Funktion                                                                                                                                                                                                                    |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lieferanten     | Produkte nach Anbieter auflisten. Dies ist eine  gute Möglichkeit, um zu sehen, ob genug von einem Produkt bestellt wurde, um die Mindestbestellmenge des Lieferanten zu erreichen.                                         |
| Zuteilung       | Listet die Produkte nach Kunden auf. Erlaubt sicherzustellen, dass Sie die Artikel des Großeinkaufs gleichmäßig auf die Kunden verteilen (d. h., dass eine Person nicht zu wenig/zu viele Artikel in ihrer Bestellung hat). |
| Packlisten      | Umpacken von Produkten, die von einem Lieferanten in grosser Menge geliefert werden, zur Abholung durch den Kunden.                                                                                                         |
| Kundenzahlungen | Dokumentiert die Rückerstattung an den Kunden bzw. die vom Kunden geforderte Nachzahlung nach der Anpassung der Lagerbestände an einen Großauftrag                                                                          |

## Daten

Die Daten in jedem Bericht sind wie folgt:

|                                               | Lieferanten | Zuteilung | Packlisten | Kundenzahlungen |
| --------------------------------------------- | ----------- | --------- | ---------- | --------------- |
| Kunde                                         | N           | J         | J          | J               |
| Anbieter                                      | J           | N         | N          | N               |
| Name des Produkts                             | J           | J         | J          | N               |
| Details zur Variante                          | J           | J         | J          | N               |
| Schüttguteinheit                              | J           | J         | N          | N               |
| Gekaufte Menge                                | J           | J         | J          | N               |
| Erforderliche Einheiten                       | J           | J         | N          | N               |
| Nicht zugewiesene                             | J           | J         | N          | N               |
| Maximale Überschussmenge                      | J           | J         | N          | N               |
| Date of order                                 | N           | N         | N          | J               |
| Gezahlter, geschuldeter Betrag & Gesamtkosten | N           | N         | N          | J               |



{% hint style="warning" %}
Produkte, die von einem Hub gelagert werden und bei denen der Großeinkauf nicht aktiviert ist, werden mit Bulk Unit = 0 angezeigt.
{% endhint %}

![Lieferanten-Bericht](../../.gitbook/assets/bulksuppliertot.jpg)

![Zuteilungs-Bericht](../../.gitbook/assets/bulkallocation.jpg)

![Packlisten-Bericht](../../.gitbook/assets/bulkpacking.jpg)

![Kundenzahlungen-Bericht](../../.gitbook/assets/bulkpayment.jpg)

## Beispiel: Gruppenkauf Lieferanten-Bericht

Dieser Bericht enthält die folgenden Informationen:

* Haben die Kunden genug von einem Produkt bestellt, um die Bestellung der Großpackung beim Lieferanten zu rechtfertigen?
* Wie viele zusätzliche Produkte sind die Kunden bereit zu kaufen, damit die Gruppe die Mengenschwelle erreicht (wenn [Gruppenkauf](../products-1/group-buy-for-bulk-ordering.md#aktivieren-des-gruppenkaufs-fuer-ein-produkt) aktiviert ist)
* Wie viele Grosspackungen werden benötigt, um die Kundennachfrage zu befriedigen?
* Wenn die Großpackung bestellt wird, wie viel Bestand bleibt dann noch übrig?
* Wie viele Kunden werden enttäuscht sein, wenn dieses Produkt nicht bestellt wird?

Das nachstehende Beispiel veranschaulicht, wie der Bericht "Bulk Co-op Totals by Supplier" verwendet werden kann:

Beispiel 1: Wenn die Großbestellmenge erreicht ist:

![](../../.gitbook/assets/radishess.png)

Beispiel 2: Die Menge der Großbestellung ist noch nicht erreicht:

![](../../.gitbook/assets/bok-choy.png)

* Beachten Sie, dass der Bericht "Gruppenkauf Zuteilung" eine ähnliche Funktion wie dieser Bericht hat, aber die Bestellungen jedes einzelnen Kunden anzeigt und nicht die kumulierte Summe aller Kunden.
