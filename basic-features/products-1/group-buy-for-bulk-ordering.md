# Group Buy - für Großbestellungen

Die Funktion "**Gruppenkauf**" ist für Unternehmen gedacht, die einen Teil ihrer eingehenden Bestände in großen Mengen kaufen und in kleineren Einheiten weiterverkaufen (z. B. Kauf eines 25-kg-Sacks Reis und Verkauf an Kunden pro kg).

Großeinkäufe sind eine gängige Praxis für **Einkaufsgemeinschaften**, die durch den Kauf großer Mengen von den Großhandelspreisen genauso profitieren können wie herkömmliche Vertriebsunternehmen. Auf diese Weise können die Mitglieder viel billiger an Lebensmittel kommen, als sie es vielleicht bei den Einzelhändlern auf der Straße tun könnten.

Für solche Unternehmen hängt die Entscheidung, ob sie ein bestimmtes Produkt bestellen, davon ab, ob die Kunden insgesamt genug bestellt haben, um einen Großeinkauf zu rechtfertigen. Dies kann aufgrund von Mengenrabatten oder Liefergebühren der Fall sein. Die Funktion des Gruppenkaufs erleichtert es dem Zentrum, die Effizienz des Großeinkaufs zu steigern.

Wenn ein Produkt dem Gruppenkauf zugewiesen ist, wird es mit der Aufschrift "Bulk" über dem Foto auf Ihrer Shopfront angezeigt. Wenn ein Kunde das Produkt in den Warenkorb legt, wird er in einem Pop-up- Fenster aufgefordert, die Mindest- und Höchstmenge einzugeben (siehe unten):

![](../../.gitbook/assets/bulkbuy.gif)

Die Kunden werden gebeten, dies anzugeben:

* Ihre **Mindestmenge** - das ist die Menge des Produkts, die sie idealerweise haben möchten.
* Ihre **Höchstmenge** - dies ist die maximale Menge, die sie zu kaufen bereit wären.

{% hint style="info" %}
Im Wesentlichen ist dies eine Möglichkeit für den Kunden zu sagen: "_Sie haben meine Erlaubnis, meine Bestellung bis zu diesem Punkt zu erhöhen, wenn dies bedeutet, dass wir als Gruppe die Großbestellmenge erreichen können"_.
{% endhint %}

In der [Großbestellungsverwaltung](../orders/view-orders.md#bulk-order-management) können Sie die gesamten Mindest- und Höchstbestellmengen für das Produkt von allen Ihren Kunden einsehen. Dann können Sie entweder die Kundenbestellungen innerhalb des zulässigen Bereichs erhöhen, um die Gesamtmenge zu erreichen, oder Sie können alle Bestellungen für dieses Produkt löschen, wenn die maximale Bestellmenge unterschritten wird.

{% hint style="danger" %}
Die Gruppenkauffunktion kann **nicht** auf Produkte angewendet werden, die mit Einheiten = **Artikel** aufgeführt sind.
{% endhint %}

## Aktivieren des Gruppenkaufs für ein Produkt

Gehen Sie auf dem Admin-Dashboard im blauen horizontalen Menü auf "**Produkte**". Wählen Sie die Option "Produkt **bearbeiten**", indem Sie auf das Bleistift- und Papiersymbol rechts neben dem betreffenden Produkt klicken:

![](../../.gitbook/assets/productedit.jpg)

Wählen Sie dann im Menü auf der rechten Seite **Gruppenkaufoptionen**.

![](../../.gitbook/assets/groupbuy.jpg)

Wählen Sie **Ja** unter **Gruppenkauf?**, **um diese Funktion für das Produkt zu aktivieren.**

Die **Großeinheitsgröße** ist der Betrag, den die Sammelbestellung der Gruppe erreichen muss.

{% hint style="warning" %}
Die **Einheiten** für die Bulk-Unit-Größe hängen von den Einheiten ab, die für den Verkauf des Produkts an Kunden ausgewählt wurden.

Wenn das Produkt von verkauft wird:

* **Gewicht:** Einheiten sind in g (wenn also die Gesamtsumme 5 kg betragen soll, geben Sie in dieses Feld '5000' ein)
* **Volumen:** Einheiten sind in Litern (wenn also die Gesamtsumme 10 l betragen soll, geben Sie in dieses Feld '10' ein)
* **Artikel:** Wenn Sie z. B. Blumensträuße verkaufen, aber insgesamt 100 Sträuße kaufen müssen, geben Sie in dieses Feld "100" ein.
{% endhint %}

## Anpassung von Aufträgen zur Erstellung vollständiger Chargen

Unter Bestellungen-> [Verwaltung von Großbestellungen](../orders/view-orders.md#bulk-order-management) können Sie Kundenbestellungen für Großeinkaufsprodukte anzeigen und bearbeiten, damit die kombinierte Bestellung aller Kunden den von Ihnen gewünschten Schwellenwert erreicht.

1. Wählen Sie den gewünschten Auftragszyklus oder Datumsbereich aus.
2. Suchen Sie nach dem Produkt (im Beispiel unten: Fisch).
3. Vergewissern Sie sich, dass die Spalte "Max" angezeigt wird, damit Sie die Obergrenze sehen können, die jeder Kunde bereit ist zu kaufen.
4. Klicken Sie dann auf den Wert ('Testfisch: Fisch Eins' im Beispiel unten) in der Spalte **Produkt : Einheit**, um das Feld Gesamtbestellungen (in blau) für das betreffende Produkt anzuzeigen.
5. Anhand der Angaben in der Spalte **Max** können Sie die bestellten Mengen erhöhen, um den Schwellenwert für eine vollständige Charge zu erreichen.&#x20;
6. Klicken Sie auf Aktualisieren, um die Änderungen an den Kundenaufträgen zu speichern.

![](../../.gitbook/assets/bulkorder2.jpg)

**Current Fulfilled Units (Aktuell erfüllte Einheiten)** dividiert Ihre Gesamtbestellmenge durch die Größe der Gruppenkaufeinheit. Wenn diese Zahl größer als 1 ist, bedeutet dies, dass die vorhandenen Kundenbestellungen die von Ihnen geforderte Stückzahl für den Gruppenkauf erfüllen oder überschreiten. Ist diese Zahl kleiner als 1, erfüllen die vorhandenen Kundenbestellungen diesen Schwellenwert nicht. Wenn Sie die Menge der Kundenaufträge erhöhen, steigt diese Zahl.

**Max Fulfilled Units (Max. erfüllte Einheiten)** ist die Summe aller MAX-Bestellmengen des Kunden, geteilt durch die Größe der Gruppenkaufeinheit. Ist diese Zahl größer als 1, dann wissen Sie, dass die Summe Ihrer MAX-Bestellungen die erforderliche Gruppenkaufmenge übersteigt. Ist diese Zahl kleiner als 1, bedeutet dies, dass auch die MAX-Bestellmengen den Schwellenwert nicht erreichen.
