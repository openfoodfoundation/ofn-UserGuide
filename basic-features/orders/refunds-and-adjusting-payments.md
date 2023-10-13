# Erstattungen und Anpassung der Zahlungen

Von Zeit zu Zeit kann ein Kunde verlangen, dass seine Bestellung angepasst wird, z. B. durch Hinzufügen oder Entfernen eines Artikels.

In anderen Fällen kann es vorkommen, dass Sie als Geschäftsleiter einen Auftrag ändern müssen. Häufige Szenarien sind:

1. Ein Produkt wurde von einem Lieferanten nicht geliefert
2. Ein Produkt war von geringerer Qualität als erwartet
3. Eine Bestellung enthält Produkte mit variablem Gewicht, wie z. B. [Fleisch oder große Gemüsesorten](../products-1/pricing-irregular-items-kg.md#option-eins-festsetzung-eines-durchschnittsgewichts-preises-und-erstattung) (d. h. ganze Artikel mit Preisangaben nach Gewicht).

Das Verfahren für die Rückerstattung oder die Aufforderung zur weiteren Zahlung hängt von der verwendeten [Zahlungsmethode](../shopfront/payment-methods.md) ab.

{% hint style="warning" %}
Auf der OFN-Plattform können Rückerstattungen und zusätzliche Zahlungen nur automatisch über den Zahlungsmittelanbieter Stripe/Stripe SCA erfolgen.
{% endhint %}

## Erstattungen

Über die OFN-Plattform können Sie eine Gesamterstattung vornehmen, bei der der gesamte Betrag der Bestellung erstattet wird, oder eine Teilerstattung, die Sie z. B. verwenden können, wenn ein Artikel nicht verfügbar war.

{% hint style="warning" %}
Wenn Sie Stripe als Zahlungsmethode integriert haben, können Sie sich in Ihr Stripe-Konto einloggen und dem Kunden über Stripe eine Rechnung ausstellen. Der Kunde erhält eine E- Mail, in der er aufgefordert wird, mit einer Kredit- oder Debitkarte zu zahlen. Beachten Sie jedoch, dass OFN nicht über diese Transaktion benachrichtigt wird und Sie die Zahlung weiterhin manuell in OFN erfassen müssen.
{% endhint %}

### Erstattung insgesamt

Um eine vollständige Rückerstattung vorzunehmen, wählen Sie die entsprechende Zahlungsmethode aus den nachstehenden Registerkarten aus:

{% tabs %}
{% tab title="Bargeld/BACS" %}
Für nicht automatisierte Zahlungsmethoden (wie Barzahlung bei Abholung oder BACS) gibt es zwei Szenarien:

\
**Der Kunde hat den Artikel noch nicht bezahlt.**\
Wenn ein Kunde eine Bestellung aufgibt und eine Zahlungsmethode wie Barzahlung bei Abholung oder BACS auswählt und die Zahlung nicht im System erfasst wurde, wird dies angezeigt:

![](https://lh6.googleusercontent.com/9lIYAkArDP1yllI88\_N00rOQYiQqu9KG-piADA0hJtUvelv1NZAPNOx0Q9Ph3a6yu1gal9zUuFgJox0xiRC4RM4UlwmcfCdspcSlG9w\_m23a8Cv\_SnWI8yfgNIBnfClRx3MJ7Ru0)

Sie können die [Bestellung sofort stornieren](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled), indem Sie die folgenden Schritte ausführen.

**Der Kunde hat den Artikel bezahlt.**

Wenn [Anzeigen von Bestellungen](view-orders.md#auflistung-der-auftraege) erscheint die Bestellung als:

![](https://lh5.googleusercontent.com/7Uorian\_j1n-fPDTQQSeSiHr1tcDQczsaCb\_WSxIKRt1PRp1S3l4bKhaFA6WfMaiEsGgN0Qx5OdLfi\_lBK9yz1r5-Oh0AcZKkM0MfrbfOzQCpejuQLWvAMRNFCom9-r-S2ZfqMjt)

1. Veranlassen Sie, dass dem Kunden die Kosten unabhängig von der OFN-Plattform erstattet werden.
2. Record this action by [**Orders -> Edit**](view-orders.md#editing-an-order) and select the ‘Payments’ tab from the right hand menu. &#x20;
3. Erfassen Sie diese Aktion über [Aufträge -> Bearbeiten](view-orders.md#einen-auftrag-bearbeiten) und wählen Sie im rechten Menü die Registerkarte "Zahlungen".\
   Wählen Sie das "X" rechts neben der Zahlung, um sie zu stornieren.

![bevor Sie die Zahlung als ungültig markieren.](https://lh6.googleusercontent.com/1mhZhKoPtqPZVZIDz\_VV4-8uBy5BefLVo9SftwfecciD7sJCGZhwgEWb-PeYAPI01w3AOZ0x\_d7oWpMTQpLBqv201qb8VtmFjB1SaK0nChsy7knCt\_EVQwlaioEPTtBZSUQLuLQa)

![Nach der Kennzeichnung der Zahlung als ungültig.](https://lh6.googleusercontent.com/ui2lGGDHK7Pp6KZQ34UHg4KERF9eGDgQKHg3YIr20B8J0oyObiCVic5hOuvpR5HOK16dvvR8aCx70LYnPE-kKN2AKBfPkz3nXvhAM17oYgdPLmDhJiApl7-w\_vfDKog2p8iFAKcY)

[Markieren Sie dann die Bestellung als "storniert",](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled) indem Sie die folgenden Schritte ausführen.
{% endtab %}

{% tab title="Stripe" %}
Die Zahlung für die Bestellung wird automatisch bei der Erstellung eingezogen (außer bei [Abonnements](../subscriptions/)), so dass die Bestellung in der [Liste der Bestellungen](view-orders.md#auflistung-der-auftraege) als solche erscheint:

![](https://lh6.googleusercontent.com/9\_eN8vGTnyWSL997ebeYQeasxhaiOGKlkwLFydvAHJGiXvUgCR1CmuPRl-fZ4DbwUw3tVNnSSEI7S8M7ZqnYrkGdPkvRHvBpPKmhK47wjFCXfDrF8VUanpBe8NdErg-3nl6b549y)

Gehen Sie zu [**Bestellungen -> Bearbeiten**](view-orders.md#einen-auftrag-bearbeiten) und wählen Sie im rechten Menü "Zahlungen". Klicken Sie auf das "**X**" rechts neben der Zahlung, um sie zu stornieren.

![](../../.gitbook/assets/stripetotal.jpg)

Dadurch wird die Zahlung automatisch an die vom Kunden verwendete Kredit- oder Debitkarte zurücküberwiesen.

{% hint style="info" %}
Beachten Sie, dass es 3 bis 5 Arbeitstage dauern kann, bis Stripe-Zahlungen auf dem Kontoauszug eines Kunden erscheinen.
{% endhint %}

Wenn Sie eine Rückerstattung vorgenommen haben, gehen Sie wie folgt vor, um die [Bestellung zu stornieren](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled).
{% endtab %}

{% tab title="PayPal" %}
Die Zahlung wird automatisch an der Kasse vom Kunden eingezogen, so dass die [Bestellung in der Auflistung](view-orders.md#auflistung-der-auftraege) Aufträge als angezeigt wird:

![](https://lh6.googleusercontent.com/9\_eN8vGTnyWSL997ebeYQeasxhaiOGKlkwLFydvAHJGiXvUgCR1CmuPRl-fZ4DbwUw3tVNnSSEI7S8M7ZqnYrkGdPkvRHvBpPKmhK47wjFCXfDrF8VUanpBe8NdErg-3nl6b549y)

{% hint style="danger" %}
**Bestellungen, die über PayPal aufgegeben und bezahlt wurden, können nicht über die OFN-Plattform erstattet werden.**
{% endhint %}

![](../../.gitbook/assets/pp.jpg)

Um dem Kunden das Geld zurückzuerstatten, müssen Sie sich in Ihr [PayPal-Konto ](https://www.paypal.com/)einloggen und das Geld über die Schnittstelle auf das Konto des Kunden zurücküberweisen.

Danach können Sie die Bestellung mit den folgenden Schritten als [storniert markieren](refunds-and-adjusting-payments.md#marking-an-order-as-cancelled).
{% endtab %}
{% endtabs %}

#### Einen Auftrag als storniert markieren

Sobald Sie eine Erstattung vorgenommen haben, können Sie die Bestellung stornieren.[ Bearbeiten Sie die Bestellung](view-orders.md#einen-auftrag-bearbeiten) und wählen Sie "Bestellung stornieren" unter "Aktionen" (blaue Schaltfläche oben rechts)

![](https://lh6.googleusercontent.com/V3A6girSx2xUYYW9Jp3VIp41YZrgSq7JaicQlLWUrcVqA1u6SzFjagJkg0KLIL05LgRBXErJyk\_iLVrBwt9metOp\_RqXmSKL8dRCxFtj6VqTEDjx7z\_NHERFNJPw-CdOlNGGmBYp)

{% hint style="success" %}
Der Kunde erhält eine E-Mail, in der er darüber informiert wird, dass seine Bestellung storniert wurde.
{% endhint %}

{% hint style="danger" %}
Beachten Sie, dass Sie eine Bestellung, die als 'Versendet' markiert wurde, nicht stornieren können.
{% endhint %}

### Teilweise Erstattung

Um eine Teilerstattung auszustellen, müssen Sie zunächst die Bestellung bearbeiten, um den geschuldeten Betrag zu ändern. Es gibt zwei Möglichkeiten, [eine Bestellung zu bearbeiten](view-orders.md#einen-auftrag-bearbeiten), wenn Sie eine Teilerstattung vornehmen möchten. Sie können die Artikelmengen anpassen oder eine Anpassung vornehmen:

**1.Bearbeiten, indem Sie einen Artikel**, der nicht vorrätig ist, entfernen oder die Menge eines Artikels ändern, indem Sie zu [Bestellungen -> Bestellung bearbeiten](view-orders.md#hinzufuegen-und-entfernen-von-produkten-aus-einer-bestellung) gehen und auf das Symbol "Bearbeiten" rechts neben dem betreffenden Artikel klicken, wie unten dargestellt:

Wählen Sie unten auf der Seite "Gebühren aktualisieren und neu berechnen".

{% hint style="danger" %}
Wenn das [Produkt](../products-1/) vom Lieferanten aus seiner Hauptproduktliste gelöscht wurde, ist es nicht möglich, diese Seite zu bearbeiten. Verwenden Sie in diesem Fall die unten stehende Methode "Anpassungen".
{% endhint %}

**2. Ändern Sie die Gebühren** in der [Bestellung](view-orders.md#einen-auftrag-bearbeiten), indem Sie im Menü auf der rechten Seite Bestellungen -> Bearbeiten -> Anpassungen aufrufen.

![](https://lh3.googleusercontent.com/qu1o7\_GwVwvozkH-aSaxH7Pg9ZJ9mcd-jXM0VrNmUTGyMeOfKmdhf8WPa66FjVayQEryr1Bkv4Q\_2UfVSlhSCDvvQcSaZ-ARj-gJG01cWPTRh4ktAMy1ofk4gyUiWQ4ZoK2OfkjB)

Daraufhin wird eine Liste der Unternehmensgebühren für jeden Artikel in der Bestellung sowie der Gebühren für Versand und Zahlungsmethode angezeigt. Sie können eine dieser Gebühren anpassen, indem Sie auf das Symbol "Bearbeiten" rechts neben dem betreffenden Artikel klicken.\


**3. Bearbeiten Sie den Auftrag**, indem Sie eine neue Anpassung hinzufügen, indem Sie im rechten Menü **Aufträge -> Bearbeiten -> Anpassungen** aufrufen und **+Neue Anpassung** (die Schaltfläche oben rechts) wählen, um eine separate Anpassung vorzunehmen, die nichts mit den Gebühren zu tun hat.

Fügen Sie die relevanten Details hinzu und denken Sie daran, dass der Wert für **eine Erstattung** eine **negative Zahl** sein muss. Wenn Sie fertig sind, klicken Sie auf "Weiter".

![](https://lh3.googleusercontent.com/RfvWyS1G6v7NVNIDGWTlpfK9hfZj7Vy5\_Q6NxlEEyWYtAnebNEphT8XTCSPGvC2EaIGrxioqhcGfaBOIpgqjhjqtSiCwCMKcd4BLFV9M2YIWQ32XkpkAqz\_fV-8GWI7CpkLteRpl)

{% hint style="success" %}
Sie können "Anpassungen" verwenden, um einem Kunden einen Teil der Kosten für ein minderwertiges Produkt zu erstatten.
{% endhint %}

Sobald die Bestellung geändert wurde, um entweder die fehlenden/angepassten Produkte oder die neue Anpassung zu berücksichtigen, erscheint die Bestellung mit dem Zahlungsstatus "Guthaben" für den Betrag, den der Kunde nicht mehr zahlen muss.

**Bearbeiten Sie die Teilerstattung**\
Wenn Sie eine Teilerstattung des geschuldeten Betrags vornehmen möchten, lesen Sie die Anweisungen, indem Sie die Zahlungsmethode auf den folgenden Registerkarten auswählen:

{% tabs %}
{% tab title="Bargeld/BACS" %}
1. Veranlassen Sie, dass die Erstattung an den Kunden unabhängig von der Plattform erfolgt.&#x20;
2. Erfassen Sie diese Aktion, indem Sie zu **Aufträge -> Bearbeiten** gehen und im rechten Menü "Zahlungen" und dann "**+ Neue Zahlung**" auswählen:

![](https://lh5.googleusercontent.com/Zt7ppdgUXqxp178D72tj9A5asLzqKoaI8YrniuLDokcraOvNRBT6Hn2oEGxOtM8n7fLb54VrXRYDzyLj4rmki6rr6NC\_8lRzME6B9VGjJ2dB78rpPMeoIT\_KBKpzA9GMncfpCXPc)



![](https://lh3.googleusercontent.com/l7lOK1yuMFNLur3XJhDEWTmaKQcfXhmziy26qbxXgUF7vs8BkvTTj7NPivA1wqgkckp5\_PNb3VtsNpOngDw7s9bszPMDMPvy5T7Ulu0c\_F2AhbHNJY0BsABUPMm6603\_ut7gqIpg)

Geben Sie in das Feld "Betrag" einen **negativen Wert** ein, um die Erstattung als erfolgt zu verbuchen.
{% endtab %}

{% tab title="Stripe" %}
Mit der OFN-Plattform können Sie einem Kunden, der mit Stripe bezahlt hat, automatisch Geld zurückerstatten. Die Erstattung wird direkt auf die Kredit- oder Debitkarte des Kunden überwiesen.

1.Gehen Sie zu **Aufträge -> Auftrag bearbeiten** und wählen Sie dann "Zahlungen" aus dem rechten Menü.

![](https://lh6.googleusercontent.com/DEfR7g7tS3wpeX3d3425q0i5yMImnTnwtJEqP2GfHEB\_nLp1SnqopkJUx8VHZ7jdZQLpYQdBwAtudkKp091KbNBBzB0jbRnd2jy5NBZH6g3WNfA18y8jSCVOPLabPe2tU-WRmfjy)

2.Da Sie die Anpassung im vorherigen Schritt vorgenommen haben, wird auf dem Zahlungsbildschirm nun "**Guthaben**" mit dem von Ihnen angegebenen Betrag angezeigt. Wenn Sie auf das Häkchen neben der Zahlung klicken, wird das dem Kunden geschuldete Guthaben automatisch zurückerstattet.

![](../../.gitbook/assets/refundfeast2.jpg)

{% hint style="warning" %}
Beachten Sie, dass es 3 bis 5 Arbeitstage dauern kann, bis Stripe-Zahlungen auf dem Kontoauszug eines Kunden erscheinen.
{% endhint %}
{% endtab %}

{% tab title="PayPal" %}
**Sie können einem Kunden, der mit PayPal automatisch über die OFN-Plattform bezahlt hat, derzeit keine Teilerstattung gewähren.**

1. Sie müssen sich in Ihr geschäftliches [PayPal-Konto](https://www.paypal.com/) einloggen und dem Kunden den korrekten Betrag über die Schnittstelle erstatten.
2. Um diese Aktion zu erfassen, müssen Sie wie folgt eine neue [Zahlungsmethode](../shopfront/payment-methods.md) einrichten:\
   Name= 'Paypal-Erstattungen'\
   Anzeige = 'Nur Back Office'\
   Zahlungsanbieter = "bar/EFT/etc".
3. Besuchen Sie **Aufträge - > Auftrag bearbeiten-> Zahlungen** (im rechten Menü).
4. Wählen Sie **+Neue Zahlung** und wählen Sie 'Paypal-Erstattungen':

![](https://lh4.googleusercontent.com/OxsAJGhZBmz7fZiuWo1Fp5l-hdfGvnFm2vIZRRAxYf5yc2z1q7pCz4-ef6wWb-T6QaKh5uxCFFAX-MG3PaXe\_N3ry4fpZ8XEp59NpmGididpdfvzf4gXvGBhQyRbmYfqhtFWrg1s)

Ein negativer Wert im Feld "Betrag" bedeutet, dass eine Erstattung erfasst wird.

{% hint style="danger" %}
Wenn Sie sich dafür entscheiden, eine neue Zahlung mit dem Zahlungsmittelanbieter "Paypal" hinzuzufügen, ist dies nicht möglich:
{% endhint %}

![](<../../.gitbook/assets/paypalnewpayment (1) (1).jpg>)
{% endtab %}
{% endtabs %}

## Einziehung zusätzlicher Zahlungen

Führen Sie die oben beschriebenen Schritte für [Teilerstattungen aus](refunds-and-adjusting-payments.md#teilweise-erstattung), um der Bestellung eines Kunden weitere Artikel hinzuzufügen oder Anpassungen über die Seite [Verwaltung von Großaufträgen](../products-1/group-buy-for-bulk-ordering.md#anpassung-von-auftraegen-zur-erstellung-vollstaendiger-chargen) vorzunehmen.

Bestellungen werden jetzt mit dem Zahlungsstatus = "Restbetrag fällig" angezeigt:

![](https://lh3.googleusercontent.com/0SIla3VUQfK-MqNQ0RTuLwndE2\_EFmBmZhafSRbb3v0QkDFwXCfPNXyKupa3cwBjXAAoiH6cc-5fMru2xP7SvfraYDnwFrH5jucOVcVUSo1SMv5hiGWn3wgNr15Jz670O80pSZ39)

Um die Zahlung der zusätzlich fälligen Beträge zu erfassen, besuchen Sie [Aufträge -> Auftrag bearbeiten](view-orders.md#einen-auftrag-bearbeiten) und dann "Zahlungen". Wählen Sie + Neue Zahlung (blaue Schaltfläche oben rechts)

1. Wenn der Kunde Ihrem Unternehmen das geschuldete Geld in **bar oder als** BACS-Zahlung gegeben hat, erfassen Sie dies auf die gleiche Weise wie bei einer Rückerstattung, verwenden aber einen positiven Wert im Feld "Betrag".
2. Wenn der Kunde anwesend ist oder am Telefon ist, können Sie die zusätzliche Zahlung über Stripe abwickeln. Hierfür benötigen Sie die Daten der Kredit-/Debitkarte des Kunden:

![](https://lh3.googleusercontent.com/xou54OA2WQDBKXWmRqHkT6em-7qkd8F6CNJ\_hvGWRCvzYbEh2JRtrI54C1ywHeL0X6VR8cFRnV3FELd\_pO-kufo2nPszNDq6d2VdO-PPHgnpw3TcgY6n8ysSq8AhaGim-alJYZNX)

{% hint style="danger" %}
Beachten Sie, dass der Einzug der zusätzlichen Gelder durch PayPal über die Plattform derzeit nicht möglich ist.
{% endhint %}

{% hint style="warning" %}
Wenn eine Zahlungsmethode mit einer Gebühr verbunden ist, wird diese Gebühr vom System jedes Mal aufgezeichnet, wenn Sie zusätzliches Geld vom Kunden einziehen oder ihm eine Erstattung ausstellen.
{% endhint %}

## Behalten Sie den Überblick über die Zahlungssalden Ihrer Kunden

Die fälligen Beträge (Guthaben) oder die fälligen Beträge (Lastschrift) für die einzelnen Aufträge können Sie auf der Verwaltungsseite Ihrer [Listingaufträge](view-orders.md) einsehen.

{% hint style="warning" %}
Remember that only payments for integrated payment methods (PayPal and Stripe) are automatically captured by the platform. If a customer pays your business by cash or BACS (or similar) you will need to [capture this payment](view-orders.md#capturing-a-payment) manually to keep your records up to date.

Denken Sie daran, dass nur Zahlungen für integrierte Zahlungsmethoden (PayPal und Stripe) automatisch von der Plattform erfasst werden. Wenn ein Kunde Ihr Unternehmen mit Bargeld oder BACS (oder ähnlichem) bezahlt, müssen Sie [diese Zahlung manuell erfassen](view-orders.md#payment-and-shipment-state), um Ihre Unterlagen auf dem neuesten Stand zu halten.
{% endhint %}

Vielleicht möchten Sie Ihren vertrauenswürdigen Kunden erlauben, einmal im Monat (per BACS) für alle ihre Bestellungen in diesem Zeitraum zu zahlen, oder denjenigen, die eine Woche Cashflow haben, etwas Spielraum bei ihren Zahlungen geben. Um die Salden der einzelnen Kunden Ihres Unternehmens zu verfolgen, besuchen Sie Ihre Kundenliste. Der fällige Kredit-/Lastschriftbetrag wird rechts neben dem Eintrag des jeweiligen Kunden angezeigt.

![](../../.gitbook/assets/customerbalance.jpg)
