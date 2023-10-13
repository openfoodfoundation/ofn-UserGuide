# Ermäßigte/freie Lieferung für schutzbedürftige Kunden

## Einführung

Für ältere oder schwache Kunden kann es schwieriger sein, Ihr Zentrum oder die Abholstelle in Ihrem Geschäft zu erreichen. Auch wenn es Ihnen nicht unbedingt möglich ist, jedem Kunden die Waren an die Haustür zu liefern (aus Kosten-, Zeit- und Entfernungsgründen), haben Sie vielleicht die Möglichkeit, einer kleinen Anzahl von "vorrangigen" Kunden vor Ort zu helfen.

Im Folgenden finden Sie eine Schritt-für-Schritt-Anleitung, um ausgewählten Kunden eine kostenlose (oder ermäßigte) Lieferung zu ermöglichen.

Das Verfahren verwendet die Funktion Kundenmanagement, die [hier](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md#show-hide-shipping-methods) ausführlich beschrieben wird.

## Was ist vor dem Start zu beachten?

* Wie viele Zustellungen können Sie maximal zum kostenlosen/ermäßigten Tarif anbieten?
* Welche Gebiete würden Sie kostenlos oder zu einem ermäßigten Tarif beliefern? Beschränken Sie das Gebiet beispielsweise auf eine bestimmte Postleitzahl/Straße/Bezirk oder vielleicht auf Straßen auf Ihrem Heimweg.
* Seien Sie realistisch in Bezug auf die Anzahl der Lieferungen, die Sie durchführen können, und die Kosten für Benzin/Zeit, um sie durchzuführen.

## Prozess

* Notieren Sie sich den Namen des Kunden und die mit seinem OFN-Konto verknüpfte E-Mail-Adresse.
* Melden Sie sich bei Ihrem OFN-Geschäftskonto an und besuchen Sie die [Seite Kunden](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/customers.md).
* Verwenden Sie das Feld "Schnellsuche", um festzustellen, ob die Person bereits bei Ihnen eingekauft hat.&#x20;

![](https://lh6.googleusercontent.com/DcRo1W18G7l7JKxuhHybJB4gIEzZWQIX-3kynCMX79RwtrKFpMR8b6SYI4uyoQjGOOlmrV1rv7oIbsYS55UkfeH1yfu4SJntTnO1vMPmwuTMljBhkX\_kRhYLiI5fKzKjxYBR\_uCO)

* Wenn die E-Mail-Adresse nicht angezeigt wird, klicken Sie auf **+ Neuer Kunde** und fügen Sie die Adresse hinzu.
* Fügen Sie dem Kundeneintrag das Tag "free\_delivery" hinzu.

![](../../.gitbook/assets/freedelivtagcust.jpg)

* Besuchen Sie Unternehmen -> Einstellungen -> [Versandmethoden](../../basic-features/shopfront/shipping-methods.md) und klicken Sie auf +Neue Versandmethode.

![](../../.gitbook/assets/freedeliv.jpg)

Name: Kostenlose lokale Hauszustellung für ältere und schutzbedürftige Kunden.\
Beschreibung: Kostenlose Lieferung an Ihre Privatadresse.\
Anzeige: Sowohl Kasse als auch Back Office\
Kategorie: Lieferung\
**Tags: Fügen Sie an dieser Stelle den Tag "free\_delivery" ein.**\
Honorar-Rechner: Pauschalbetrag = 0,00\
Kategorien: Standard\
Zonen: UK\_VAT

* Rufen Sie die Seite Unternehmen -> Einstellungen auf und wählen Sie im linken Menü die Option "[Tag-Regeln](../../basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules.md)" aus. Richten Sie die folgenden Tag-Regeln ein:

Standard: Versandmethoden mit der Kennzeichnung 'free\_delivery' sind nicht sichtbar.\
Für Kunden, die mit "free\_delivery" gekennzeichnet sind, sind die mit "free\_delivery" gekennzeichneten Versandmethoden sichtbar.

![](../../.gitbook/assets/freedelivtags.jpg)

**Bingo! Ein Kunde, der sich bei Ihnen als älterer Mensch registriert hat und in der Nähe wohnt, hat diese Möglichkeiten an der Kasse:**

![Tagged customer view at checkout](https://lh3.googleusercontent.com/eq2nJ6QucE4SZCtLsrat2veXR2k8uxxdm5BPd7oyWc8EhT7wo8gMBEzKVGt07JqenrR8OOt5VmNbBotrnXEx8\_a9B8Ok3sdgOAlLWhutrgkMG42npDpiSnJl9G8xiBOIfT-MIs6d)

Alle anderen können nur Ihre Standardversandmethoden sehen:

![View of non-tagged customer's Shipping Options at checkout](https://lh4.googleusercontent.com/MHj98plQ6gLA6GCdl5g3p9S5wZccyaLwDb2PaHo1PVUE5iDXfcUTGlVZJrhL2TXKELmFkwdVt2iAMA2RxIFzsfv33Y60nh1OmQ4QunNfhPEYSCtvsYhkKCa511tvJrsr-UBdmww5)

{% hint style="success" %}
Fügen Sie einen Kommentar zu Ihren Standardversandmethoden hinzu (im Feld "Beschreibung"), um ältere und schutzbedürftige Kunden darüber zu informieren, wie sie mit Ihnen in Kontakt treten können, um in Zukunft für eine kostenlose Lieferung in Frage zu kommen.
{% endhint %}

## Das könnte Sie auch interessieren: Fügen Sie eine Nachricht an Ihre Kunden auf Ihrer Shop-Benachrichtigungsseite hinzu.

Vergessen Sie nicht, Ihre "Schaufenster-Nachricht" zu bearbeiten (zu finden unter Unternehmen -> Einstellungen -> Shop-Einstellungen), um neue ältere/gefährdete Kunden einzuladen, sich mit Ihnen in Verbindung zu setzen, damit sie vorrangig behandelt werden können.

![Admin view](https://lh5.googleusercontent.com/Wg3e\_guD-P5zbZE1oa6OFb36YU-csR35WpZD9Hxn0cT3O05jXDDihtHH2EL9CIP7atYsXXK3va9gUSvyfNka\_ovDGDtSG2uRqreA2nW4cp8IjCnL3eodEv12iZ5QkA2eRIGaCkzD)

![](../../.gitbook/assets/notices2.jpg)
