# Werkzeug zur Bestandsaufnahme

## Einführung

Das "Inventar" gibt Unternehmen mehr Kontrolle und Flexibilität bei der Produktverwaltung, wenn sie dies wünschen. Die Funktion wird vor allem für Hubs und Hub-Manager von Interesse sein.

Mit Hilfe der Funktion "Inventar" kann Hub A die Preise und Lagerbestände der Artikel ändern, für die es eine Verkaufsgenehmigung besitzt. Mit dieser Funktion kann Hub A auch nur eine Teilauswahl von Waren seiner Zulieferer für den Verkauf in seinem Laden zur Verfügung stellen, wenn er nicht die gesamte Produktpalette vertreiben möchte. All dies ist möglich, ohne die Masterkopie der Produkte zu verändern. Wenn also sowohl Hub A als auch Hub B dieselben Produkte vorrätig haben, kann Hub A mit Hilfe des Inventarisierungstools den Preis und andere grundlegende Informationen über die von ihm verkauften Artikel ändern, ohne dass dies Auswirkungen auf Hub B hat.

## Profileinstellungen für die Bestandsaufnahme

Um auf das Inventar zuzugreifen, gehen Sie auf "Unternehmen" (im blauen horizontalen Menü) und dann auf "Einstellungen". Wählen Sie in der Menüleiste auf der linken Seite "Inventareinstellungen".

![](../../.gitbook/assets/inventory-settings.png)

Sie haben zwei Möglichkeiten:

* **Neue Produkte können in mein Schaufenster gestellt werden (empfohlen):** Die Produkte Ihres Lieferanten können in Ihr Online-Schaufenster aufgenommen werden, _ohne dass Sie sie vorher in Ihrem Shop/Hub-Inventar hinzufügen müssen_. Wenn Sie einen Bestellzyklus erstellen, stehen Ihnen alle Produkte der ausgewählten Hersteller zur Verfügung, die Sie dem "eingehenden" Teil des Zyklus (dem Bestellzyklus) hinzufügen können. \
  Dies ist die Standardoption und wird für Hubs empfohlen, die die Preise oder Lagerbestände der von ihnen verkauften Artikel nicht ändern möchten.

{% hint style="warning" %}
VORSICHT - wenn Sie Ihre Inventareinstellungen in diesem Standardmodus belassen, aber gleichzeitig Produkte in Ihr Hub-Inventar hochladen und deren Preise oder Lagerbestände ändern, werden die geänderten Informationen auf Ihrer Shopfront angezeigt, nicht diejenigen der Masterkopie.
{% endhint %}

* **Neue Produkte müssen zu meinem Inventar hinzugefügt werden, bevor sie zu meinem Schaufenster hinzugefügt werden können:** Wenn Sie einen Bestellzyklus erstellen, werden nur die Produkte, die Sie zuvor dem Hub-Inventar hinzugefügt haben, zur Auswahl im "eingehenden" Teil des Bestellzyklus angezeigt.

## Besuchen Sie Ihren Shop/Hub-Bestand

Klicken Sie oben im Admin-Dashboard auf das Menü Produkte und dann im grünen Untermenü auf Inventar. Wenn Sie mehrere Unternehmen verwalten, werden Sie aufgefordert, eines auszuwählen, da jedes Inventar unabhängig verwaltet wird.

![](../../.gitbook/assets/inventory1.jpg)

Wenn Ihre Lieferanten zwischen den einzelnen Besuchen Ihres Shops/Hub-Inventars neue Produkte hinzugefügt haben, wird die folgende Meldung angezeigt:

![](../../.gitbook/assets/new-products-alert.png)

Solange Sie diese Produkte nicht in den Bestand aufgenommen haben, verbleiben sie in der Kategorie "**Neue Produkte**" und sind für die Auswahl bei der Erstellung eines Bestellzyklus nicht sichtbar. Wenn Sie auf "**Jetzt prüfen**" klicken, werden Sie zur Liste der neuen Produkte weitergeleitet.

## Überprüfung neuer Produkte

