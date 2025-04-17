# Abonnements - FAQs

### Wenn ich einen Bestellzyklus aus einem Zeitplan entferne, an den bereits offene Abonnementaufträge angehängt sind, was geschieht dann mit diesen Aufträgen? Werden diese Abonnements dann gelöscht?

Diese Aufträge bleiben offen. Bei Abschluss des Bestellzyklus werden die Abonnementaufträge wie normale Abonnementaufträge bearbeitet. Wenn Sie alle Abonnementaufträge, die mit diesem Bestellzyklus verbunden waren, stornieren möchten, müssen Sie jeden [Abonnementauftrag einzeln löschen](subscriptions-creating-and-managing-orders.md#bearbeiten-sie-das-basisabonnement).

### Wenn ich ein neues Abonnement in der Mitte eines offenen Bestellzyklus hinzufüge, wird dann ein Abonnement für diesen Kunden erstellt?

Ja, wenn Sie ein Abonnement erstellen, während ein Bestellzyklus in diesem Zeitplan offen ist, wird ein Auftrag für diesen Kunden erstellt. Wenn Sie nicht möchten, dass das Abonnement für den aktuellen offenen Bestellzyklus gilt, müssen Sie das Startdatum des Abonnements auf einen Zeitpunkt nach dem Ende dieses Bestellzyklus festlegen.

### Was ist, wenn ein Teil des Bestands verfügbar ist, aber nicht der gesamte Bestand? Welche Kunden erhalten den begrenzten Vorrat?

Wenn der Bestand eines Produkts nicht ausreicht, um alle Abonnementbestellungen zu erfüllen, wird der begrenzte Bestand nicht gleichmäßig auf die Kunden verteilt, sondern es werden die Kundenbestellungen mit dem verfügbaren Bestand erfüllt, bis dieser aufgebraucht ist. Einige Kunden erhalten ihre gesamte Bestellung, andere erhalten keine.

### Was passiert, wenn ich das Abonnement ändere, während es "offen" ist?

Es ist nicht möglich, **Artikel** zum Hauptabonnementauftrag **hinzuzufügen**, während ein Bestellzyklus des Abonnementplans offen ist. Alle zusätzlichen Produkte müssen hinzugefügt werden, wenn die Bestellzyklen geschlossen sind (d. h. bei wöchentlichen Abonnements, die dem Zeitplan "Wöchentlich" zugeordnet sind, in dem Zeitraum zwischen dem Schließen von Bestellzyklus A und dem Öffnen von Bestellzyklus B, wenn sowohl A als auch B zum Zeitplan "Wöchentlich" gehören).

Wenn Sie das Hauptabonnement eines Kunden bearbeiten, um **Produkte zu entfernen**, während ein Bestellzyklus geöffnet ist, wirkt sich diese Änderung auf die im aktuellen Bestellzyklus aufgegebene Bestellung aus.

### Was ist, wenn der Vorrat begrenzt ist, aber ein Kunde seine Bestellung storniert? Wird dieser Vorrat dann automatisch anderen Abonnenten zugeteilt, die das Produkt haben wollten, es aber aufgrund des unzureichenden Vorrats nicht bekommen konnten?

Nein, wenn ein Kunde seine Abonnementbestellung storniert oder ein Produkt aus der Bestellung entfernt, wird dieser Bestand wieder dem Wert in "Verfügbar" zugeordnet. Er wird nicht automatisch anderen Kunden zugewiesen, aber Sie können diesen Bestand jetzt manuell der Bestellung eines anderen Kunden hinzufügen, indem Sie [dessen Bestellung bearbeiten](../orders/view-orders.md#einen-auftrag-bearbeiten).

### Kann ich oder der Kunde eine Bestellung bearbeiten, die über das Abonnement-System aufgegeben wurde?

Dies hängt davon ab, ob Sie Produkte hinzufügen oder entfernen möchten:

* Als Unternehmensleiter können Sie Produkte entfernen (oder eine Bestellung stornieren), die über das Abonnement-System über das OFN-Administrationspanel auf die[ übliche Weise ](../orders/view-orders.md#einen-auftrag-bearbeiten)aufgegeben wurden.
* Wenn Sie als Unternehmensleiter einer Bestellung, die vom Abonnement-System über das [OFN-Administrationspanel ](../orders/view-orders.md#einen-auftrag-bearbeiten)aufgegeben wurde, Produkte hinzufügen, löst dies [eine zweite Zahlung](../orders/refunds-and-adjusting-payments.md#einziehung-zusaetzlicher-zahlungen) aus, die am Ende des Bestellzyklus nicht automatisch verarbeitet wird.
* Wenn Sie Kunden die Möglichkeit geben,[ Bestellungen zu bearbeiten oder zu stornieren](../enterprise-profile/enterprise-settings.md#shop-einstellungen), während der Bestellzyklus noch läuft, können sie Artikel aus ihrer Abonnementbestellung entfernen. Um Artikel hinzuzufügen, müssen sie eine zweite Bestellung erstellen und die Kasse wie gewohnt besuchen.

