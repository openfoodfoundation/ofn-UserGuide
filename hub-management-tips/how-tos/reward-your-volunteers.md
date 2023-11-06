# Belohnen Sie Ihre Freiwilligen

{% hint style="danger" %}
<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-LpeYcYHvFT89zDzVlG4%2F-LpeZq2i0oaAbNYfYfu5%2FCapture%20du%202019-09-26%2000-38-19.png?alt=media&#x26;token=aef3eea2-4d60-4d24-99ec-6edbda36b45c" alt="" data-size="line">-->​<img src="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-L9rgk4wEweX_zxXIzmW%2F-MdHZQzZkj-9uNA4c3qD%2F-MdIF6yxdsNWC5BK3awW%2FFlagge%20Deutschland.jpg?alt=media&#x26;token=9bbe895b-2aa1-40da-8221-01fb74558b92" alt="" data-size="line"> Diese Seite ist noch nicht ins Deutsche übersetzt. Wenn du mithelfen möchtest, melde dich gerne bei uns [per E-Mail](mailto:konrad@openfoodnetwork.de) oder [im Slack](https://join.slack.com/t/openfoodnetwork/shared\_invite/zt-9sjkjdlu-r02kUMP1zbrTgUhZhYPF\~A)!
{% endhint %}

## Einführung

Möchten Sie sich bei den Menschen bedanken, die Ihr Lebensmittelunternehmen mitbetreuen? Eine Möglichkeit ist, Mitarbeitern und Freiwilligen einen kleinen Rabatt auf ihre Einkäufe zu gewähren. Im Folgenden finden Sie eine Schritt-für-Schritt-Anleitung, wie Sie dies umsetzen können. Der Prozess stützt sich auf die äußerst flexiblen Kundenmanagement-Tools, die mit [Tags und Tag-Regeln](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md) zur Verfügung stehen.

## Prozess

* Bitten Sie Ihre Freiwilligen, Ihnen die mit ihrem OFN-Konto verknüpfte E-Mail-Adresse mitzuteilen.
* Melden Sie sich bei Ihrem OFN-Geschäftskonto an und besuchen Sie die Seite [Kunden](https://app.openfoodswitzerland.ch/admin/customers).
* Verwenden Sie das Feld "Schnellsuche", um festzustellen, ob die Person bereits bei Ihnen eingekauft hat.

![](https://lh6.googleusercontent.com/DcRo1W18G7l7JKxuhHybJB4gIEzZWQIX-3kynCMX79RwtrKFpMR8b6SYI4uyoQjGOOlmrV1rv7oIbsYS55UkfeH1yfu4SJntTnO1vMPmwuTMljBhkX\_kRhYLiI5fKzKjxYBR\_uCO)

* Wenn die E-Mail-Adresse nicht angezeigt wird, klicken Sie auf **+ Neuer Kunde** und fügen Sie die Adresse hinzu.
* Fügen Sie dem Eintrag des Kunden die Markierung "Freiwilliger" hinzu.

![](https://lh6.googleusercontent.com/SQyjjQgyilzSxTiEtRooR\_ELTZdT\_v0JAId0xIT5YsSf7crTmCZFyIkLg6mhfFD3\_BA9BA43QFWtCqeciTOyim-diGYfcrQrDHCb8umBvxb3nQcNOdS58tC0qg2bOlFPSsMinFbC)

* Gehen Sie zu Unternehmen -> Einstellungen und wählen Sie dann "[Zahlungsmethoden](../../basic-features/shopfront/payment-methods.md)" aus dem Menü auf der linken Seite. &#x20;
* Klicken Sie auf **+ Neue Zahlungsmethode**.

![](../../.gitbook/assets/voldiscount.jpg)

\
Name: Volontär 5% Rabatt\
Beschreibung: Danke, dass Sie uns helfen, unser lokales Lebensmittelzentrum zu betreiben.\
Anzeige: Sowohl Kasse als auch Back Office\
Aktiv: ja\
**Stichworte:** Fügen Sie an dieser Stelle den Tag "Freiwilliger" ein.\
Anbieter: Wählen Sie die für Ihr Unternehmen am besten geeignete Methode.\
Honorar-Rechner: Pauschaler Prozentsatz

* Nachdem Sie "Erstellen" ausgewählt haben, fügen Sie in das Feld "Betrag" des Abschnitts "Gebührenrechner" ein "-5" \* ein. (Negatives Vorzeichen führt zu einem Rabatt)\
  \
  \*-5 führt zu einer Ermäßigung von 5 %, wenn Ihr Unternehmen die Unternehmensgebühren nicht in Anspruch nimmt.

![](../../.gitbook/assets/pmcalc.jpg)

{% hint style="danger" %}
Alle **prozentualen Gebühren** werden nur auf der Grundlage eines Prozentsatzes der **Produktkosten** berechnet.
{% endhint %}

{% hint style="warning" %}
Wenn Ihr Unternehmen eine pauschale prozentuale Unternehmensgebühr auf alle Produkte erhebt, dann ist der Betrag, den Sie in das Feld "Pauschaler Prozentsatz" für diese Rabatt-Zahlungsmethode eingeben müssen:

&#x20;$$= (100 + Unternehmensgebühr)* Gewünschter Rabatt/100$$&#x20;

z. B. für ein Unternehmen mit einer Unternehmensgebühr von 20 %, das Freiwilligen einen Rabatt von 5 % gewähren möchte, lautet der Betrag, der in den pauschalen Prozentsatz für diese Zahlungsmethode einzugeben ist:

$$= -(100 + 20) *5/100 = -6$$&#x20;
{% endhint %}

* Rufen Sie die Seite **Unternehmen -> Einstellungen** auf und wählen Sie im linken Menü die Option "[Tag-Regeln](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#zahlungsarten-anzeigen-ausblenden)" aus. Richten Sie die folgenden Tag-Regeln ein:

Standard: Zahlungsarten mit der Kennzeichnung "Freiwillig" sind nicht sichtbar.\
Für Kunden mit der Kennzeichnung "Freiwillige" sind Zahlungsmethoden mit der Kennzeichnung "Freiwillige" sichtbar.

![](https://lh5.googleusercontent.com/wSWqmOnwusb\_3gWx8J5MVBceTFYfq7AB1-uKMcFfD2neWmuiESg2rI896B4iugX767fDxljCVLe-vFIS5V7pQojimIl2e3iuBPlFzLtlPL1oqtMhYesm9CPX-JybyR3rHpKJ0HXS)

**Bingo! Nur Ihre Freiwilligen erhalten einen Rabatt von 5 %, wenn sie bei Ihnen einkaufen.**

![Checkout view for volunteer](https://lh4.googleusercontent.com/aniH6MTDqxKFnR\_7PRP4duUp33nNOd7XdQpa0RRFcEgcoyjsUHSwLXOSEO8lbXWtNTXYFGTrt6QAopPjuiu8zJGxwtcXYalNBw8Y3wi-alSuGLyyBXm4h\_AH5pSc11fmvhS\_IMuk)

![Checkout view for all other customers](../../.gitbook/assets/allcart.jpg)

