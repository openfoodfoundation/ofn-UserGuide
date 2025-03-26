# Abonnements - die Perspektive des Kunden

Auf dieser Seite erfahren Sie, was ein Kunde mit einem Abonnement erwarten kann. Sie hebt auch einige Dinge hervor, die Geschäfte, die Abonnements anbieten, beachten sollten.

## Anmeldung bei OFN

Kunden müssen ein Konto bei OFN haben, bevor Sie Abonnementbestellungen für sie bearbeiten können.Um ein Konto zu erstellen, leiten Sie den Kunden auf die lokale Open Food Network-Homepage und wählen Sie "Login" in der oberen rechten Ecke. Sie werden dann durch die Registrierung bei OFN geführt. **Kunden müssen eine aktive E-Mail-Adresse haben, um sich zu registrieren.**

Nach der Anmeldung erhalten sie eine Bestätigungs-E-Mail. Sobald sie auf den Link in dieser E-Mail klicken, wird ihr Konto bestätigt und sie können sich anmelden.

{% hint style="info" %}
Aufgrund übereifriger E-Mail-Filter (die Spam abwehren sollen) erhalten Kunden manchmal ihre Bestätigungs-E-Mail nicht von uns (oder sie wird in ihren Junk-Ordner geleitet). Bitten Sie sie in diesem Fall, open food network in den Einstellungen ihres E-Mail-Kontos zu ihrer "sicheren" Liste hinzuzufügen.
{% endhint %}

## Speichern von Kreditkarten und Autorisierung von Gebühren

Kunden, die ihre Abonnementbestellungen über automatische Abbuchungen von ihrer Kredit-/Debitkarte (Stripe) bezahlen möchten, müssen a) ihre bevorzugte Karte in ihrem OFN-Konto speichern und b) dem Shop die Erlaubnis erteilen, diese Karte zu belasten.

### Speichern der Kreditkartendaten im Kundenkonto

Die Seite Kundenkonto kann nach der Anmeldung bei OFN über die Schaltfläche "Profil" oben rechts aufgerufen werden:

![](../../.gitbook/assets/subcard1.jpg)

Ihr Kunde kann eine oder mehrere Karten in seinem Konto auf der Registerkarte "**Kreditkarten**" speichern.

![](../../.gitbook/assets/subcard2.jpg)

Wenn ein Kunde mehr als eine Debit-/Kreditkarte registriert, wird die als "Standard" bezeichnete Karte automatisch von Stripe belastet (wenn er ein Abonnement mit Stripe als gewählter Zahlungsmethode hat).

{% hint style="danger" %}
Wenn keine ihrer Karten als "Standard" ausgewählt ist, werden ihre Kreditkartenzahlungen nicht bearbeitet.
{% endhint %}

![](<../../.gitbook/assets/image (26) (1).png>)

Wenn Ihr Kunde Kreditkarten in seinem Konto speichert, kann er diese auch beim Einkauf in Ihrem Shop an der Kasse schnell auswählen.

![](<../../.gitbook/assets/image (4) (1).png>)

### Einem Geschäft die Genehmigung erteilen, seine Standardkarte zu belasten

**Sie sollten Ihre Kunden zu Ihrer** [**Kundenliste**](../shopfront/customer-management-and-conditional-displays-prices/customers.md) **hinzufügen, bevor Sie sie bitten, ihre Kreditkartendaten zu speichern und Ihren Shop zu ermächtigen, ihre Karte abzurechnen. Der Kunde wird Ihr Unternehmen nicht in der Liste "Autorisierte Geschäfte" auf der rechten Seite sehen, wenn Sie dies nicht getan haben.**

Damit die Stripe-Zahlungsmethode für ein Abonnement funktioniert, das der Kunde bei Ihrem Unternehmen abgeschlossen hat, muss er das Kontrollkästchen "Gebühren zulassen" aktivieren:

![](../../.gitbook/assets/subcard2.jpg)
