# Durchführung einer Social Media Promotion

## Einführung

Um treue Kunden zu halten und/oder neue Kunden zu gewinnen, können Sie von Zeit zu Zeit eine Werbeaktion in den sozialen Medien durchführen. Sie könnten zum Beispiel auf Facebook und Instagram posten, dass Kunden für alle Bestellungen, die in der kommenden Woche im Wert von mehr als 20 Pfund eingehen, einen Rabatt von 5 % auf ihren Einkauf in der folgenden Woche erhalten.

Im Folgenden finden Sie eine schrittweise Anleitung zur Umsetzung des obigen Beispiels. Der Prozess basiert auf der äußerst flexiblen [Tag- und Tag-Regel-Funktion](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#zahlungsarten-anzeigen-ausblenden) der OFN-Plattform. Am Ende dieser Seite finden Sie Tipps, wie Sie dieses Werbeangebot [anpassen](running-a-social-media-promotion.md#sie-koennten-auch-in-erwaegung-ziehen-stammkunden-mit-einem-kleinen-rabatt-zu-belohnen.) können.

## Prozess

{% hint style="warning" %}
Dies ist ein DREISTUFIGER Prozess:

1. Identifizierung der zugelassenen Kunden, die über dem Schwellenwert gekauft haben.
2. So können diese Kunden in der folgenden Woche einen Rabatt erhalten.
3. Dieser Rabatt wird nach einer Woche aufgehoben.
{% endhint %}

### Schritt eins

* Überprüfen Sie Ihre [Bestellungen](https://app.openfoodswitzerland.ch/admin/orders), wenn der aktuelle Bestellzyklus abgeschlossen ist. Sie können alle Kunden, die über dem Schwellenwert gekauft haben, wie folgt identifizieren:
  1. Filter nach Auftragszyklusname
  2. Sortieren nach Gesamtwert hoch bis niedrig (zweimal auf 'Gesamt' klicken)

![](https://lh5.googleusercontent.com/WkOpNQ7tngre9J8YhYye8cP7a6-Cl5xdnc26z4Nd4TjCkUE2bozCPSKAo1IHiWFwIIITZ1l4h5sLzJmPjIfzpM1gKBu\_cS2-b877P8LOGm6r4Yre1S6uoVZeJh9oDmG\_g\_5e7JoG)

### Zweiter Schritt

* Besuchen Sie Ihre [Kundenseite](https://app.openfoodswitzerland.ch/admin/customers).
* Verwenden Sie das Feld "Schnellsuche", um Kunden zu finden, die im Bestellzyklus der letzten Woche mehr als den von Ihnen festgelegten Schwellenwert ausgegeben haben.

![](../../.gitbook/assets/customers1.jpg)

* Fügen Sie dem Eintrag des Kunden das Tag "week2reward" hinzu.

![](https://lh5.googleusercontent.com/msnCbxUJsibbhqjIkK8bWAGDaqgGcPWSiAdZQcNc0bi1h\_rx49qtGG4XxXLYyD9KIXaoS55kMXtHO3NXmghqUZn1EPv\_memdQqy4D07rugbzEculm-wSa4MpR9CpmboYi7CTZFnb)

*
* Gehen Sie zu **Unternehmen -> Einstellungen** und wählen Sie dann "[Zahlungsmethoden](../../basic-features/shopfront/payment-methods.md)" aus dem linken Menü. Klicken Sie auf **+ Neue Zahlungsmethode**.

![](<../../.gitbook/assets/thankyoupaymentmethod (1).jpg>)

\
Name: Dankeschön Rabatt\
Beschreibung: eine Nachricht Ihrer Wahl (z. B. "Als kleines Dankeschön für Ihre Unterstützung möchten wir Ihnen diese Woche einen Rabatt von 5 % auf Ihren Einkauf anbieten")\
Anzeige: Sowohl Kasse als auch Back Office\
Aktiv: ja\
**Tags: Fügen Sie den Tag 'week2reward' an dieser Stelle ein.**\
Anbieter: Wählen Sie die für Ihr Unternehmen am besten geeignete Methode.\
Honorar-Rechner: Pauschaler Prozentsatz

* Nachdem Sie "Erstellen" ausgewählt haben, fügen Sie in das Feld "Betrag" des Abschnitts "Gebührenrechner" ein "-5" \* ein. (Negatives Vorzeichen führt zu einem Rabatt)\
  \
  \*-5 führt zu einer Ermäßigung von 5 %, wenn Ihr Unternehmen keine Enterprise Fees verwendet.

![](../../.gitbook/assets/pmcalc.jpg)

{% hint style="danger" %}
Alle **prozentualen Gebühren** werden nur auf der Grundlage eines Prozentsatzes der **Produktkosten** berechnet.
{% endhint %}

{% hint style="warning" %}
Wenn Ihr Unternehmen eine pauschale Unternehmensgebühr auf alle Produkte erhebt, müssen Sie für diese Rabatt-Zahlungsmethode den folgenden Betrag in das Feld "Pauschaler Prozentsatz" eingeben:

&#x20;$$= (100 + Unternehmensgebühr)* Gewünschter Rabatt/100$$&#x20;

z. B. für ein Unternehmen mit einer Unternehmensgebühr von 20 %, das Freiwilligen einen Rabatt von 5 % gewähren möchte, lautet der Betrag, der in den pauschalen Prozentsatz für diese Zahlungsmethode einzugeben ist:

$$= -(100 + 20) *5/100 = -6$$&#x20;
{% endhint %}

* Rufen Sie die Seite **Unternehmen -> Einstellungen** auf und wählen Sie im linken Menü die Option "Tag-Regeln" aus. Richten Sie die folgenden [Tag-Regeln](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#zahlungsarten-anzeigen-ausblenden) ein:

Standard: Zahlungsmethoden mit der Bezeichnung 'week2reward' sind nicht sichtbar.\
Für Kunden mit dem Tag "week2reward" sind Zahlungsmethoden mit dem Tag "week2reward" sichtbar.

![](https://lh3.googleusercontent.com/VbTR4DNvEgEduOZz2DuJDeMZSjHC10XVPhFpVKEN6hN7t7L66B599oiTFuUvUKgfm4fAZtBhyHcBHjQtiqF0\_1N\_DJDiDi6XcVY3MjyZbTsXTtOBABp3jnoNcqww8oGBIZm-Z3ky)

**Bingo! Nur die Kunden, die letzte Woche mehr als den Schwellenwert ausgegeben haben, erhalten diese Woche einen Rabatt von 5 %, wenn sie bei Ihnen einkaufen.**

![Checkout view for eligible customer](https://lh4.googleusercontent.com/mYndbgcYtUAcWk0Hzf1fHmnnVYOK78o2CsUVpshoPmCHXQAh6M7r0UFWoYSrCNqxlwVzDIkPANPPbNJdGv5na7b64xVEs-vBrp32oRODlgDgKiTLqVIn4DKk-ODCiIFrWDZZRXF9)

### Dritter Schritt

Wenn der Bestellzyklus abgeschlossen ist, möchten Sie vielleicht nicht, dass diese bestimmte Gruppe von Kunden für einen 5%-Rabatt auf ihre zukünftigen Einkäufe in Frage kommt (d.h. dass der Rabatt länger als eine Woche gilt). In diesem Fall müssen Sie entweder:

* Entfernen Sie das "week2reward"-Tag aus allen Kundennamen\
  **Oder**
* Ändern Sie die Tag-Regel in:\
  Für Kunden mit dem Tag 'week2reward' sind Zahlungsmethoden mit dem Tag 'week2reward' NICHT SICHTBAR.

![](https://lh4.googleusercontent.com/ub-vearrc\_EX85fXpvGNyr1YQLTMvqd-5q8WNrLSDboGVu\_3kWh240orHjgqBElO-dGW4hf\_41p\_JQce4YBhbd1O7wW1B4ylqcw0JiY\_6qUirT6kerXo2tpitFKbrI7o\_j5QbamA)

## Sie könnten auch in Erwägung ziehen, Stammkunden mit einem kleinen Rabatt zu belohnen.&#x20;

Wenn Sie nur die Kunden belohnen, die mehr als einen bestimmten Betrag ausgeben, werden möglicherweise diejenigen ausgeschlossen, die allein leben oder ein begrenztes Haushaltsbudget haben. Vielleicht möchten Sie eine Kampagne in den sozialen Medien durchführen, um die Kundentreue zu fördern - unabhängig vom Wert der wöchentlichen/monatlichen Ausgaben.

Dazu müssen Sie extern aufzeichnen, wie oft jeder Kunde in Ihrem OFN-Schaufenster einkauft. Das [Support-Team in Ihrer lokalen Instanz ](../../local-ofn-organizations-and-contacts.md)kann Ihnen vielleicht dabei helfen, diese Daten zusammenzustellen.

Mit diesen Informationen können Sie einige Ideen für Kampagnen umsetzen:

**5% Rabatt auf die nächste Bestellung für Kunden, die x Wochen/Bestellzyklen hintereinander bestellen.**

In diesem Fall würden Sie dieselben Schritte wie oben beschrieben durchführen, um sowohl den Kunden als auch die Zahlungsmethode (mit einem negativen Gebührenrechner) für einen Auftragszyklus zu kennzeichnen.

#### Kostenlose oder ermäßigte Lieferung der nächsten Bestellung für Kunden, die eine bestimmte Anzahl von Wochen hintereinander bestellt haben (z. B. 3 Lieferungen kaufen und die nächste kostenlos erhalten). 

In diesem Fall würden Sie den Kunden mit einem Tag versehen (z. B. "thankyouweek1") und dann eine [Versandmethode](../../basic-features/shopfront/shipping-methods.md) mit demselben Tag erstellen (die zu einem ermäßigten Preis angeboten wird).

Die Standard- und ergänzenden Tag-Regeln lauten:

Standard: Versandmethoden mit dem Tag thankyouweek1 sind NICHT SICHTBAR\
Regel: Für Kunden, die mit thankyouweek1 gekennzeichnet sind, sind die mit thakyouweek1 gekennzeichneten Versandmethoden SICHTBAR\
\
\
\