Neue Produkte können entweder zu Ihrer Inventarliste **hinzugefügt** oder **ausgeblendet** werden. Wenn es ein Produkt in der Liste gibt, dessen Details Sie überschreiben oder für das Sie einen wiederkehrenden Lagerbestand festlegen möchten, müssen Sie es zu Ihrer Inventarliste **hinzufügen**. Wenn es ein Produkt gibt, das Sie nie in Ihrem Shop verkaufen oder zumindest in naher Zukunft nicht auf Lager haben möchten, können Sie es **ausblenden** (siehe Abschnitt **Ausgeblendete** **Produkte** unten).

![](../../.gitbook/assets/new-products.png)

{% hint style="info" %}
Denken Sie daran: Wenn Ihre **Bestandseinstellungen** so festgelegt sind, dass "neue Produkte erst in den Bestand aufgenommen werden müssen, bevor sie in mein Schaufenster gestellt werden können", werden alle Produkte, die Sie in der Liste "Neue Produkte" belassen, effektiv ausgeblendet. Wenn Ihre Bestandseinstellungen auf "Neue Produkte können in mein Schaufenster gestellt werden" eingestellt sind, werden die Produkte in Ihrer Liste "Neue Produkte" weiterhin in Ihrem Bestellzyklus angezeigt.
{% endhint %}

## Verwaltung Ihres Lagerbestands Produkte

In der Produktliste Ihres Inventars können Sie Produktdetails überschreiben, die Rücksetzung des Lagerbestands einrichten und Produkte ausblenden.

![](../../.gitbook/assets/viewing-inventory-settings.png)

Über die Schaltfläche "Spalten" auf der rechten Seite der Tabelle können Sie auswählen, welche Einstellungen Sie sehen und ändern möchten.

![](../../.gitbook/assets/columns-1.png)

### Ändern Sie SKU, Preise und Lagerbestände für Produkte in Ihrem Schaufenster

Alle Änderungen, die Sie hier vornehmen, werden in Ihrem Shop sichtbar und überschreiben somit die vom Lieferanten festgelegten Details. Sie können die folgenden Felder ändern:

* **SKU** - wenn Sie eine alternative SKU (Referenznummer) für ein Produkt verwenden möchten, können Sie hier die SKU des Herstellers außer Kraft setzen, indem Sie eine Alternative eingeben.
* **Preis** - Sie können einen anderen Preis festlegen, der in Ihrem Shop angezeigt wird. Beachten Sie, dass die Einheiten des Produkts gleich bleiben. Wenn das Produkt also einen Preis pro kg hat, können Sie nur die Kosten pro kg ändern, nicht aber die festen Kosten pro Artikel.
* **Auf Lager** - Wenn Ihr Bestand an diesem Produkt von dem von den Herstellern angebotenen Bestand abweicht, können Sie Ihren Bestand angeben. Ihre Produkte werden im Shop nicht mehr sichtbar sein, sobald der Lagerbestand Null erreicht.

{% hint style="info" %}
Das kann praktisch sein, wenn Sie einen Großeinkauf von z. B. 50 Artikeln pro Monat erhalten und die Verkäufe vor der nächsten Lieferung im Auge behalten müssen.
{% endhint %}

* **Unbegrenzt?** - Sie können wählen, ob Sie die Lagerbestände des Herstellers übernehmen möchten (in diesem Fall bleibt die Zahl in der Spalte "auf Lager" grau), ob Sie einen unbegrenzten Lagerbestand haben möchten (in diesem Fall geht der Artikel nie zur Neige und ist immer verfügbar, wenn er zu einem aktiven Auftragszyklus hinzugefügt wird) oder ob Sie Ihre eigenen Lagerbestände definieren möchten (in diesem Fall wird die Zahl in der Spalte "auf Lager" auf weißem Hintergrund angezeigt).

![](../../.gitbook/assets/inventorystock.jpg)

