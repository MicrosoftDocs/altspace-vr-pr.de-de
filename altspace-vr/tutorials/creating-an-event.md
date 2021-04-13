---
title: Erstellen eines Ereignisses
description: Erfahren Sie mehr über altspacevr-Ereignisse, wie Sie Sie erstellen und mit dem Welt-Editor Branding-und 3D-Objekte hinzufügen.
ms.date: 03/11/2021
ms.topic: article
keywords: Veranstaltungen, Terminologie, Konsole, Multimedia, World Editor, Livestream
ms.openlocfilehash: 9b9f7ac8ef5d036b739873fc19c879250a1e264e
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212290"
---
# <a name="creating-an-event"></a>Erstellen eines Ereignisses

Dies ist eine Schritt-für-Schritt-Anleitung zum Erstellen von Ereignissen in altspacevr. Es wird dringend empfohlen, dass Sie mehrere Ereignisse in altspacevr besuchen, um sich mit der Funktionsweise vertraut zu machen. Überprüfen Sie den [altspacevr-Ereignis Kalender](https://account.altvr.com/events) auf eine Liste aller Ereignisse.

In diesem Artikel lernen Sie Folgendes:

* Altspacevr-Ereignis Terminologie
* Erstellen von Ereignis-und Ereignis Raum oder Welt
* Verwenden der Multimedia-Konsole für eine Folien Präsentation
* Branding Ihres Ereignisses mit Bildern
* Hinzufügen von 3D-Objekten mithilfe von World Editor/Kits
* Vorgehensweise beim Aufzeichnen oder Live Stream meines Ereignisses

## <a name="altspacevr-event-terminology"></a>Altspacevr-Ereignis Terminologie

Im folgenden sind die Begriffe aufgeführt, mit denen Sie sich vertraut machen müssen, um das Ereignis und den Ereignis Bereich zu erstellen:

</br>

| Begriff | Definition |
|---|---|
| Welt aufbauen | Altspacevr bietet die Möglichkeit, virtuelle Umgebungen zu erstellen und anzupassen. Altspacevr-Hosts unterstützen Dokumentation, Zwietracht-Kanäle und in-World-Veranstaltungen, [damit Sie mehr darüber erfahren, wie Sie Hilfe erhalten und mit der Gebäude Bildung beginnen](../world-building/world-building-faq.md). |
| World | Eine Welt ist ein virtueller Bereich in altspacevr. Möglicherweise handelt es sich um einen Büro-oder einen großen Berg Bereich. Es handelt sich um eine hochgradig anpassbare Umgebung. Sie befindet sich in einem Universum, und es können mehrere Welten innerhalb dieses Universums vorhanden sein. Wenn Sie über mehrere Ereignis Bereiche für spezielle Ereignisse, Schulungszentren und verschiedene Besprechungsräume verfügen möchten, um die Dinge zu untersuchen, fügen Sie die Welten unter demselben Universum hinzu, um Sie als Gruppe zusammenzuhalten. |
| Universe | Ein Universum in altspacevr World, das die Aufteilung der Welt repräsentiert. Jedes Universum kann mehrere Welten enthalten. Die Welt erbt die Einstellungen des Universums und vereinfacht so das Hinzufügen von Personen zu "Allow-List" für mehrere Welten und andere Steuerungsfunktionen. Weitere Informationen finden [Sie unter Verwalten](../world-building/managing-worlds.md) von Umgebungen. |
| Vorlage | Eine Vorlage (oder eine Speicherplatz Vorlage) ist eine vorgefertigte Welt oder Umgebung, die verwendet werden kann, anstatt Sie mithilfe der Welt erstellerfunktionen zu erstellen. Altspacevr bietet eine Vielzahl von Vorlagen für verschiedene Erfahrungen und Ereignisse. |
| Ereignis Bereich | Ein Ereignis Bereich ist ein Synonym für Welt in altspacevr. Im Allgemeinen bezieht es sich auf eine Welt, die zum Hosten von Ereignissen verwendet wird. |
| Website | Verweise auf die "Website" sind auf der [Website von altspacevr](https://altvr.com/)enthalten. Häufig ist es einfacher, Ereignisse über die [Ereignis Webseite](https://account.altvr.com/events/my) auf einem Computer oder Tablet und nicht über Ihr VR-Gerät zu erstellen und zu bearbeiten. Sie müssen auch auf die Website für das [weltweite Gebäude](../world-building/managing-worlds.md) zugreifen. |
| Kontextabhängige Rollen | [Kontext Rollen](../getting-started/roles.md) werden vom Ereignis Ersteller oder World Builder zugewiesen. Diese Rollen enthalten Benutzern in einer Welt oder einem Ereignis Bereich zusätzliche Features und Funktionen. Zurzeit bestehen diese aus "Host", "Presenter", "Moderator", "Pilot (Flight)", "Terraformer" (Welt Gebäude) und "megaphone". Diese können einzeln oder Global zugewiesen werden, sodass alle die gleichen Rollen im Ereignis Bereich oder in der Welt haben können. |
| Benutzeroberfläche (UI)/Menu | Wenn Sie in altspacevr in der Umgebung sind, gibt es in der immersiven Umgebung Menüs auf der linken und rechten Seite des Bildschirms. Das Kreis-oder Hauptmenü mit dem altspacevr-Logo öffnet die Hauptbenutzer Oberfläche (UI) oder das Menü, um auf verschiedene Bildschirme zum Kennenlernen von altspacevr und zum Anpassen Ihrer Benutzeroberfläche zuzugreifen. Optionale Benutzeroberflächen Elemente werden auf der rechten Bildschirmgröße gefunden und enthalten in der Regel den World Editor und die Host Tools. Diese werden geöffnet und interagiert, indem Sie mit dem Cursor darauf klicken. |
| SDK/MRE | Dabei handelt es sich um Länder Bausteine, die mit dem Software Development Kit und den [Mixed Reality-Erweiterungen](../world-building/using-mixed-reality-extensions.md) verknüpft sind, mit denen Features und Funktionen zur weltweiten Entwicklung hinzugefügt werden. Diese sind in der Regel für fortgeschrittene Benutzer. |

## <a name="understanding-events"></a>Grundlegendes zu Ereignissen

Mit altspacevr können Sie ganz einfach eine Welt erstellen, in der Sie einen vorgefertigten Vorlagen Bereich verwenden können, um Ihre speziellen Anforderungen zu verwenden oder anzupassen, oder eine Welt von Grund auf neu erstellen. In diesem Artikel wird die Verwendung einer vorgefertigten Vorlage zum Erstellen Ihres Ereignisses behandelt. Die folgenden Abschnitte zum [Branding Ihres Ereignisses mit Bildern](#branding-your-event-with-images) und zum [Hinzufügen von 3D-Objekten mithilfe von World Editor und Kits](#adding-3d-objects-using-world-editor-and-kits) enthalten Tipps zur weiteren Anpassung. Weitere Informationen zum Erstellen einer benutzerdefinierten Welt von Grund auf finden Sie in der Welt Building Tour Meetups in altspacevr. [sehen Sie sich die Dokumentation zur Welt Erstellungs Unterstützung](../world-building/world-editor-getting-started.md)an.

Altspacevr bietet zwei Möglichkeiten zum Erstellen eines Speicherplatzes für das Ereignis.

* **Einmalige Verwendung:** Erstellen Sie ein Ereignis, und wählen Sie eine Vorlagen Welt aus.
* **Wiederholte Verwendung:** Erstellen Sie einen Welt Raum, und importieren Sie ihn in das-Ereignis.

Der Prozess des Erstellens eines Ereignisses ist für beide identisch, mit einer Ausnahme: der [Erstellung einer Welt und dem Import](../world-building/managing-worlds.md) als Wiederholungs verwendende Ereignis Bereich. Außerdem müssen Sie Folgendes wissen:

</br>

| Begriff | Definition |
|---|---|
| Welt kopiert | Die Verwendung eines weltweiten Raums für ein wiederholtes Ereignis ermöglicht eine permanente Anpassung. Zeichen, Bilder, erstellungspunkte und andere Anpassungen werden von Ereignis zu Ereignis verwaltet, anstatt den Ereignis Bereich jedes Mal anzupassen. |
| Anpassen von Event World | Wenn ein Ereignis erstellt wird, wird die Vorlage oder die importierte Welt kopiert und in dieses Ereignis gesperrt. Möglicherweise nehmen Sie Änderungen an der Welt des Ereignisses vor und wirken sich nicht auf die ursprüngliche Welt aus, und umgekehrt. Es empfiehlt sich, Ferien Dekorationen, Bilder oder andere dekorative Elemente der einmaligen Verwendung des World Editors hinzuzufügen, um den Ereignis Bereich zu optimieren und für das Ereignis geeignet zu machen. |

Änderungen, die an der ursprünglichen Welt vorgenommen werden, sind nicht in der Ereignis Welt, es sei denn, der Ereignis Bereich wird aktualisiert:
1. Verwenden Sie die Schaltfläche " **Welt neu importieren** " auf der Ereignis Webseite.
2. Hiermit wird die Synchronisierung von 2-3 Minuten zugelassen. 
3. Wenn sich der Ereignis Bereich nicht geändert hat, wechseln Sie zu **Einstellungen > moderieren > den Speicherplatz zurücksetzen** , um den Ereignis Bereich zurückzusetzen. Sie werden viel Platz als Welt Generator zurücksetzen!

Wenn Sie technische Probleme haben, z. b. Elemente, die nicht ordnungsgemäß geladen werden, wechseln Sie zum Menü "altspacevr", und wählen Sie " **Einstellungen" > >** "Mittel", um den Ereignis Bereich zurückzusetzen und die neuen Änderungen Windows-PC-Benutzer in 2D können die Tastenkombination " **STRG + ALT + R** " in "altspacevr" verwenden, um den Bereich schnell zurückzusetzen.

## <a name="creating-your-event-and-event-space-or-world"></a>Erstellen von Ereignis-und Ereignis Raum oder Welt

Im folgenden finden Sie Schritt-für-Schritt-Anleitungen zum Erstellen eines Ereignisses für ein einmalige oder wiederholtes Ereignis. Durch Auswählen der Vorlage oder Importieren einer Welt für das Ereignis. 

> [!NOTE]
> Die Webseite für altspacevr-Ereignisse bietet Anweisungen zu jedem Aspekt des Formulars durch die Verwendung von grünen Fragezeichen-Schaltflächen. Führen Sie für bestimmte Anweisungen einen Rollover für den Cursor durch.

Wählen Sie auf der Webseite [Ereignisse > meine Ereignisse](https://account.altvr.com/events/my) auf der Website von altspacevr die **Option Ereignis planen** aus, oder wechseln Sie direkt zum Ereignis erstellen auf der Webseite [altspacevr](https://account.altvr.com/events/new).

1. **Ereignis Titel:** Geben Sie den Namen des Ereignisses ein. Sorgen Sie für eine genaue und präzise Anzeige der verschiedenen Kalender Ansichten in der Website von altspacevr und in der Welt. Versuchen Sie, ihren Titel unter 23 Zeichen, einschließlich Leerzeichen zwischen Wörtern, beizubehalten.
2. **Beschreibung:** Geben Sie die Beschreibung des Ereignisses ein.
    * In der Beschreibung müssen mindestens 10 Zeichen enthalten sein, oder das Ereignis wird nicht erstellt.
    * Fügen Sie einen leeren Leerraum zwischen Absätzen hinzu.
    * Um einen Link zu Facebook, Zwietracht, Website oder anderen Ressourcen Ihres Ereignisses hinzuzufügen, verwenden Sie das folgende Format (dieses markdown funktioniert nur auf der Promotionseite Ihres Ereignisses auf der Website, dies wird nicht ordnungsgemäß in den Menüs "altspacevr" angezeigt): `[Event Name](http://example.com/)`

3. **Start Datum/Enddatum:** Legen Sie die Startzeit fest, und stellen Sie sicher, dass die Endzeit nach der Startzeit liegt.
4. **Kategorie:** Wählen Sie die Kategorie aus, die den Ereignistyp am besten beschreibt. 
5. Legen Sie das Ereignis auf **Privat** oder **öffentlich** fest.
    * Sichtbarkeit: öffentliche Ereignisse werden auf der [Registerkarte alle](https://account.altvr.com/events/all) auf dem Ereignis Kalender des altspacevr-Website angezeigt und sind öffentlich zugänglich.
    * Private Ereignisse sind in den Ereignis Kalendern von altspacevr nicht sichtbar und erfordern die Ereignis-URL, um den Ereignis Bereich einzugeben.
    * Wenn Sie "als Hauptereignis hinzufügen" möchten, muss das Ereignis auf "Public" festgelegt werden.
6. **Vorlage auswählen:** Auf der rechten Seite der Webseite befindet sich eine Liste mit Miniaturbildern der verfügbaren Vorlagen in altspacevr. Es gibt Spielräume, Niederlassungen, Besprechungsräume, Präsentationsräume und spaßbereiche. Wählen Sie einen Wert aus, der interessant aussieht. Wenn Sie dies nicht möchten, erstellen Sie einfach ein neues Ereignis mit einer neuen Vorlage. Wenn Sie Ihre eigene benutzerdefinierte Ereignis Welt erstellen möchten, wählen Sie den **coolsky** als Standardvorlage aus, und befolgen Sie die Anweisungen unten, um Ihre Welt zu importieren.
7. **Erweiterte Optionen** auswählen

### <a name="advanced-options"></a>Erweiterte Optionen

1. Herauf Stufen **:** Jedes Ereignis erfordert zwei brandingimages (diese Images werden auf der altspacevr-Website angezeigt und werden nicht in Ihrem Ereignis innerhalb von altspacevr angezeigt):
    * **Kachel:** Das Kachel Bild muss 1920 x 1080 Pixel betragen. Dieses Bild wird auf verschiedene Miniatur Ansichts Größen skaliert und im Kalender für altspacevr-Ereignisse mit anderen Ereignissen angezeigt. Stellen Sie sicher, dass das Bild eindeutig ist und keinen großen Text enthält. Verwenden Sie keine urheberrechtlich geschützten Images/Logos, die Sie nicht besitzen.
    * **Banner:** Die Banner Bilder müssen 1920 x 576 sein. Diese Größe wird nach Bedarf automatisch angepasst und auf der Ereignis Information oder Webseite angezeigt. Eine halbtransparente Überlagerung deckt die unteren 25% des Bilds ab. Vermeiden Sie das Platzieren von Text in diesem Bereich.
    * Eine weitere (schnellere) Option ist das **Kopieren eines Kachel Bilds in das Hintergrund Banner Bild**. dabei wird auch das Kachel Bild als Banner Bild verwendet. Probieren Sie es aus,:). Wenn es nicht gut aussieht, können Sie ein neues Banner Bild erstellen.
2. **In VR:** Dieser Abschnitt enthält Funktionen, die für die virtuelle Darstellung während des Ereignisses innerhalb der altspacevr-App gelten:
    * **Standardmäßige Kontext Rollen:** Das grüne Fragezeichen listet die einzelnen Rollen auf, die für *alle Audience-Mitglieder im Ereignis* verfügbar sind. Am häufigsten wird *megaphone_only*. Fügen Sie diese hinzu, um die Option "meine Stimme verstärken" unter der Schaltfläche "Host Tools" allen Audience-Membern zuzuweisen, damit Sie in Ihrem gesamten Ereignis, wenn es sich um einen großen Bereich handelt, angezeigt werden. Wenn für Ihr Ereignis ein Flug erforderlich ist, fügen Sie *Pilot* hinzu. Um beides hinzuzufügen, ist das Format: *megaphone_only, Pilotprojekt*. Jeder Benutzer muss den Modus "fliegen" in der altspacevr-App aktivieren, indem er zu "Einstellungen/Eingabe/fortfahren" wechselt.
    * **Anweisungen:** Die [Anweisungen](../world-building/adding-welcome-messages.md) sind für Text, der bei Eingang im Raum ein Willkommens Bild generiert. Benutzer müssen "OK" auswählen, um Sie aus der Ansicht zu entfernen. Dies wird häufig zum Bereitstellen von Zielgruppen Anweisungen verwendet, wie z. b. "Sie bleiben stumm gehalten, um zu sprechen" oder "Willkommen bei XYZ-Ereignis, bei dem wir ABC behandeln." Dies ist nicht erforderlich. verwenden Sie daher die Verwendung von bedacht. Sie können markdown auch zum Hinzufügen von Farbe und Schriftgröße hinzufügen, ausführlichere Informationen: [http://digitalnativestudios.com/textmeshpro/docs/rich-text](http://digitalnativestudios.com/textmeshpro/docs/rich-text)
3. **Erweitert:** Im folgenden finden Sie eine kurze Erläuterung der erweiterten Features für Ereignisse (einige dieser Features werden erst angezeigt, wenn das Ereignis erstellt wurde und Sie das Ereignis bearbeiten):
    * **Administratoren:** Administratoren sind altspacevr-Benutzer, denen Sie Vertrauen, um Sie bei der Verwaltung Ihres Ereignisses zu unterstützen. Dabei kann es sich um Ihre Co-Hosts oder Sicherungs Hosts handeln. Wenn Sie Ihren Benutzernamen zur Liste der Administratoren hinzufügen, können Sie folgende Aktionen ausführen:
        * Ändern Sie den Ereignis Titel, die Beschreibung und andere Features.
        * Fügen Sie Kontext Rollen für Moderatoren, Referenten und andere Rollen hinzu, und entfernen Sie Sie.
        * Löschen Sie das-Ereignis.
    * **Gruppe:** Wählen Sie über das Dropdown Menü aus Ihren privaten [Gruppen](group-features.md) aus. Wird nur angezeigt, wenn Ihr Konto einer Gruppe erstellt bzw. hinzugefügt wurde.
    * **Tagline:** Dieser präzise Satz wird auf der Ereignis Webseite unter dem Titel angezeigt.
    * **Aus Welt importieren:** Um einen erstellten weltweiten Ereignis Bereich für die wiederholte Verwendung zu verwenden, ist dies der Abschnitt im Formular, mit dem das Layout und die Anpassung der Welt in Ihr Ereignis importiert werden. Beachten Sie die folgenden Aspekte:

    **Importieren Sie Ihre eigene Welt:** Zum Importieren einer Welt erstellen Sie Folgendes:
    * Wählen Sie den Dropdown Pfeil aus, um eine Liste der von Ihnen erstellten Umgebungen anzuzeigen.
    * Wählen Sie die Welt aus.
    * Nachdem Sie den Rest des Ereignis Formulars abgeschlossen haben, warten Sie mindestens zwei Minuten, bevor Sie den Ereignis Bereich in altspacevr aufrufen, um sicherzustellen, dass die Datenbankinformationen aktualisiert werden und die Welt generiert wird.
    
    **Verwenden Sie die Welt einer anderen Person:**
    * Wenden Sie sich an den Besitzer der Welt, um anzufordern, dass er die Funktion **Freigabe mit Freunden** in einer individuellen Welt verwendet, um Sie für Sie freizugeben.

3. **YouTube-Video-ID:** Auf der Webseite des Ereignisses werden auf der Seite des Ereignisses YouTube-ereignisnachspann oder-Videos zur Ereignis Webseite hinzugefügt, nicht in der Welt. Sie benötigen nur den Video-ID-Teil der URL: dQw4w9WgXcQ
4. **Twitter-handle:** Dadurch wird der Twitter-Stream der Webseite des Ereignisses hinzugefügt. Wenn das Twitter-Konto privat ist und nicht mit dem Ereignis oder der Zuordnung verknüpft ist, ist die Freigabe möglicherweise nicht möglich. Sie benötigen nur das Handle: @elonmusk
5. **Kontextabhängige Rollen:** An dieser Stelle steuern Sie die Superkräfte oder [kontextbezogenen Rollen](../world-building/granting-roles.md) ihrer Ereignis Hosts, Presenter, Moderatoren und anderen Rollen innerhalb des Ereignisses. Um Sie hinzuzufügen, geben Sie Ihren altspacevr-Benutzernamen ein, und weisen Sie Ihnen im Dropdown Menü eine Rolle zu. Um diese zu entfernen, aktivieren Sie das Kontrollkästchen, um die Ereignis Webseite zu entfernen und zu speichern. Hinweis: Wenn Sie eine Presenter-Moderations Funktion gewähren möchten, müssen Sie Sie als Presenter und Moderator hinzufügen. Die folgenden kontextbezogenen Rollen sind zurzeit verfügbar:
    * **Presenter:** Fügt der-Schnittstelle der Person in altspacevr die [Features der Vorder Zeile](../faqs/front-row-events.md) hinzu, um diese Features hinzuzufügen.
    * **Moderator:** Fügt der-Schnittstelle der Person Moderations Features hinzu, einschließlich der Möglichkeit, jeden Teilnehmer zu Texten, Sie Global für das Ereignis zu stumm schalten oder aus dem Ereignis zu entfernen. Fügen Sie den Presenter erneut hinzu, und geben Sie ihm Moderations Rollen, wenn Sie über Moderations Berechtigungen verfügen möchten.
    * **Nur megaphone:** Fügt die Schaltfläche meine Stimme verstärken über die Schaltfläche "Hosttools" zu Ihrer Schnittstelle hinzu.
    * **Terraformer:** Fügt die Schaltfläche "World Editor" zu Ihrer Schnittstelle hinzu.
    * **Pilot Projekt:** Fügt Flug Funktionen für diese Person hinzu. Hinweis: Sie müssen dies in "Einstellungen/Eingabe/Betrieb" aktivieren.
    * **Musikalischer Performer:** Fügt Funktionen und Features hinzu, die mit Konzert-und Musik Ereignissen verknüpft sind.
6. **Aufgeführte Benutzer blockieren:** Wenn Sie verhindern möchten, dass ein Benutzer den Zugriff sperrt, oder wenn ein Benutzer zuvor von einem Moderator oder Präsentator aus dem Ereignis entfernt wurde und das Ereignis dupliziert wurde, wird der Name des aufgelisteten Benutzers aufgeführt. Ereignis Hosts oder Administratoren können jederzeit einen von einem Benutzer aufgelisteten Benutzer hinzufügen oder entfernen.

Wenn das Formular fertig und dreifach aktiviert ist, wählen Sie **Ereignis erstellen** aus.

> [!IMPORTANT]
> Wenn Ihr Ereignis nicht ordnungsgemäß erstellt wird, stellen Sie sicher, dass in ihrer Beschreibung mindestens 10 Zeichen vorhanden sind und/oder Sie eine Vorlage ausgewählt haben, wird der Name der Vorlage bei Auswahl von weiß in blau angezeigt.

## <a name="event-page-actions"></a>Aktionen der Ereignis Seite

Auf der Ereignis Webseite stehen Ihnen die folgenden Aktionen und Optionen zur Seite:

1. Wählen Sie **Bearbeiten** aus, um die Ereignis Einstellungen zu ändern.
2. Wählen Sie **Ereignis beenden** aus, um das Ereignis zu beenden (wenn das Ereignis beispielsweise über einen frühen Zeitpunkt liegt).
3. Wählen Sie **auf Entwurf festlegen** , um das Ereignis auf Draft anstelle von aktiv festzulegen.
4. Wenn Sie ein Update Ihrer importierten Welt durchgeführt haben, müssen Sie die Option " **neu importieren** " auswählen, damit diese Änderungen in Ihrem Ereignis angezeigt werden. vergessen Sie nicht, den Speicherplatz im Ereignis zurückzusetzen:)
5. Wählen Sie **doppeltes Ereignis** aus, um das Ereignis für zukünftige Ereignisse zu duplizieren. Dieses Duplikat wird dann in "Ereignisse"/"Entwurf" angezeigt, Sie müssen den neuen Tag und die Uhrzeit aktualisieren und dort aktivieren.
6. Wählen Sie **als Hauptereignis hinzufügen** aus, um das Ereignis auf die Kalender Auflistung festzulegen.
7. Wählen Sie **Ereignis löschen** aus, wenn Sie das Ereignis vollständig löschen möchten (Sie können das Ereignis nicht wiederherstellen).

Wenn Sie fertig sind, wechseln Sie zum Menü **Ereignisse > Menü Meine Ereignisse** in der Oberfläche von altspacevr in der Welt, und geben Sie den Ereignis Bereich ein, um den Bereich zurückzusetzen, die Änderungen zu überprüfen oder die Anpassung fortzusetzen. 

> [!IMPORTANT]
> Dies ist eine Kopie, und Anpassungen an den Ereignis Bereich sind nur für dieses Ereignis vorgesehen. Wenn Sie viel Zeit damit verbringen, den Platz des Ereignisses anzupassen, ist es möglicherweise besser, eine Welt für das **wiederholte Verwendungs Ereignis** zu erstellen.

Weitere Informationen zum Anpassen des Ereignis Raums oder zum Erstellen einer ursprünglichen Ereignis Raumumgebung zum Importieren:

* [Gewusst wie anderen Personen in meiner Welt Rollen zu gewähren?](../world-building/granting-roles.md)
* [Gewusst wie können Menschen in meiner Welt fliegen (oder andere Möglichkeiten haben)?](../world-building/adding-user-abilities.md)
* [Wo erhalte ich Hilfe bei der Welt erbaustellung?](../world-building/getting-help.md)
* [Gewusst wie meine Welten verwalten?](../world-building/managing-worlds.md)
* [Häufig gestellte Fragen zur Welt](../world-building/world-building-faq.md)
* [Gewusst wie zu meinen Welten benutzerdefinierte erfügende Punkte hinzufügen?](../world-building/adding-custom-spawn-points.md)
* [Gewusst wie meine eigenen Kits hochladen?](../world-building/uploading-custom-kits.md)
* [Gewusst wie beginnen Sie mit dem World Building Toolkit (Unity Uploader)?](../world-building/world-building-toolkit-getting-started.md)

## <a name="using-the-multimedia-console-for-a-slide-presentation"></a>Verwenden der Multimedia-Konsole für eine Folien Präsentation

Die Multimedia-Konsole eignet sich hervorragend zum Organisieren Ihrer Inhalte für eine Präsentation, einschließlich Bildern, Audiodaten oder Videos. Befolgen Sie die Anweisungen in der [Multimedia-Konsole](multimedia-console.md) , um das Setup für Ihr Ereignis zu erhalten.

## <a name="branding-your-event-with-images"></a>Branding Ihres Ereignisses mit Bildern

In altspacevr ist das Hinzufügen von Bildern zu Ihrem Ereignis Bereich oder Firmenlogo und-Branding oder sogar Fotos von sich selbst, Ihrem Team oder anderen visuellen Inhalten ganz einfach.

Die Abbild Anforderungen lauten:
* JPG-oder PNG-Dateien werden akzeptiert.
* Maximale Bildgröße: 1920 × 1080
* Lösung: 72 dpi
* Dateigröße: weniger als 250 KB pro Datei

Der Prozess umfasst das Hochladen des Images auf Ihre [altspacevr-Fotos](https://account.altvr.com/photos)und die anschließende Verwendung der Fotos im Welt-Editor in der Welt, um Sie in den Veranstaltungsraum zu importieren und zu platzieren.

1. Wechseln Sie auf der altspacevr-Website zu [Fotos](https://account.altvr.com/photos) .
2. Klicken Sie auf **Hochladen**.
3. Wählen Sie **Durchsuchen** aus, um ein Dialogfeld auf Ihrem Computer zu öffnen und das optimierte Abbild zu suchen und auszuwählen.
4. Klicken Sie auf **Öffnen**.
5. Wählen Sie **Foto erstellen** aus.
6. Wiederholen Sie diesen Schritt für alle Ihre Images.

Positionieren Sie sich in altspacevr und in der Ereignis Welt an der Stelle, an der Sie das Bild platzieren möchten. (Wenn Sie dies für ein **wiederholtes Verwendungs Ereignis** erstellen, stellen Sie sicher, dass Sie sich in ihrer Welt befinden und sich nicht im Ereignis Bereich befinden!)

1. Wählen Sie auf der Benutzeroberfläche in der unteren rechten Ecke die Option " **World Editor/Editor Panel** " aus.
2. Klicken Sie unten auf die Registerkarte **meine** .
3. Wählen Sie **Fotos** aus.
4. Fotos werden in der chronologischen Reihenfolge des Uploads gespeichert, sodass das neueste hochgeladene Bild das erste Bild in der Liste sein sollte. Wählen Sie diese Option aus, um Sie der Welt hinzuzufügen.
5. Verwenden Sie den Cursor des Geräts, und platzieren Sie es an der Stelle, an der Sie es wünschen.
    * Sie können die Größe des Datenträgers mithilfe ihrer Controller ändern (in der Regel über den Touchpad in VR schieben oder mit der Maus im 2D-Modus).
    * Um die Position und Drehung des Bilds zu optimieren, wählen Sie das **Zahnrad** Symbol auf dem Bild im Editor aus, und legen Sie die Drehung und Position entsprechend fest.
    * Sie können auch die Größe des Abbilds mit dem Feature skalieren ändern.

> [!NOTE]
> Wenn der Bearbeitungsmodus on (orangefarbener Text) ist, können Sie automatisch einen Vorgang durchführen, um eine einfachere Bewegung zum Platzieren von Bildern in der Ereignis Welt zu ermöglichen.

6. Wiederholen Sie diesen Schritt für jede Bild Platzierung.
7. Wenn die Bilder direkt festgelegt sind, wählen Sie **alle Sperren** aus, wenn Sie Sie nicht einzeln gesperrt haben, und deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den Editor.
8. Pro Ereignis können maximal fünf Fotos verwendet werden.

## <a name="adding-3d-objects-using-world-editor-and-kits"></a>Hinzufügen von 3D-Objekten mithilfe des World Editors und Kits

Altspacevr ermöglicht das Importieren von 3D-Objekten in eine Welt mit dem Welt-Editor. Es gibt viele World Editoren-Kits, die derzeit zur Verwendung verfügbar sind, und vieles mehr. Es gibt zwischen Raum Hüften, Raketen, animierte Tiere, Skulpturen, Strukturen, Werke und viele verschiedene Objekte. Oder Sie können Ihre eigenen Kits der öffentlichen Sammlung oder ihrer eigenen persönlichen Verwendung hinzufügen, oder Sie können eine der [altspacevr-MRE-apps](../world-building/using-mixed-reality-extensions.md)verwenden, die Objekt übergreifende Objekte in Ihre Welt bringen, wie z. b. Helm, Schwerter, Wings, Bekleidung, Hüte oder andere Objekte, die sich in der Tabelle befinden. Erwarten Sie, dass die Liste der Objekte bald erweitert wird.

Die hier aufgeführten Anweisungen konzentrieren sich auf die Verwendung von bereits in den Kits verwendeten Elementen. Weitere Informationen zum Hinzufügen und Importieren von 3D-Objekten in altspacevr finden [Sie unter "Importieren von gltf-Modellen in meine Welt"](../world-building/importing-models.md) . und ["Gewusst wie meine eigenen Kits hochladen?"](../world-building/uploading-custom-kits.md).

Wenn Sie ein vorhandenes 3D-Objekt aus den World Building Kits in ihrer Ereignis Umgebung hinzufügen möchten, können Sie mit dem Bereich "World Editor/Editor" den offenen und den Bearbeitungsmodus aktivieren

1. Erkunden Sie die Kits für das Objekt, das Sie importieren möchten, und wählen Sie es aus.
2. Wählen Sie das Kit-Objekt mit dem Cursor aus, und positionieren Sie es. Verwenden Sie das Zahnrad Symbol für das Objekt im Welt-Editor, um die Optionen Position, Drehung und Skalierung für den manuellen Nummern Eintrag zu verwenden.
3. Wenn das Objekt an der rechten Position platziert wird, Sperren Sie es, indem Sie auf das Sperrsymbol klicken.
4. Fügen Sie ein weiteres Objekt hinzu, wenn Sie möchten. Wenn Sie 3D-Objekte hinzufügen möchten, halten Sie Ihre Auswahl nicht mehr als Elemente aus fünf verschiedenen Einzel Kits, um die Unterstützung von Oculus Quest-Benutzern zu verbessern. Verwenden Sie nicht mehr als 200 Objekte in einer Welt.
5. Wenn Sie diesen Vorgang abgeschlossen haben, Sperren Sie alle Elemente, deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den World Editor. Umherlaufen. Laden Sie einige Tester ein, um Sie zu besuchen und auszuprobieren, und bereiten Sie sich auf Ihr gutes Ereignis vor!

Weitere Informationen zu den World Editor Kits und zum Hinzufügen von 3D-Objekten zu altspacevr:

* [Was ist das frühe Zugriffs Programm?](../world-building/early-access.md)
* [Wie werden gltf-Modelle in meine Welten importiert?](../world-building/importing-models.md)
* [Gewusst wie eine MRE in meiner Welt verwenden?](../world-building/using-mixed-reality-extensions.md)

## <a name="how-to-record-or-live-stream-my-event"></a>Vorgehensweise beim Aufzeichnen oder Live Stream meines Ereignisses

Im folgenden Supportdokument finden Sie Anweisungen zum Aufzeichnen oder Live Streaming Ihres Ereignisses:

* [Vorgehensweise beim Aufzeichnen oder Live Stream meines Ereignisses](recording-and-live-streaming.md)