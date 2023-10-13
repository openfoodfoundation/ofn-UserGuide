---
description: Zahlungsberichte, Steuerberichte, Xero
---

# Zahlungen und Steuerberichte

## Zahlungsberichte

{% hint style="success" %}
Die drei Zahlungsberichte sind gut geeignet, um den Überblick über die gesamten ein- und ausgehenden Einnahmen Ihres Lebensmittelzentrums innerhalb eines bestimmten Zeitraums zu behalten.
{% endhint %}

### Zahlung nach Art

Der einfachste Zahlungsbericht. Dieser dokumentiert die Summe der gezahlten Beträge, den fälligen Saldo und das geschuldete Guthaben für die verschiedenen Zahlungsarten, die ein Hub verwenden kann (z. B. eine Summe für Stripe-Zahlungen, eine Summe für Bargeld/EFT-Zahlungen und eine für PayPal).

![Payment by Type](../../.gitbook/assets/payment-by-type.jpg)

### Einzelverbindungsnachweis Gesamtbetrag der Zahlungen

Dieser Bericht ist nach Zahlungsstatus (bezahlt, fälliger Saldo, ausstehendes Guthaben) und nicht nach Zahlungsanbieter geordnet und enthält eine Aufschlüsselung der Einnahmen (Produktkosten, Versandgebühren) sowie der Gesamtsumme. Die Spalte Ausstehender Saldo ist 0,0 für den Zahlungsstatus "bezahlt".

![Itemised Payment Totals](../../.gitbook/assets/itemizedpayment.jpg)

### Zahlungssummen

Zusätzlich zu den Gesamtbeträgen der Einzelzahlungen werden in diesem Bericht die Einnahmen aus EFT (Bargeld oder Banküberweisung) und Paypal separat aufgeführt.

![Payment Totals](../../.gitbook/assets/payment-totals.jpg)

## Verkaufssteuer

Es gibt zwei Umsatzsteuermeldungen: Steuerarten und Steuersätze.

{% hint style="success" %}
Der Bericht "**Steuerart**" ist nützlich, um die Gesamtsteuer pro Bestellung in ihre verschiedenen Bestandteile aufzuteilen: Steuer auf Produkte, Steuer auf Versandart und Steuer auf Zahlungsart.
{% endhint %}

![Tax type report](../../.gitbook/assets/taxtype.jpg)

Der Bericht über die **Steuersätze** enthält eine auftragsbezogene Aufschlüsselung der Steuern nach dem jeweiligen Steuersatz (voll, ermäßigt oder zum Nullsatz). Es werden auch die Auftragssummen einschließlich und ausschließlich der Steuer angegeben.

![Tax rate report](../../.gitbook/assets/taxrates.jpg)

## Xero-Rechnungen

Dieser Bericht erstellt CSV-Dateien, die in das Buchhaltungspaket "Xero" importiert werden können, um Rechnungen für Kunden zu erstellen.

### Generierung des Berichts

![Xero Report Fields](../../.gitbook/assets/xero-report.png)

**Datumsbereich:** Sie können Bestellungen nach dem Datum filtern, an dem die Bestellung aufgegeben wurde.

**Berichtstyp:** Sie können einen "detaillierten" Bericht herunterladen, der einen Einzelposten für jeden Artikel enthält, den der Kunde gekauft hat, einschließlich aller Gebühren und Anpassungen an seiner Bestellung.

**Hub und Auftragszyklus:** Sie können angeben, über welchen Hub und Auftragszyklus die Aufträge erteilt wurden.

**Erste Rechnungsnummer:** Um die Kompatibilität mit Ihrem Xero-Rechnungsnummerierungssystem zu gewährleisten, geben Sie die erste Rechnungsnummer ein, die neuen Rechnungen zugewiesen werden soll. Alle nachfolgenden Rechnungen werden ab diesem Punkt nummeriert.

**Rechnungsdatum:** Sie können das Datum auswählen, mit dem die Rechnungen in Xero gekennzeichnet werden sollen. Dieses Datum kann bearbeitet werden, sobald Sie die Rechnung in Xero haben, aber wenn Sie es hier eingeben, können Sie alle Rechnungen in einem einzigen Bericht datieren.

**Fälligkeitsdatum:** Sie können das Fälligkeitsdatum auswählen, das auf Xero-Rechnungen markiert werden soll. Auch dies ist in Xero bearbeitbar.

**Kontocode:** Wenn Sie hier einen Xero-Kontocode eingeben, werden alle Posten der Rechnung diesem Konto zugeordnet. Dieser Code kann in Xero bearbeitet werden.

**Als CSV herunterladen:** Wenn Sie bereit sind, die Datei für den Import herunterzuladen, aktivieren Sie das Kontrollkästchen und klicken Sie auf **Suchen**.

### Daten verfügbar

* Kundenname, E-Mail, Rechnungsadresse (keine Telefonnummer)
* Rechnungsnummer und Datum des Kaufs. Das Fälligkeitsdatum ist ein Monat nach Rechnungsdatum. Die Referenznummer ist dieselbe wie die Rechnungsnummer.
* Produktname, Menge, Kosten, Steuersatz, SKU, Gebühr
* Zahlungsstatus (bezahlt oder fälliger Saldo)
* Währung der Transaktion.

### Importieren des Berichts in Xero

Gehen Sie in Xero zu **Konten**, **Verkäufe** und klicken Sie auf Importieren.

![Xero Import](../../.gitbook/assets/xero-import.png)

Als nächstes wählen Sie Ihren heruntergeladenen OFN Xero-Bericht zum Hochladen aus. Die Einstellungen, die Sie auswählen sollten, sind unten aufgeführt.

![Xero Import Steps](../../.gitbook/assets/xero-import-steps.png)

Durch die Auswahl von **Ignorieren der** Kontaktadressdaten wird sichergestellt, dass Ihre Xero- Kundendaten nicht verändert werden.

Wenn Sie die Option "**Steuerfrei**" auswählen, wird sichergestellt, dass die Produkte, die Sie im Open Food Network als steuerpflichtig gekennzeichnet haben, auch steuerpflichtig sind, während Ihre steuerfreien Artikel steuerfrei bleiben.