Informieren Sie sich [hier](products.md#hinzufuegen-von-produkten) über "auf Lager" und "unbegrenzt".

{% hint style="warning" %}
Es ist nicht möglich, den Produktnamen, die Eigenschaften, die Beschreibung oder das Bild zu ändern.
{% endhint %}

### "Lagerbestände auf Standardbestände zurücksetzen" aktivieren?

In der Spalte "Lagerbestände auf Standardbestände zurücksetzen" können Sie die Menge "Auf Lager" auf einen Standardwert zurücksetzen, z. B. zu Beginn jedes neuen Auftragszyklus. Der **Standardwert** ist die Zahl, die in dieser Spalte neben dem Kontrollkästchen eingegeben wird. Mit dem Kontrollkästchen können Sie nur die Artikel auswählen, die Sie zu einem bestimmten Zeitpunkt zurücksetzen möchten.

Um den Standardlagerbestand für diese Produkte zurückzusetzen, klicken Sie oben links in der Bestandstabelle auf "Aktionen" und dann auf "Lagerbestände auf Standardwerte zurücksetzen". Von dieser Aktion sind nur Produkte betroffen, für die das Kästchen "Lagerbestand zurücksetzbar?" markiert wurde.&#x20;

![](../../.gitbook/assets/inventorystockreset.jpg)

> In diesem Beispiel ist der Standardlagerbestand an gebackenen Bohnen 5. Derzeit sind noch 2 Stück auf Lager. Wenn der Benutzer zu Beginn eines Bestellzyklus auf 5 zurücksetzen möchte, muss er unter "Aktionen" auf "Lagerbestände auf Standardwerte zurücksetzen" klicken.

{% hint style="info" %}
Dies ist eine nützliche Funktion für Hubs, die einmal im Monat oder in regelmäßigen Abständen bestimmte Produkte geliefert bekommen.
{% endhint %}

### Eigenschaften übernehmen?

Wenn Sie keinen der Werte in der Inventartabelle für ein Produkt geändert haben, ist das Kontrollkästchen "Eigenschaften übernehmen?" standardmäßig aktiviert. Das bedeutet, dass die vom Hersteller eingegebenen und grau hinterlegten Informationen in Ihrem Schaufenster angezeigt werden.

![](../../.gitbook/assets/inventoryinherit.jpg)

Wenn Sie eines oder mehrere der Felder ändern, wird dieses Kontrollkästchen automatisch deaktiviert. Um Werte (Preis, Bestand, SKU usw.) auf die Werte der Herstellervorlage zurückzusetzen, können Sie dieses Kästchen jederzeit wieder aktivieren.

### Ausblenden

Wie in der Liste **Neue Produkte** können Sie auch Produkte aus Ihrer **Inventarliste ausblenden**. Wenn Sie auf die Schaltfläche "Ausblenden" klicken, wird das Produkt in Ihre Liste "**Ausgeblendete Produkte**" verschoben. Wenn Sie in Ihrem Inventarprofil die Einstellung "**Neue Produkte müssen meinem Inventar hinzugefügt werden, bevor sie meinem Schaufenster hinzugefügt werden können**" gewählt haben (siehe [hier](inventory-tool.md#profileinstellungen-fuer-die-bestandsaufnahme)), dann steht das Produkt, das Sie gerade ausgeblendet haben, im Bestellzyklus Ihres Hubs nicht mehr zur Auswahl und ist somit auch nicht in Ihrem Schaufenster sichtbar.

## Versteckte Produkte

Dies ist eine Liste mit allen Produkten, die Sie ausblenden möchten:

![](../../.gitbook/assets/hidden-products.png)

Wenn Sie Ihre Liste der ausgeblendeten Produkte ansehen, können Sie diese wieder sichtbar machen, indem Sie auf die Schaltfläche "**Hinzufügen**" rechts neben dem Artikel klicken.

![](../../.gitbook/assets/inventoryhidden.jpg)

## Bestandsaufnahme und Auftragszyklen

Beim Einrichten von Bestellzyklen können Sie von Fall zu Fall wählen, ob Sie aus allen verfügbaren Produkten oder nur aus denen, die sich in Ihrem Shop/Hub-Bestand befinden, auswählen möchten.

Dies wird unter "Erweiterte Einstellungen" (oben rechts auf der Seite des Bestellzyklus) gesteuert:

![](../../.gitbook/assets/advanced-oc-settings.png)

Diese Option hat dieselbe Wirkung wie die Änderung unserer [Unternehmensprofileinstellungen für Ihr Inventar](inventory-tool.md#profileinstellungen-fuer-die-bestandsaufnahme), aber im Gegensatz zu letzterem gilt sie nur für den betreffenden Auftragszyklus.

{% hint style="danger" %}
Wenn Sie Änderungen vorgenommen haben, denken Sie daran, auf "Aktualisieren" oder "Speichern" zu klicken, bevor Sie weitermachen!
{% endhint %}
