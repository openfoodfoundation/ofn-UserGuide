# Fehlersuche

{% hint style="success" %}
Speichern oder aktualisieren Sie immer am Ende jeder Änderung, die Sie vornehmen. Die Änderungen gehen verloren, wenn Sie zu einer anderen Seite wechseln, ohne zu speichern. Manchmal werden Sie nicht zum Speichern aufgefordert.
{% endhint %}

## Es lässt mich keinen Auftragszyklus einrichten

* Haben Sie eine aktive [Zahlungsmethode](basic-features/shopfront/payment-methods.md) für Ihren Shop oder Hub eingerichtet?
* Haben Sie eine aktive [Versandmethode](basic-features/shopfront/shipping-methods.md) für Ihren Shop oder Hub eingerichtet?
* Sind alle [relevanten Pflichtfelder ausgefüllt](basic-features/shopfront/order-cycle/)? Sie müssen Öffnungs- und Schließzeiten für den Auftragszyklus festlegen, ihm einen eindeutigen Namen geben und das Feld "Bereit für" ausfüllen.

## Ich möchte ganze Hühner verkaufen, kenne aber das Gewicht der einzelnen Tiere erst am Tag der Schlachtung.

* Das ist kein Problem! Lesen Sie [hier](basic-features/products-1/pricing-irregular-items-kg.md) eine Reihe von Möglichkeiten, wie die OFN-Plattform so flexibel gestaltet wurde, dass sie den spezifischen Bedürfnissen von Lebensmittelherstellern gerecht wird.

## Ich liefere dem "Hofladen A" Kartoffeln zum Preis von 1 £/kg. Meine Kartoffeln werden zum Verkauf an Kunden zu 1,20 £/kg angeboten.

Hofladen A muss möglicherweise bei jedem Verkauf zusätzliche Einnahmen erzielen, um seine Gemeinkosten zu decken. Dies kann auf verschiedene Weise geschehen:

* Wenn Sie eine [Unternehmensgenehmigung](basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) einrichten, mit der Ihr Unternehmen dem Hofladen A erlaubt, Ihre Produkte in seinen Bestand aufzunehmen, kann er auf diese Weise die Preise ändern, die ein Kunde für Ihre Produkte bezahlt.
* Farmshop A kann auf Ihren [Selbstkostenpreis](basic-features/shopfront/enterprise-fees.md) für die Kartoffeln eine Unternehmensgebühr aufschlagen. Wenn dies der Fall ist, können Kunden, die die Artikel kaufen, eine Aufschlüsselung des Preises sehen, den sie zahlen, indem sie auf das Tortendiagramm-Symbol rechts neben dem Produktpreis auf der Ladenfront klicken.

Gute Arbeitsbeziehungen sind der Schlüssel zu jedem nachhaltigen Lebensmittelnetzwerk. Sprechen Sie mit Hofladen A darüber, wie er den Verkauf Ihrer Produkte organisiert hat (entweder persönlich, telefonisch oder per E-Mail).

Hofladen A sollte Ihnen (aus moralischen Gründen) für jedes Kilogramm Kartoffeln, das Sie liefern, 1 £/kg zahlen, um seine Verkäufe zu decken. Die Bezahlung der Waren (vom Händler an den Lieferanten) ist eine private Vereinbarung, die außerhalb der OFN-Plattform getroffen wird.

## Ich habe neue Produkte hinzugefügt, aber sie werden nicht im Schaufenster angezeigt.

Neu hinzugefügte Produkte müssen einem aktiven Bestellzyklus hinzugefügt werden, bevor sie im Schaufenster für die Kunden sichtbar sind und gekauft werden können.

