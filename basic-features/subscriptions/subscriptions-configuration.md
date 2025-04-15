# Konfiguration

## Aktivieren von Abonnements

Um die Abonnementfunktion für Ihr Unternehmen zu aktivieren, gehen Sie zu Unternehmen-> Einstellungen-> [Laden](../enterprise-profile/enterprise-settings.md#shop-einstellungen).

Ändern Sie unten auf der Seite Abonnements auf "aktiviert".

![](../../.gitbook/assets/subscriptions1.jpg)

**Gastbestellungen:** Für Unternehmen mit aktivierten Abonnements empfehlen wir, dass sich alle Kunden anmelden müssen, bevor sie bei Ihnen einkaufen können. Dadurch wird sichergestellt, dass jeder Kunde mit einem Abonnement sich anmeldet und seine bestehende Abonnementbestellung sieht und nicht versehentlich eine Doppelbestellung aufgibt.

**Aufträge ändern:** Für Kunden mit einem Abonnement von Ihrem Unternehmen, wirken sich die Optionen für diese Einstellung wie folgt aus:

* _Erteilte Aufträge können nicht geändert/storniert werden:_ Der Kunde muss sich mit Ihnen in Verbindung setzen, um seine reguläre Bestellung zu ändern (Änderung der Mengen der einzelnen gewünschten Produkte oder Stornierung der Bestellung).
* _Kunden können Bestellungen ändern/stornieren, während der Bestellzyklus offen ist:_ Der Kunde kann die Menge der Produkte, die er in seinem Abonnement wünscht, ändern und/oder die gesamte Bestellung stornieren.

{% hint style="info" %}
Wenn ein Kunde mit einer Abonnementbestellung ein Produkt kaufen möchte, das nicht Teil seiner regulären Bestellung ist, muss er in jedem Fall einen zweiten Warenkorb anlegen und zur Kasse gehen. **Weder Sie noch der Kunde können neue Produkte zu seiner Abonnementbestellung hinzufügen, sobald der Bestellzyklus geöffnet ist.**
{% endhint %}

## Versand- und Zahlungsarten für Abonnements

Wenn Sie das Abonnement des Kunden erstellen, müssen Sie die Lieferoption und die Zahlungsart auswählen, mit der der Kunde bezahlt werden soll. Dies gilt dann für alle folgenden Abonnements-Bestellungen für den Kunden.

### Lieferoptionen

Sie können jede [Versand-/Liefermethode](subscriptions-configuration.md#versandmethoden) für ein Abonnement verwenden.

### Zahlungsmöglichkeiten

Sie können Abonnements nur zwei Arten von [Zahlungsarten](../shopfront/payment-methods.md) zuordnen.

1. **Manuelle Zahlungsarten:** Bargeld, Scheck, Banküberweisung (d. h. jede Methode, die keine automatische Online-Validierung durch die OFN-Plattform beinhaltet).
2. **Stripe**: Stripe ist eine Zahlungs-Schnittstelle, die Zahlungen mit Kreditkarten entgegennimmt. Einzelheiten darüber, wie Sie Stripe-Zahlungen für Ihr Unternehmen konfigurieren, finden Sie [hier](../shopfront/payment-methods.md#integrierte-zahlungsanbieter).

{% hint style="info" %}
Bei jeder Bestellung, die automatisch durch ein Abonnement aufgegeben wird, wird die Bankkarte des Kunden für die Bestellung belastet (bei Abschluss des entsprechenden Bestellzyklus). Der belastete Betrag spiegelt alle Änderungen wider, die Sie oder der Kunde an der Bestellung vorgenommen haben.\
Den Kunden werden keine Kosten in Rechnung gestellt, wenn sie ihre Abonnementbestellung stornieren.
{% endhint %}

{% hint style="warning" %}
Damit der Kunde korrekt belastet werden kann, muss er ein Konto auf der Open Food Network-Plattform haben. Auf ihrem OFN-Konto müssen sie eine Standard-Kreditkarte registriert und ihrem Unternehmen die Erlaubnis erteilt haben, von dieser Karte abzubuchen. Weitere Informationen finden Sie [hier](subscriptions-the-customers-perspective.md#speichern-von-kreditkarten-und-autorisierung-von-gebuehren).
{% endhint %}

{% hint style="success" %}
Wenn Sie Stripe als Zahlungsmethode für Abonnements verwenden, ist es für den Kunden hilfreich, wenn Sie eine klare, detaillierte Erklärung hinzufügen, wie die Zahlung abgewickelt wird, wenn er diese Option wählt.\
\
Anstatt die [Zahlungsmethode](../shopfront/payment-methods.md) "Kreditkarte" zu nennen, könnten Sie sie zum Beispiel "automatische Kreditkartenabrechnung für Abonnements" nennen. Eine mögliche Beschreibung könnte lauten: "Ihre in Ihrem OFN-Konto gespeicherte Standardkreditkarte wird belastet, wenn Ihre Abonnementbestellung am Mittwochabend bestätigt wird". Dieser Name und die Beschreibung werden in der E-Mail-Bestätigung für Abonnement-Kunden erscheinen (siehe Beispiel unten), daher ist es gut, sie detailliert anzugeben, damit der Kunde weiß, was ihn erwartet.
{% endhint %}

![](<../../.gitbook/assets/image (15) (1).png>)

## Sammeln Sie Informationen von Ihren Kunden

Um ein Abonnement für einen Kunden einzurichten, müssen Sie einige Informationen von ihm erhalten, wie unten beschrieben:

**Name, Telefonnummer und E-Mail Adresse:** Denken Sie daran, dass jeder Kunde, der eine automatisierte regelmäßige Bestellung (Abonnement) bei Ihrem Unternehmen aufgeben möchte, ein registriertes und bestätigtes Benutzerkonto auf der OFN-Plattform haben MUSS. Kunden mit Abonnements müssen auf der [Kundenliste](../shopfront/customer-management-and-conditional-displays-prices/customers.md) Ihres Unternehmens stehen. Siehe unten für [weitere](subscriptions-configuration.md#fuegen-sie-ihre-abonnenten-zu-ihrer-kundenliste-hinzu) Details.

**Rechnungs- und Lieferadresse**

**Produkte:** Welche Produkte möchten sie in ihr Abonnement aufnehmen?

**Versand-/Zustellungsmethode:** Sie müssen der Abonnementbestellung eine Versand-/Liefer-/Abholmethode zuweisen. Wie möchten sie die Waren erhalten?

**Zahlungsmethode**: Kunden können zwischen manuellen Zahlungsmethoden (z.B. Barzahlung, Banküberweisung) oder der Zahlung mit Kreditkarte über das Stripe-Konto Ihres Shops wählen. Wenn der Kunde seine Abonnementbestellungen über Stripe bezahlen möchte, muss er eine Standardzahlungskarte hinzufügen und eine Autorisierung erteilen. Siehe [hier](subscriptions-the-customers-perspective.md#speichern-von-kreditkarten-und-autorisierung-von-gebuehren) für weitere Details.

**Start- und Enddatum für ihre Abonnementaufträge:** Damit ein Abonnementauftrag für einen bestimmten Auftragszyklus erstellt werden kann, muss er ein Startdatum haben, das entweder vor oder nach dem Eröffnungsdatum des Bestellzyklus liegt, und das Enddatum des Abonnements muss nach dem Abschlussdatum des Bestellzyklus liegen.

## Fügen Sie Ihre Abonnenten zu Ihrer Kundenliste hinzu

Bevor Sie einen Abonnementauftrag für einen Kunden einrichten können, muss dieser zu Ihrer [Kundenliste](../shopfront/customer-management-and-conditional-displays-prices/customers.md) hinzugefügt werden.

**Nachdem Sie Ihre Kunden zu Ihrer Kundenliste hinzugefügt haben**, schicken Sie ihnen eine E-Mail und bitten sie, [sich für ein OFN-Konto anzumelden](subscriptions-the-customers-perspective.md#anmeldung-bei-ofn). Wenn Sie vorhaben, Ihre Kunden über Stripe abzurechnen, müssen Sie sie außerdem auffordern, die [hier](subscriptions-the-customers-perspective.md#speichern-der-kreditkartendaten-im-kundenkonto) beschriebenen zusätzlichen Schritte zu befolgen, um ihrem OFN-Benutzerkonto eine Standard-Kredit-/Debitkarte hinzuzufügen und Ihrem Unternehmen die Genehmigung zu erteilen, Zahlungen entgegenzunehmen.

{% hint style="info" %}
Sie können Kunden zu Ihrer Kundenliste hinzufügen, bevor oder nachdem sie sich für ein Konto bei OFN angemeldet haben. Bevor ein Abonnementauftrag erfolgreich eingerichtet werden kann, muss der Kunde jedoch die E-Mail-Adresse bestätigen, auf die sein OFN-Konto registriert ist.
{% endhint %}

{% hint style="warning" %}
Wenn Sie einen Kunden für seine Abonnementbestellung über Stripe belasten möchten, muss er zu Ihrer [Kundenliste](../shopfront/customer-management-and-conditional-displays-prices/customers.md) hinzugefügt werden, BEVOR er Ihr [Unternehmen ermächtigen kann](subscriptions-the-customers-perspective.md#speichern-von-kreditkarten-und-autorisierung-von-gebuehren), Zahlungen von seiner Kredit-/Debitkarte zu nehmen.\
Wir empfehlen daher das folgende Verfahren:

1. Setzen Sie sich mit dem Kunden in Verbindung und holen Sie alle erforderlichen Informationen ein (siehe [oben](subscriptions-configuration.md#sammeln-sie-informationen-von-ihren-kunden)).
2. Fügen Sie sie zu Ihrer [Kundenliste](../shopfront/customer-management-and-conditional-displays-prices/customers.md) hinzu.
3. Senden Sie dem Kunden eine E-Mail, in der Sie ihn auffordern, sich bei [OFN für ein Konto zu registrieren](subscriptions-the-customers-perspective.md#anmeldung-bei-ofn) und seine [Kredit-/Debitkartendaten zu diesem Konto hinzuzufügen](subscriptions-the-customers-perspective.md#speichern-von-kreditkarten-und-autorisierung-von-gebuehren).
4. [Erstellen Sie das Abonnement.](subscriptions-creating-and-managing-orders.md)
{% endhint %}

## Zeitpläne

{% hint style="info" %}
Wenn Sie neu bei OFN sind, empfehlen wir Ihnen, sich mit der Einrichtung von [Bestellzyklen](../shopfront/order-cycle/) vertraut zu machen, bevor Sie Zeitpläne und Abonnements einrichten.
{% endhint %}

### Über Zeitpläne

Abonnements sind so eingerichtet, dass jedes Mal, wenn ein Unternehmen einen Bestellzyklus öffnet, automatisch Bestellungen für Kunden generiert werden können, die ein Abonnement bei diesem Shop haben. Die Häufigkeit, mit der eine Abonnementbestellung für einen bestimmten Kunden aufgegeben wird (d. h. welcher Ihrer aktiven Bestellzyklen sein Abonnement auslöst), wird über eine Funktion namens "**Zeitpläne**" gesteuert.

Zeitpläne sind Gruppen, denen Bestellzyklen zugeordnet werden können. Sobald ein Zeitplan erstellt wurde, werden Kundenabonnements auf den Zeitplan angewendet, so dass eine Bestellung für ihr Abonnement nur für neue Bestellzyklen in diesem Zeitplan generiert wird.

{% hint style="info" %}
In diesem Fall würden Sie ihre Abonnements zu einem Zeitplan hinzufügen, der alle Ihre wöchentlichen Bestellzyklen umfasst. Für andere Kundengruppen, die nur vierzehntägige/monatliche Bestellungen wünschen, können Sie zusätzliche Zeitpläne erstellen, die nur abwechselnd/einmal pro Woche einen Ihrer wöchentlichen Bestellzyklen enthalten.
{% endhint %}

{% hint style="success" %}
Dieses Arrangement ist sehr flexibel, so dass Sie ruhig experimentieren können, um die für Ihr Unternehmen am besten geeignete Kombination aus Bestellzyklus und Zeitplan zu finden. Sie können zum Beispiel "ungerade Wochen" und "gerade Wochen", "Großhandel", "monatliches Fleisch"....
{% endhint %}

### Einen Zeitplan erstellen

Wenn Sie alle oben beschriebenen Schritte durchgeführt haben, erscheint die Schaltfläche **+Neuer Zeitplan** oben in Ihrem Menü Bestellzyklen:

![](<../../.gitbook/assets/ordercycle1 (2) (2).jpg>)

{% hint style="warning" %}
Sie müssen mindestens einen offenen oder zu öffnenden Bestellzyklus haben, um einen neuen Zeitplan erstellen zu können.
{% endhint %}

![](../../.gitbook/assets/new-schedule.bin)

**Name:** Geben Sie dem Zeitplan einen logischen Namen, der diese Gruppe von Bestellzyklen beschreibt. Z.B. 'wöchentlich', 'monatlich', 'Dienstagslieferungen', 'Großhandel' oder 'Einzelhandel'. Dieser Name ist für die Kunden nicht sichtbar.

{% hint style="info" %}
Wenn Sie mehrere OFN-Unternehmen verwalten und die Abonnements in mehr als einem Unternehmen aktiviert sind, müssen Sie Ihre Zeitpläne eindeutig benennen, z. B. weekly\_hubA, weekly\_hubB, fortnightly\_hubA, fortnightly\_hubB.\
Jedes Unternehmen benötigt einen anderen Zeitplan, aber wenn Sie ein Abonnement für einen Kunden erstellen, werden die Zeitpläne für alle Ihre Unternehmen angezeigt. Daher hilft Ihnen der beschreibende Name sicherzustellen, dass das Abonnement für das richtige Unternehmen für diesen bestimmten Kunden erstellt wird.
{% endhint %}

Sie können bestehende Bestellzyklen in den neuen Zeitplan einfügen und aus ihm herausnehmen, indem Sie auf die Schaltflächen "<" und ">" klicken.

Klicken Sie auf Erstellen, wenn Sie fertig sind.

### Bearbeiten oder Löschen eines Zeitplans

Um einen Zeitplan zu bearbeiten oder zu löschen, klicken Sie auf den Namen des Zeitplans neben dem entsprechenden Bestellzyklus in der Spalte "Zeitpläne". (Möglicherweise müssen Sie die Spalte "Zeitpläne" sichtbar machen, indem Sie sie im Dropdown-Spaltenmenü oben rechts anklicken).

![](../../.gitbook/assets/show-schedules.bin)

Sie können den Namen des Zeitplans ändern, Bestellzyklen hinzufügen/entfernen oder den Zeitplan löschen.

![](../../.gitbook/assets/delete-schedule.bin)

{% hint style="danger" %}
Sie können einen Zeitplan nicht löschen, wenn er mit Abonnements verbunden ist.
{% endhint %}

### Hinzufügen oder Entfernen von Bestellzyklen aus Zeitplänen

Sie können Bestellzyklen aus Zeitplänen hinzufügen und entfernen, indem Sie entweder den Zeitplan bearbeiten (siehe [oben](subscriptions-configuration.md#bearbeiten-oder-loeschen-eines-zeitplans)) oder den Bestellzyklus bearbeiten und den Zeitplan im Feld "Zeitpläne" hinzufügen/entfernen:

![](../../.gitbook/assets/ordercycle3.jpg)

{% hint style="success" %}
Bestellzyklen können in mehr als einem Zeitplan enthalten sein. Wenn Ihre Bestellzyklen beispielsweise wöchentlich sind, Sie aber drei Zeitpläne haben (wöchentlich, vierzehntägig-ungerade Wochen und vierzehntägig-gerade Wochen), dann kann ein Bestellzyklus sowohl mit dem "wöchentlichen" als auch mit dem "vierzehntägig-ungeraden" Wochenzeitplan verbunden sein.
{% endhint %}

