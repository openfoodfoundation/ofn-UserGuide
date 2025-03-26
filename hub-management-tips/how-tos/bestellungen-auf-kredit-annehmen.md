# Bestellungen auf Kredit annehmen

## Einführung

Obwohl diese Funktion noch nicht in OFN integriert ist, ist es mit ein paar schnellen Schritten möglich, Kunden die Möglichkeit zu geben, mit Prepaid-Guthaben auf OFN zu bezahlen. Dazu muss zunächst ein Kreditprodukt erstellt werden, mit dem der Kunde auscheckt. Der Filialleiter geht dann in das Backoffice und „löscht“ dieses Produkt, indem er ein „Guthaben“ auf das Kundenkonto setzt. Künftige Bestellungen können dann mit dem Guthaben auf dem Konto „bezahlt“ werden.

## Prozess

Erstellen Sie zunächst ein Kreditprodukt im Backend. Wenn Sie das Produkt im Backend erstellen, legen Sie auch eine Variante mit dem Namen „Platzhalterguthaben“ für CHF 0 und mit „0“ für „vorrätig“ an. Diese Variante wird später in der Bestellverwaltung im Backend nützlich sein. Fügen Sie dann alle Varianten zu einem Bestellzyklus hinzu, um das Prepaid-Guthaben an Ihre Kunden zu verkaufen.

Hier ist ein Beispiel für ein Kreditprodukt im Schaufenster, das der Kunde auswählen kann, um seinem Konto „Kredit“ hinzuzufügen.

Weisen Sie den Kunden an, die Höhe des Guthabens auszuwählen, das er seinem Konto gutschreiben möchte, und überprüfen Sie seine Bestellung. Achten Sie darauf, dass der Kunde seine Kontoinformationen „speichert“, indem er beim Auschecken „LOGIN“ wählt und ein Konto mit einem Passwort erstellt.

