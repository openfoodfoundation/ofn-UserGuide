# Einbetten einer Gruppenseite in eine Website

Es ist jetzt möglich, eine Gruppenseite in eine Website außerhalb von OFN einzubinden. Hier finden Sie eine Schritt-für-Schritt-Anleitung, wie Sie dies einrichten können. Diese Funktion ist relativ neu und wurde noch nicht umfassend auf allen Plattformen getestet. Bitte kontaktieren Sie[ Ihr lokales OFN](https://openfoodnetwork.org/find-your-local-open-food-network/), wenn Sie Probleme mit der Einbindung einer Gruppenseite in Ihre Website haben.

## Voraussetzungen für das Einbetten einer Gruppenseite&#x20;

### Plattform

Es ist möglich, eine Gruppenseite auf jeder Website einzubetten, auf der Sie der Zielseite benutzerdefiniertes HTML hinzufügen können, einschließlich Plattformen wie WordPress, Squarespace oder Wix.

Im Folgenden finden Sie einige plattformspezifische Ressourcen:

* Weitere Informationen zum Hinzufügen von benutzerdefiniertem HTML mit "Codeblocks" finden Sie bei [Squarespace](https://support.squarespace.com/hc/en-us/articles/206543167).

### Sicherheit

Da OFN eine eCommerce-Plattform ist und Geldtransaktionen abwickelt, hat es höhere Sicherheitsanforderungen als andere Websites. Daher müssen Sie auf der Website, in die Sie Ihre Gruppenseite einbetten möchten, SSL/TLS einrichten lassen. Sie können ein kostenloses Sicherheitszertifikat von [Let's Encrypt](https://letsencrypt.org/) oder für etwa $10-$30 einen anderen kostenpflichtigen Dienst erhalten.

### Seite der OFN-Fraktion

Bevor Sie fortfahren, sollten Sie Ihre [Gruppenseite im Open Food Network einrichten](group-page.md). Sie müssen die URL Ihrer OFN-Gruppenseite kennen, um die folgenden Einrichtungsschritte durchführen zu können.

## Wie man eine Gruppenseite einbettet

**1) Kontaktieren Sie Ihr lokales OFN-Team**

Zunächst müssen Sie Ihr [lokales OFN-Team ](https://openfoodnetwork.org/find-your-local-open-food-network/)kontaktieren und ihm mitteilen, dass Sie Ihre OFN-Gruppenseite in Ihre Website einbinden möchten. Sie müssen ihnen Ihre externe Domain mitteilen, z. B. regionalgroup.com.au, damit sie die Erlaubnis erteilen können, dass Ihre Website mit OFN kommunizieren kann.

**2) Hinzufügen von benutzerdefiniertem HTML zu Ihrer Website**

Das Einbinden Ihrer Gruppenseite ist so einfach wie das Einfügen einer Codezeile in Ihre Website. Nachstehend finden Sie ein Beispiel für den HTML-Code, den Sie in die Seite einfügen müssen, in die Sie Ihre OFN-Gruppenseite einbetten möchten. Sie müssen "flavour-crusader" durch den eindeutigen OFN-Permalink Ihres Shops ersetzen.

```
<iframe src="https://openfoodnetwork.org.au/groups/flavour-crusader?embedded_shopfront=true" style="width:100%;min-height:35em"></iframe>
```

Sobald Sie dies getan haben, sollte Ihre OFN-Gruppenseite auf Ihrer Website an der Stelle erscheinen, an der Sie den HTML-Code eingefügt haben.

HINWEIS: Lesen Sie die Anweisungen zum [Erstellen und Verwalten einer Gruppenseite](group-page.md), um herauszufinden, wie Sie Ihren einzigartigen OFN-Permalink bearbeiten können.

**3) Styling**

Je nach der Gestaltung Ihrer Website müssen Sie möglicherweise das CSS bearbeiten. Wenn Sie mit CSS nicht vertraut sind, müssen Sie möglicherweise die Dienste Ihres Website-Administrators in Anspruch nehmen. CSS kann erforderlich sein, um zwei Bildlaufleisten zu vermeiden und um sicherzustellen, dass die Länge und Breite der eingebetteten Gruppenseite optisch ansprechend ist. Stellen Sie sicher, dass Sie die Anzeige Ihrer Gruppenseite auch auf einem mobilen Gerät testen, da dies möglicherweise weitere Änderungen erfordert.

## Anweisungen für Besucher

### Cookies

Die meisten Menschen haben Cookies in ihren Webbrowsern aktiviert. Wenn ein Besucher jedoch keine Cookies aktiviert hat, kann es sein, dass er eine ähnliche Fehlermeldung wie die unten stehende erhält und die eingebettete Gruppe nicht anzeigen kann.

![](../../.gitbook/assets/cookies.png)