* Wenn Sie die **Waren an einen Hub liefern**, müssen Sie sich mit der Person in Verbindung setzen, die den betreffenden Auftragszyklus koordiniert. Dies muss außerhalb der OFN-Plattform geschehen (per E-Mail oder telefonisch/persönlich).
* Wenn Sie ein **Shop** sind, müssen Sie die neuen Produkte zu Ihrem [aktiven, offenen Bestellzyklus hinzufügen](basic-features/shopfront/order-cycle/).
* Wenn Sie ein Hub sind, dann:
  * Stellen Sie sicher, dass die neuen Produkte sowohl dem Eingangs- als auch dem Ausgangsbereich des [aktiven Auftragszyklus](basic-features/shopfront/order-cycle/) hinzugefügt werden.
  * Wenn die neuen Produkte nicht für die Auswahl verfügbar sind, um sie entweder in den Eingangs- oder Ausgangsbereich aufzunehmen, überprüfen Sie Ihre [Bestandseinstellungen](basic-features/enterprise-profile/enterprise-settings.md#inventar-einstellungen). Möglicherweise müssen Sie die Produkte erst zu [Ihrem Inventar hinzufügen](basic-features/products-1/inventory-tool.md#ueberpruefung-neuer-produkte), bevor sie der Shopfront hinzugefügt werden können.

{% hint style="info" %}
Überprüfen Sie in jedem Fall den Lagerbestand der neuen Produkte. Nur Artikel mit einem Wert von 1 oder höher auf Lager oder solche, die als **unbegrenzt** markiert sind, werden für einen Kunden zum Kauf angezeigt.
{% endhint %}

## Nicht alle Produkte meines Lieferanten sind für mich verfügbar, um sie in meinen Bestellzyklus aufzunehmen.

Möglicherweise haben Sie in Ihren [Inventareinstellungen](basic-features/enterprise-profile/enterprise-settings.md#inventar-einstellungen) die Option "Neue Produkte müssen meinem Inventar hinzugefügt werden, bevor sie meinem Schaufenster hinzugefügt werden können" eingestellt.\
In diesem Fall müssen Sie Ihren Produktbestand überprüfen und [neue/ausgeblendete Produkte](basic-features/products-1/inventory-tool.md#verwaltung-ihres-lagerbestands-produkte) zum Bestand hinzufügen, damit sie im Bestellzyklus zur Auswahl stehen.

Wenn Sie einen Bestellzyklus koordinieren, an dem mehrere Lieferanten und Händler beteiligt sind, von denen einige oder alle ihren Produktbestand für die Bestückung ihrer Schaufenster verwenden können, sollten Sie überprüfen, ob alle relevanten Unternehmensgenehmigungen erteilt wurden. Lesen Sie [hier](basic-features/shopfront/order-cycle/permissions-in-multi-enterprise-order-cycles.md) mehr.

## Ein neuer Produzent hat in der Nähe eröffnet, aber ich kann seine Produkte nicht in meine Hub-Shopfront aufnehmen.

Sie müssen deren Erlaubnis einholen, bevor Sie die von ihnen hergestellten oder gelieferten Waren verkaufen können. Dies geschieht formell auf der OFN-Plattform durch den neuen Hersteller über [Unternehmensgenehmigungen](basic-features/shopfront/enterprise-fees.md).

## Ich habe ein Gemüsekistenprogramm, möchte aber den Kunden die Möglichkeit geben, ihrer Bestellung jede Woche zusätzliche Artikel hinzuzufügen, wenn sie dies wünschen.

**Szenario eins:** Der Kunde kauft jede Woche die Gemüsekiste über ein automatisches [Abonnement](basic-features/subscriptions/), das auf der OFN-Plattform eingerichtet ist:\
Ändern Sie Ihre [Unternehmenseinstellungen](basic-features/enterprise-profile/enterprise-settings.md#zugriff-auf-ihre-unternehmenseinstellungen)-> Shop-Einstellungen-> Bestellungen ändern? auf 'Kunden können Bestellungen ändern/stornieren, während der Bestellzyklus offen ist'.\
Wenn der Bestellzyklus eröffnet wird, erhält der Kunde eine automatische E-Mail, in der er darüber informiert wird, dass seine Gemüsekisten-Bestellung erstellt worden ist. Er hat dann bis zum Ende des Bestellzyklus Zeit, sich in sein OFN-Konto einzuloggen, seine Bestellung zu bearbeiten und zusätzliche Artikel aus Ihrem Shop in den Warenkorb zu legen.

{% hint style="info" %}
Die zusätzlichen Artikel werden als separate Bestellung bearbeitet. Der Kunde wird zur Kasse geleitet, um für diese Artikel zu bezahlen. Die Zahlung für die Abonnementbestellung wird am Ende des Bestellvorgangs automatisch eingezogen.
{% endhint %}

**Szenario zwei:** Der Kunde kauft eine Gemüsekiste über eine externe Plattform. Richten Sie in diesem Fall vielleicht ein [privates Schaufenster](basic-features/shopfront/private-shopfront.md) ein, das nur für Kunden sichtbar ist, die bei Ihrem externen Gemüsekistenprogramm angemeldet sind. Verwenden Sie externe Software oder Tabellenkalkulationen, um zusätzliche Artikel, die über die OFN-Schaufensterfront gebracht werden, den Gemüsekisten der Kunden zuzuordnen, so dass Sie nur einmal liefern müssen!

## Es gab eine Missernte und wir haben weniger Tomaten geliefert, als wir brauchen, um alle Bestellungen zu erfüllen.

Kein Problem - das passiert jedem ab und zu! Lesen Sie [hier](basic-features/orders/view-orders.md#beispiele-fuer-die-verwendung-von-bulk-order-management), wie Sie alle Bestellungen Ihrer Kunden auf einmal anpassen können.

## Ein Produzent ist nur dann bereit, meinen Hub zu beliefern, wenn seine Bestellungen ein Mindestkriterium erfüllen

Die [hier](basic-features/products-1/group-buy-for-bulk-ordering.md) beschriebene Funktion des "Gruppeneinkaufs" kann auch für diesen Zweck genutzt werden!

## Ich kann einem Kunden, der mit PayPal bezahlt hat, kein Geld zurückerstatten.

Derzeit können Sie keine Rückerstattungen an Kunden ausstellen, die Waren per PayPal direkt über die OFN-Plattform gekauft haben. Sie müssen Ihr geschäftliches PayPal-Konto besuchen und dort die Rückerstattung an den Kunden manuell vornehmen. Wir hoffen, dass wir diese Funktion in Zukunft entwickeln können, wenn genügend Nutzer dies wünschen.

{% hint style="warning" %}
Wenn keiner dieser Schritte hilft oder Sie ein anderes Problem haben, wenden Sie sich bitte an Ihr [örtliches OFN-Supportteam](local-ofn-organizations-and-contacts.md), das sein Bestes tun wird, um Ihnen so schnell wie möglich Lösungen und Hilfe anzubieten.
{% endhint %}

## Wie können meine Kunden ihre Bestellungen bearbeiten, nachdem sie aufgegeben wurden?

Gelegentlich kommt es vor, dass ein Kunde eine Bestellung bei Ihrem Lebensmittelunternehmen aufgibt und es sich dann anders überlegt oder sich erinnert, dass er vergessen hat, ein paar Artikel hinzuzufügen. Es gibt einige Szenarien:

#### Dem Kunden die Möglichkeit geben, seine eigenen Bestellungen zu bearbeiten

In Ihren [Unternehmenseinstellungen](basic-features/enterprise-profile/enterprise-settings.md#shop-einstellungen) können Sie auf der Registerkarte "Shop-Einstellungen" die Option "Änderungsaufträge" aktivieren.

![](.gitbook/assets/changeorders.jpg)

Das bedeutet, dass die Kunden dies tun können:

* Artikel aus dem Warenkorb entfernen oder die Bestellung ganz stornieren.
* die Menge der bereits im Warenkorb befindlichen Produkte erhöhen, sofern die Bestellung nicht über das Abonnement-System erfolgt ist.

{% hint style="warning" %}
Die Kunden können keine weiteren Produkte in den Warenkorb legen. Wenn sie dies tun, werden sie erneut zur Kasse geleitet, um für diese Artikel zu bezahlen. Die beiden Bestellungen erscheinen jedoch nacheinander in Ihren Berichten, wenn sie nach Kundennamen sortiert sind, so dass sie zusammen verpackt werden können (wenn Sie es wünschen), wenn Sie die Abholung vorbereiten.
{% endhint %}

#### Aufträge nur im Namen Ihres Kunden bearbeiten

Sie können eine Nachricht auf Ihrer [Schaufenster-Seite hinzufügen](basic-features/enterprise-profile/enterprise-settings.md#shop-einstellungen), in der Sie Ihre Kunden bitten, sich per E-Mail oder Telefon mit Ihnen in Verbindung zu setzen, wenn sie ihre Bestellungen ändern möchten. Mit den [hier](basic-features/orders/view-orders.md#einen-auftrag-bearbeiten) beschriebenen Schritten können Sie Produkte zu Bestellungen hinzufügen oder aus ihnen entfernen.

{% hint style="warning" %}
Beachten Sie, dass das Hinzufügen von Artikeln zu einer Bestellung [zusätzliche Zahlungen](basic-features/orders/refunds-and-adjusting-payments.md#einziehung-zusaetzlicher-zahlungen) erforderlich macht.
{% endhint %}

#### Der Auftrag wurde durch ein Abonnement erteilt.

Informationen zur Bearbeitung einer Bestellung, die über das Abonnement-System aufgegeben wurde, finden Sie unter:

* [hier](basic-features/subscriptions/subscriptions-faqs.md#kann-ich-oder-der-kunde-eine-bestellung-bearbeiten-die-ueber-das-abonnement-system-aufgegeben-wurde) für einmalige Bestellungen
* [hier](basic-features/subscriptions/subscriptions-faqs.md#was-passiert-wenn-ich-das-abonnement-aendere-waehrend-es-offen-ist) für die Bearbeitung des Basisabonnementauftrags.