![image3](https://user-images.githubusercontent.com/88801240/207040600-029c79d3-f975-4985-849d-4af2f0df0085.png)

Im Backend sehen Sie nun die Bestellung mit dem Betrag des Guthabens, das sie kaufen.

Sobald der Kunde die Bestellung bezahlt hat, können Sie die Zahlung mit dem grünen Häkchen „erfassen“.

Dann müssen Sie die Bestellung bearbeiten, aber zuerst müssen Sie dem Produkt „Platzhalterguthaben“ einen „Bestand“ hinzufügen. Fügen Sie die Menge an „Vorrat“ hinzu, die der Anzahl der Kreditaufträge entspricht, die Sie zu diesem Zeitpunkt bearbeiten (d.h. Sie haben 1 Kreditauftrag, fügen Sie „1“ als „Vorrat“ zur Variante „Platzhalter Kredit“ hinzu und SPEICHERN SIE DIE ÄNDERUNGEN).

Nun können Sie zu Ihrer Bestellliste zurückkehren und die Kreditbestellung bearbeiten“.

Zuerst müssen Sie das „Platzhalterguthaben“ zur Bestellung hinzufügen.

Jetzt können Sie das andere „Guthaben“-Produkt aus der Bestellung löschen (durch das Hinzufügen der „Platzhalter-Guthaben“-Variante wird verhindert, dass die gesamte Bestellung storniert wird; dieser Schritt wäre unnötig, wenn die Bestellung bereits andere Produkte enthält).

In Ihrer Auftragsliste wird der Zahlungsstatus für den Auftrag nun auf „Guthaben“ für den Betrag des vorausbezahlten Guthabens zurückgesetzt.

So sieht es auch in Ihrer Kundenliste auf der Registerkarte Kunden für diesen Kunden aus.

Und wenn Sie unter **Berichte** einen Lieferbericht für einen Bestellzyklus (Bestellzyklusverwaltung -> Lieferungen) erstellen, wird dieser einen positiven Saldo für den Kunden ausweisen.

Und wenn sich der Kunde bei seinem Konto auf OFN anmeldet und zu den Transaktionen geht, sieht er den laufenden Saldo seines Kontos bei Ihnen.

Um das Guthaben für künftige Bestellungen zu verwenden, müssen Sie eine [Zahlungsoption einrichten](bestellungen-auf-kredit-annehmen.md#einfuhrung)[ ](bestellungen-auf-kredit-annehmen.md#einfuhrung)- „mit Guthaben bezahlen“ -, die die Kunden an der Kasse auswählen können, um anzugeben, dass sie ihr Guthaben verwenden möchten.

Sie können [Tags](https://guide.openfoodnetwork.org/v/deutsch/basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules) verwenden, wenn Sie möchten, dass diese Zahlungsoption nur für die Kunden verfügbar/sichtbar ist, die bei Ihnen ein Prepaid-Guthaben erworben haben. Fügen Sie das entsprechende Tag zum Kundenkonto hinzu:

Und richten Sie die folgenden Tag-Regeln ein:

Stellen Sie sicher, dass Sie die neue Zahlungsmethode auf Seite 4 Ihrer Bestellzyklen ('Checkout options') hinzufügen, wenn Sie einen neuen Bestellzyklus einrichten.

Dies ist das, was der Kunde sieht, wenn er zur Kasse geht.

Sobald der Kunde eine 2. Bestellung aufgegeben hat, erscheint diese in Ihrer **Bestellungsliste** mit einem **fälligen** **Saldo**.

Das sehen sie, wenn sie sich bei ihrem Konto anmelden. Der negative Betrag steht für das Restguthaben.

Und genau das werden Sie sehen, wenn Sie als Manager von Ihrer Kundenliste ausgehen.

Und wenn Sie den Lieferbericht ausführen.

**WENN** Sie die neue Bestellung als „Bezahlt“ markieren möchten, indem Sie den Zahlungsstatus von „Restbetrag fällig“ auf „Bezahlt“ ändern, können Sie auf das grüne Häkchen rechts neben der Bestellung klicken. (**Hinweis**: Überprüfen Sie zunächst Ihre Kundenliste, um sicherzustellen, dass der Kunde über genügend Guthaben verfügt, um die Kosten der Bestellung zu decken. Ist dies nicht der Fall, können Sie eine Teilzahlung auf die Bestellung mit dem verbleibenden Guthaben vornehmen und dem Kunden dann eine Rechnung über den Restbetrag der Bestellung schicken).

Der Zahlungsstatus der Bestellung lautet nun „bezahlt“ in Ihrer Auftragsliste.

Im Kundendatensatz und in Ihrer Kundenliste wird der laufende Saldo jedoch wieder auf den vollen im Voraus bezahlten Kreditbetrag zurückgesetzt.

Um die Zahlung für den 2. Auftrag dem laufenden Guthaben gutzuschreiben, müssen wir nun den ursprünglichen Kreditauftrag aufrufen und eine negative Zahlung in Höhe des 2. Auftrags vornehmen (d. h. - 5,70 CHF).

Bearbeiten Sie zunächst den ursprünglichen Kreditauftrag.

Wählen Sie dann Zahlungen aus dem Menü auf der rechten Seite. Wählen Sie Neue Zahlung aus dem Menü oben rechts.

Geben Sie den Betrag der bezahlten Bestellung ein, dem ein Minuszeichen vorangestellt ist (z. B. -CHF 5,70), und wählen Sie „Per Kredit bezahlen“, dann „Aktualisieren“.

Erfassen“ Sie diese Zahlung mit dem grünen Häkchen.

Jetzt wurde das „geschuldete Guthaben“ um den korrekten Betrag auf dem Kreditauftrag reduziert.

![image30](https://user-images.githubusercontent.com/88801240/207069952-80e23eb1-92a8-4654-931d-1bdd316d7be9.png)

Und der Saldo ist in Ihrer Kundenliste korrekt.

Und im Lieferbericht wird der aktuelle Saldo für den Kunden angezeigt. Die 2. Bestellung wurde bezahlt (sie ist also nicht mehr negativ) und das Guthaben oder der positive Saldo wurde reduziert.

Und wenn sich der Kunde schließlich in sein Konto einloggt, sind der aktuelle Saldo und der Guthabenbetrag korrekt.
