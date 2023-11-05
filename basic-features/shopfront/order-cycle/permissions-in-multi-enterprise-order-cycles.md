# Berechtigungen in unternehmensübergreifenden Auftragszyk

Diese Seite erläutert die unterschiedlichen Rechte, die jedes Unternehmen im Rahmen komplexer, unternehmensübergreifender Auftragszyklen hat. Sei es:

* der Hersteller ([Profil](../../../your-quick-start-on-ofn-given-who-you-are.md#profil) oder [Shop](../../../your-quick-start-on-ofn-given-who-you-are.md#laden)), der nur den Auftragszyklus liefert,
* eine [Drehscheibe](../../../your-quick-start-on-ofn-given-who-you-are.md#produzentenladen), die nur Waren vertreibt,
* oder eine Drehscheibe, die den Auftragszyklus [koordiniert](permissions-in-multi-enterprise-order-cycles.md#der-koordinator) (und gegebenenfalls auch Waren liefert oder vertreibt).

Weitere Einzelheiten zu einfachen Bestellzyklen, bei denen ein einzelner Hersteller nur seine eigenen Bestände verkauft ([Herstellershop](../../../your-quick-start-on-ofn-given-who-you-are.md#produzentenladen)), finden Sie [hier](order-cycles-for-producers.md).

_**Der Koordinator hat den höchsten Grad an Kontrolle über einen Auftragszyklus. Andere Unternehmen können die Auftragszyklen, an denen sie beteiligt sind, einsehen, aber nur die Einstellungen bearbeiten, die sie betreffen.**_

## Der Koordinator

{% hint style="info" %}
Die volle Funktionalität des Auftragszyklus kann nur genutzt werden, wenn ein Unternehmen als [Hub](../../../your-quick-start-on-ofn-given-who-you-are.md#produzentenladen) registriert ist. Um Ihren Unternehmenstyp zu ändern, siehe [hier](../../enterprise-profile/package-types.md#aendern-sie-ihren-profiltyp).
{% endhint %}

{% hint style="warning" %}
Sobald ein Auftragszyklus erstellt wurde, ist es nicht mehr möglich, den Koordinator zu ändern.
{% endhint %}

Der Koordinator eines [Auftragszyklus](order-cycles-for-hubs.md) kann:

* Erstellen Sie die Auftragszyklen
* Legen Sie den Namen des Auftragszyklus sowie das Eröffnungs- und Abschlussdatum fest und bearbeiten Sie ihn.
* Anwendung von Unternehmensgebühren auf alle Produkte (Koordinatorgebühr), auf Produkte, die von Produzenten geliefert werden (im [Eingangsbereich](permissions-in-multi-enterprise-order-cycles.md#incoming)), und/oder auf Produkte, die von Hubs verteilt werden (im [Ausgangsbereich](permissions-in-multi-enterprise-order-cycles.md#ausgehend-von)).

### **Incoming**

* Der Koordinator kann Unternehmen als Lieferanten hinzufügen. Dazu muss das liefernde Unternehmen (das bei OFN als [Produzent](../../enterprise-profile/package-types.md#fuer-erzeuger) registriert ist) dem koordinierenden Hub jedoch die Erlaubnis erteilt haben, seine[ Produkte einem Auftragszyklus hinzuzufügen](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md#erteilen-und-verwalten-von-berechtigungen).
* Der Koordinator kann alle oder eine Teilmenge der Produkte seiner Lieferanten auswählen, die er in den Bestellzyklus aufnehmen möchte.
*   Der Koordinator kann den einzelnen Lieferanten unterschiedliche [Unternehmensgebühren](../enterprise-fees.md) in Rechnung stellen. So kann er z. B. einem Metzger, der die Ware liefert, einen höheren Satz berechnen (um die zusätzlichen Kosten für den Kühltransport zu decken) als einem Bäcker.



### Ausgehend von

Der Koordinator kann wählen, über welche Unternehmen die in einem Auftragszyklus aufgeführten Produkte vertrieben werden (einschließlich seiner selbst).

Dazu muss jeder potenzielle Händler in der Lage sein:

1. Registriert als [Hub](../../../your-quick-start-on-ofn-given-who-you-are.md#produzentenladen).
2. Sie haben dem Koordinierungszentrum die Erlaubnis erteilt, Produkte zu einem [Auftragszyklus hinzuzufügen](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md#erteilen-und-verwalten-von-berechtigungen).
3. Sie müssen mindestens eine aktive [Versand](../shipping-methods.md)- und [Zahlungsmethode](../payment-methods.md) haben.

{% hint style="info" %}
Wenn ein potenzielles Vertriebsunternehmen in der Liste der möglichen Optionen im Abschnitt "Ausgang" des Auftragszyklus erscheint, aber nicht ausgewählt werden kann, hat es wahrscheinlich noch keine Versand- und/oder Zahlungsmethoden eingerichtet.
{% endhint %}

Der Koordinator kann aus der vollständigen Liste der eingehenden Produkte wählen, die im Schaufenster des jeweiligen Verteilernetzes angezeigt wird. **Der Lieferant (Herstellerprofil oder Shop) muss zwischen sich und dem jeweiligen Distributions-Hub (sowie dem Koordinator) eine** [**Unternehmensgenehmigung**](../../enterprise-profile/enterprise-to-enterprise-permissions-e2es.md) **für das "Hinzufügen zum Bestellzyklus" eingerichtet haben.**

Der Koordinator kann, falls gewünscht, jedem Verteilerknoten unterschiedliche [Unternehmensgebühren](../enterprise-fees.md) auferlegen. Dies kann von Vorteil sein, wenn ein Knotenpunkt weiter vom Koordinator entfernt ist als ein anderer und daher einen höheren Transportaufwand hat.

## Versorgung von (eingehenden) Unternehmen

Der Lieferant ([Produzent](../../enterprise-profile/package-types.md#fuer-erzeuger)) kann alle Auftragszyklen einsehen, an denen er beteiligt ist, indem er die Seite mit der Zusammenfassung der Auftragszyklen aufruft (im oberen horizontalen blauen Menü), auch wenn er die Auftragszyklen nicht selbst erstellt hat.\
Durch Anklicken des Auftragszyklus kann ein eingehender Produzent nur seine eigenen Angaben sehen, nicht aber die Produkte oder Angaben der anderen am Auftragszyklus Beteiligten. Er kann seine eigenen Daten bearbeiten: Er kann zum Beispiel ein Produkt, das nicht mehr vorrätig ist, aus einem Auftragszyklus entfernen. Ein lieferndes Unternehmen kann weder den Namen noch die Daten eines Auftragszyklus ändern.

Im Bereich Berichte (oberes horizontales blaues Menü) kann ein liefernder Produzent die für den Auftragszyklus eingegangenen Aufträge einsehen

{% hint style="warning" %}
Ein lieferndes Unternehmen sieht nicht automatisch die Namen der Kunden, die seine Produkte gekauft haben, wenn es nicht gleichzeitig der Koordinator des Auftragszyklus ist. Diese Einstellung kann vom Auftragszykluskoordinator (Unternehmen, das den Auftragszyklus verwaltet) geändert werden. Wenn Sie die Kundennamen sehen müssen, um das Verpacken und Ausführen von Bestellungen zu erleichtern, können Sie sich an Ihren Bestellzyklus-Koordinator wenden und ihn bitten, das Kontrollkästchen Kundennamen in Berichten in den [Unternehmenseinstellungen](../../enterprise-profile/enterprise-settings.md) unter Shop-Einstellungen zu aktivieren.
{% endhint %}

### Eingehend

* Ein Lieferant kann **seine** Produkte im Abschnitt "Eingehende Produkte" eines Auftragszyklus anzeigen, hinzufügen und entfernen.
* Ein Lieferant kann Unternehmensgebühren hinzufügen/entfernen, die auf **seine** Produkte im Abschnitt "Eingehende Produkte" des Auftragszyklus angewendet werden. Dies könnte für Produzenten nützlich sein, die mehrere Hubs beliefern, von denen einige viel weiter entfernt sind als andere. Sie möchten vielleicht eine zusätzliche Abgabe für weiter entfernte Hubs erheben, um die Transportkosten zu decken.

### Ausgehend von

Der Grad des Einflusses, den ein Lieferant auf seine Produkte im Abschnitt "Ausgehende Produkte" eines Auftragszyklus hat, hängt von den spezifischen Unternehmensberechtigungen ab, die er dem Distributionszentrum erteilt hat, und vice versa.

* Wenn der vertreibende Hub dem liefernden Produzenten (Profil, Shop oder Hub) das Recht eingeräumt hat, "zum Bestellzyklus \[des Hubs] hinzuzufügen", dann kann der Lieferant Produkte in der Liste im Abschnitt "Ausgehende Produkte" des Bestellzyklus sehen, hinzufügen und entfernen.
* Wenn der vertreibende Hub dem liefernden Produzenten (Profil, Shop oder Hub) nicht das Recht eingeräumt hat, "zum Bestellzyklus \[des Hubs] hinzuzufügen", dann kann der Lieferant die Liste im Abschnitt "Ausgehende Produkte" des Bestellzyklus einsehen, aber NICHT Produkte hinzufügen oder entfernen.
* Ein Lieferant kann weder die Abhol- und Lieferbedingungen noch die für den Händler geltenden Unternehmensgebühren ändern.

## Verteilendes (ausgehendes) Unternehmen

Ein Verteilerunternehmen kann die Auftragszyklen, an denen es beteiligt ist, auf seiner Übersichtsseite für Auftragszyklen anzeigen, auch wenn es diese nicht selbst erstellt hat (d.h. nicht der Koordinator des Auftragszyklus ist). Durch Anklicken eines Auftragszyklus kann das abgebende Vertriebsunternehmen die Details eines Auftragszyklus sehen, die sich nur auf ihn beziehen. (Wenn sie z.B. nicht der einzige Verteiler des Auftragszyklus sind, können sie weder sehen, wer die anderen Verteilerunternehmen sind, noch die Produkte, die sie in ihrem Shop anbieten). Das ausgehende Vertriebszentrum kann die Details seines Vertriebs - Liefertermine und -methoden sowie Unternehmensgebühren für den Vertrieb - einsehen und bearbeiten, nicht aber den Namen oder den Zeitraum des Auftragszyklus selbst.

Im Menü "Berichte" kann ein Auftragszyklus-Händler die erteilten Aufträge (zusammen mit den Kundennamen) einsehen, um die Lieferung/Versendung von Waren zu unterstützen.

### Eingehend

Ein Händler kann die eingehenden Produkte von Lieferanten einsehen, die ihm die Unternehmensberechtigung "zum Bestellzyklus hinzufügen" erteilt haben, aber er kann weder Lagerbestände/Verfügbarkeit bearbeiten noch herstellerspezifische Unternehmensgebühren anwenden/entfernen.

{% hint style="warning" %}
Gegenwärtig kann nur der Koordinator eines Auftragszyklus zusätzliche Lieferanten (Produzenten) zu diesem hinzufügen.
{% endhint %}

### Ausgehend von

Der Grad des Einflusses, den das Vertriebszentrum auf die Produkte im Abschnitt "ausgehende Produkte" eines Auftragszyklus hat, hängt von den Unternehmensrechten zwischen ihm und dem liefernden Hersteller ab.

* Der verteilende Hub kann Produkte zu seinem ausgehenden Austausch hinzufügen/entfernen. Dies gilt nur für Produkte von Produzenten, die vom Koordinator in den Auftragszyklus aufgenommen wurden und die dem Verteiler die Unternehmensberechtigung "zum Auftragszyklus hinzufügen" erteilt haben.
* Sie können die Abhol-/Lieferdaten ändern
* Können ihre Unternehmensgebühr hinzufügen/entfernen
