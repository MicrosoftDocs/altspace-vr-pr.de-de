---
title: Erstellen einer Veranstaltung
description: Erfahren Sie mehr über AltspaceVR-Ereignisse, deren Erstellung und das Hinzufügen von Branding- und 3D-Objekten mit dem World Editor.
ms.date: 03/11/2021
ms.topic: article
keywords: Ereignisse, Terminologie, Konsole, Multimedia, Welt-Editor, Livestream
ms.openlocfilehash: 0c6e59604339ad354dc0241ca81335f92d65b0845529f6d1fe5eb2eb0d18627f
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127452"
---
# <a name="creating-an-event"></a>Erstellen einer Veranstaltung

Dies ist eine Schritt-für-Schritt-Anleitung zum Erstellen von Ereignissen in AltspaceVR. Es wird dringend empfohlen, an mehreren Veranstaltungen in AltspaceVR teilzunehmen, um ein Gefühl für deren Funktionsweise zu erhalten. Überprüfen Sie den [AltspaceVR-Ereigniskalender](https://account.altvr.com/events) auf eine Liste aller unserer Ereignisse.

In diesem Artikel lernen Sie Folgendes:

* AltspaceVR-Ereignisterminologie
* Erstellen ihres Ereignis- und Ereignisraums oder Ihrer Welt
* Verwenden der Multimediakonsole für eine Präsentation
* Branding Ihres Ereignisses mit Bildern
* Hinzufügen von 3D-Objekten mithilfe von World Editor/Kits
* Aufzeichnen oder Live Stream My Event

## <a name="altspacevr-event-terminology"></a>AltspaceVR-Ereignisterminologie

Im Folgenden finden Sie Begriffe, mit denen Sie beim Erstellen Ihres Ereignis- und Ereignisbereichs vertraut sein müssen:

</br>

| Begriff | Definition |
|---|---|
| World Building | AltspaceVR bietet die Möglichkeit, virtuelle Welten zu erstellen und anzupassen. AltspaceVR-Hosts unterstützen Dokumentation, Discordkanäle und In-World-Ereignisse, damit Sie mehr darüber erfahren, wie Sie Hilfe erhalten und mit dem [Erstellen von Welten beginnen](../world-building/world-building-faq.md)können. |
| World | Eine Welt ist ein virtueller Raum in AltspaceVR. Es kann sich um ein Büro oder einen großen Höhenbereich handelt. Es ist eine hochgradig anpassbare Umgebung. Es befindet sich in einem Universe, und es gibt möglicherweise mehrere Welten in diesem Universe. Wenn Sie über mehrere Ereignisräume für besondere Ereignisse, Training centers und verschiedene Besprechungsräume verfügen möchten, um Dinge zusammenzubringen, fügen Sie die Welten unter demselben Universe hinzu, um sie als Gruppe zusammenzuhalten. |
| Universe | Ein Universe in altspaceVR world building vernaular stellt die Kategorisierung Ihrer Welten dar. Jedes Universe kann mehrere Welten enthalten. Die Welten erben die Einstellungen des Weltalls, sodass es einfach ist, Personen zur "Allow-List" für mehrere Welten und andere Steuerungsfunktionen hinzuzufügen. Weitere Informationen finden Sie unter [Verwalten Ihrer Welten.](../world-building/managing-worlds.md) |
| Vorlage | Eine Vorlage (oder Raumvorlage) ist eine vorgefertigte Welt oder Umgebung, die verwendet werden kann, anstatt eine mithilfe der World Building-Features zu erstellen. AltspaceVR bietet eine Vielzahl von Vorlagen für verschiedene Erfahrungen und Ereignisse. |
| Ereignisbereich | Ein Ereignisraum ist ein Synonym für die Welt in AltspaceVR. Im Allgemeinen bezieht sie sich auf eine Welt, die zum Hosten von Ereignissen verwendet wird. |
| Website | Verweise auf die "Website" beziehen sich auf die [AltspaceVR-Website](https://altvr.com/). Es ist häufig einfacher, Ereignisse über die [Webseite Ereignisse](https://account.altvr.com/events/my) auf einem Computer oder Tablet zu erstellen und zu bearbeiten, anstatt über Ihr VR-Gerät. Sie müssen auch auf die Website zugreifen, um weltweit [zu erstellen.](../world-building/managing-worlds.md) |
| Kontextbezogene Rollen | [Kontextbezogene Rollen](../getting-started/roles.md) werden vom Ereignisersteller oder World Builder zugewiesen. Diese Rollen bieten Benutzern in einer Welt oder einem Ereignisbereich zusätzliche Features und Funktionen. Derzeit bestehen diese aus Host, Moderator, Pilot (Flight), Terraformer (World Building) und Megaphone Only. Diese können einzeln oder global zugewiesen werden, sodass jeder die gleichen Rollen im Ereignisraum oder in der Welt haben kann. |
| Benutzeroberfläche (BENUTZEROBERFLÄCHE)/Menü | Wenn Sie sich in altspaceVR in der Welt befinden, befinden sich in der immersiven Umgebung Menüs auf der linken und rechten Seite des Bildschirms. Der Kreis oder das Hauptmenü mit dem AltspaceVR-Logo öffnet die Hauptbenutzeroberfläche (UI) oder das Menü, um auf verschiedene Bildschirme zuzugreifen, um AltspaceVR zu erkunden und Ihre Benutzeroberfläche anzupassen. Optionale Benutzeroberflächenelemente befinden sich auf der richtigen Bildschirmgröße und enthalten in der Regel World Editor und Host Tools. Diese werden geöffnet und interagieren mit , indem Sie mit dem Cursor darauf klicken. |
| SDK/MRE | Hierbei handelt es sich um World Building-Begriffe, die dem Software Development Kit zugeordnet sind, und [Mixed Reality Erweiterungen,](../world-building/using-mixed-reality-extensions.md) die zum Hinzufügen von Features und Funktionen zur Weltweiten Gebäudeerfahrung verwendet werden. Diese sind in der Regel für fortgeschrittene Benutzer vorgesehen. |

## <a name="understanding-events"></a>Grundlegendes zu Ereignissen

AltspaceVR vereinfacht das Erstellen einer Welt, in der Sie einen vorgefertigten Vorlagenbereich verwenden können, um sie für Ihre spezifischen Anforderungen zu verwenden oder anzupassen oder eine Welt von Grund auf neu zu erstellen. In diesem Artikel wird die Verwendung einer vorgefertigten Vorlage zum Erstellen Ihres Ereignisses behandelt. Die folgenden Abschnitte zu [Branding Your Event with Images](#branding-your-event-with-images) und Adding [3D Objects using World Editor and Kits](#adding-3d-objects-using-world-editor-and-kits) enthalten Tipps zur weiteren Anpassung. Informationen zum Erstellen einer benutzerdefinierten Welt von Grund auf finden Sie in den World Building Tour-Treffen in AltspaceVR und in der Dokumentation zur [World Building-Unterstützung.](../world-building/world-editor-getting-started.md)

AltspaceVR bietet zwei Möglichkeiten, einen Raum für Ihr Ereignis zu erstellen.

* **Einmalige Verwendung:** Erstellen Sie ein Ereignis, und wählen Sie eine Vorlagenwelt aus.
* **Wiederholte Verwendung:** Erstellen Sie einen Weltraum, und importieren Sie ihn in das Ereignis.

Der Prozess zum Erstellen eines Ereignisses ist für beide identisch, mit einer Ausnahme: der [Erstellung einer Welt und](../world-building/managing-worlds.md) dem Importieren als Wiederholungsereignisbereich. Außerdem müssen Sie Wissen:

</br>

| Begriff | Definition |
|---|---|
| Kopierte Welt | Die Verwendung eines Weltraums für ein wiederholtes Ereignis ermöglicht eine dauerhafte Anpassung. Zeichen, Bilder, Spawnpunkte und andere Anpassungen werden von Ereignis zu Ereignis beibehalten, anstatt den Ereignisraum jedes Mal anzupassen. |
| Anpassen der Ereigniswelt | Wenn ein Ereignis erstellt wird, wird die Vorlage oder die importierte Welt kopiert und in dieses Ereignis gesperrt. Sie können Änderungen an der Ereigniswelt vornehmen und sich nicht auf die ursprüngliche Welt auswirken, und umgekehrt. Erwägen Sie das Hinzufügen von Feiertagsdekorationen, Bildern oder anderen zierlichen Einmaligen Verwenden von Elementen des Welt-Editors, um den Ereignisraum für das Ereignis besser und geeigneter zu gestalten. |

Änderungen an der ursprünglichen Welt werden nur dann in der Ereigniswelt vorgenommen, wenn der Ereignisbereich aktualisiert wird:
1. Verwenden Sie die Schaltfläche **RE-IMPORT WORLD** auf der Ereigniswebseite.
2. Warten Sie 2 bis 3 Minuten, bis die Synchronisierung abgeschlossen ist. 
3. Wenn sich der Ereignisbereich nicht geändert hat, wechseln Sie zu **Einstellungen > Moderieren > Speicherplatz zurücksetzen,** um den Ereignisbereich zurückzusetzen. Als Ersteller der Welt werden Sie viel Speicherplatz zurücksetzen!

Wenn sie technische Probleme haben, z. B. elemente nicht ordnungsgemäß geladen werden, wechseln Sie zu Ihrem AltspaceVR-Menü, und wählen Sie **Einstellungen > Moderieren > Speicherplatz zurücksetzen** aus, um den Ereignisbereich zurückzusetzen und die neuen Änderungen anzuzeigen. Windows PC-Benutzer in 2D können die Tastenkombination verwenden: **STRG + ALT + R** in AltspaceVR, um Speicherplatz schnell zurückzusetzen.

## <a name="creating-your-event-and-event-space-or-world"></a>Erstellen ihres Ereignis- und Ereignisraums oder Ihrer Welt

Im Folgenden finden Sie schrittweise Anweisungen zum Erstellen eines Ereignisses für ein einmaliges oder wiederholtes Ereignis. Durch Auswählen der Vorlage oder Importieren einer Welt für das Ereignis. 

> [!NOTE]
> Die AltspaceVR-Ereigniswebseite bietet Anweisungen zu jedem Aspekt des Formulars mithilfe von grünen Fragezeichenschaltflächen. Setzen Sie den Cursor auf diese, um bestimmte Anweisungen zu erhalten.

Wählen Sie auf der Website von AltspaceVR auf der Webseite Events > My Events (Ereignisse [> Meine Ereignisse)](https://account.altvr.com/events/my) die Option **Ereignis planen** aus, oder wechseln Sie direkt zur Webseite Create Event in [AltspaceVR (Ereignis in AltspaceVR erstellen).](https://account.altvr.com/events/new)

1. **Ereignistitel:** Geben Sie den Namen des Ereignisses ein. Halten Sie es spezifisch und präzise für die Anzeige der verschiedenen Kalenderansichten auf der AltspaceVR-Website und der in-world-Schnittstelle. Versuchen Sie, den Titel unter 23 Zeichen zu halten, einschließlich Leerzeichen zwischen Wörtern.
2. **Beschreibung:** Geben Sie die Beschreibung des Ereignisses ein.
    * Muss mindestens 10 Zeichen in der Beschreibung enthalten, sonst wird Ihr Ereignis nicht erstellt.
    * Fügen Sie einen leeren Bereich zwischen Absätzen hinzu.
    * Um einen Link zu Facebook, Discord, Website oder anderen Ressourcen Ihres Ereignisses hinzuzufügen, verwenden Sie das folgende Format (dieses Markdown funktioniert nur auf der Promotion Page Ihres Ereignisses auf der Website, dies wird in den AltspaceVR-Menüs nicht ordnungsgemäß gerendert): `[Event Name](http://example.com/)`

3. **Startdatum/Enddatum:** Legen Sie die Startzeit fest, und stellen Sie sicher, dass die Endzeit nach der Startzeit liegt.
4. **Kategorie:** Wählen Sie die Kategorie aus, die Ihren Ereignistyp am besten beschreibt. 
5. Legen Sie das Ereignis auf **Privat** oder **Öffentlich** fest.
    * Sichtbarkeit: Öffentliche Ereignisse sind auf der [Registerkarte Alle](https://account.altvr.com/events/all) des AltspaceVR-Websiteereigniskalenders sichtbar und für die Öffentlichkeit geöffnet.
    * Private Ereignisse sind in den AltspaceVR-Ereigniskalendern nicht sichtbar und erfordern die Ereignis-URL, um in den Ereignisbereich zu gelangen.
    * Wenn Sie "Als Hauptereignis hinzufügen" möchten, muss das Ereignis auf public festgelegt werden.
6. **Wählen Sie eine Vorlage aus:** Auf der rechten Seite der Webseite befindet sich eine Liste mit Miniaturbildern der verfügbaren Vorlagen in AltspaceVR. Es gibt Spielräume, Büros, Besprechungsräume, Präsentationsräume und Spaß-Meetup-Räume. Wählen Sie einen aus, der interessant aussieht. Wenn Ihnen dies nicht gefällt, erstellen Sie einfach ein neues Ereignis mit einer neuen Vorlage. Wenn Sie Ihre eigene benutzerdefinierte Event World erstellen möchten, wählen Sie **Cool Sky** als Standardvorlage aus, und befolgen Sie die nachstehenden Anweisungen zum Importieren Ihrer Welt.
7. Wählen Sie **ERWEITERTE OPTIONEN aus.**

### <a name="advanced-options"></a>Erweiterte Optionen

1. **Promote (Bewerben):** Jedes Ereignis erfordert zwei Brandingbilder (diese Bilder werden auf der AltspaceVR-Website und nicht in Ihrem Ereignis in AltspaceVR angezeigt):
    * **Kachel:** Das Kachelbild muss 1920 x 1080 Pixel betragen. Dieses Bild wird auf verschiedene Miniaturansichtsgrößen skaliert und mit anderen Ereignissen im AltspaceVR-Ereigniskalender angezeigt. Stellen Sie sicher, dass das Bild klar ist und nicht viel Text enthält. Verwenden Sie keine urheberrechtlich geschützten Bilder/Logos, die Sie nicht besitzen.
    * **Banner:** Die Bannerbilder müssen 1920 x 576 sein. Die Größe wird bei Bedarf automatisch geändert und wird auf den Ereignisinformationen oder auf der Webseite angezeigt. Eine halbtransparente Überlagerung deckt die unteren 25 % des Bilds ab. Vermeiden Sie es, Text in diesem Bereich zu platzieren.
    * Eine weitere (schnellere) Option ist das Kopieren eines Kachelbilds in ein Hintergrundbannerbild. Dabei wird auch Ihr Kachelbild als Bannerbild verwendet. Probieren Sie es :). Wenn es nicht gut ausschaut, können Sie ein neues Bannerbild erstellen.
2. **In VR:** Dieser Abschnitt enthält Features, die für die virtuelle Umgebung während des Ereignisses innerhalb der AltspaceVR-App gelten:
    * **Kontextbezogene Standardrollen:** Das grüne Fragezeichen listet die spezifischen Rollen auf, die *allen Zielgruppenmitgliedern im Ereignis zur Verfügung stehen.* Am häufigsten wird *megaphone_only.* Fügen Sie diese Option hinzu, um allen Mitgliedern der Zielgruppe unter der Schaltfläche "Hosttools" die Option "Amplify My Voice" zu geben, damit sie bei einem großen Bereich über Ihr Ereignis hinweg gehört werden können. Wenn Ihr Ereignis einen Flug erfordert, fügen Sie *pilot hinzu.* Um beide hinzuzufügen, ist das Format: *megaphone_only, Pilot*. Jeder Benutzer muss den Fly-Modus in der AltspaceVR-App aktivieren, indem er zu Einstellungen/Eingabe/Fly wechseln.
    * **Anweisungen:** Die [Anweisungen](../world-building/adding-welcome-messages.md) sind für Text, der bei der Ankunft im Raum ein Begrüßungsbild generiert. Benutzer müssen "OK" auswählen, um sie aus ihrer Ansicht zu entfernen. Dies wird häufig verwendet, um Zielgruppenanweisungen wie "Please stay muted until invited to speak" (Bitte bleiben Sie stumm, bis zum Sprechen eingeladen) oder "Welcome to XYZ event where we'll be covering ABC" (Willkommen bei der XYZ-Veranstaltung, bei der ABC erläutert wird) zur Verfügung zu stellen. Dies ist nicht erforderlich, verwenden Sie daher mit Umsicht. Sie können Markdown auch verwenden, um die Größe von Farbe und Schriftart hinzuzufügen. Weitere Details: [http://digitalnativestudios.com/textmeshpro/docs/rich-text](http://digitalnativestudios.com/textmeshpro/docs/rich-text)
3. **Erweitert:** Im Folgenden finden Sie eine kurze Erläuterung der erweiterten Features für Ereignisse (einige dieser Features werden erst angezeigt, nachdem Das Ereignis erstellt wurde und Sie das Ereignis bearbeiten):
    * **Administratoren:** Administratoren sind AltspaceVR-Benutzer, die Ihnen vertrauen, um Sie bei der Verwaltung Ihres Ereignisses zu unterstützen. Dies können Ihre Cohosts oder Sicherungshosts sein. Durch Hinzufügen ihres Benutzernamens zur Liste "Administratoren" haben sie die folgenden Zugriffe:
        * Ändern Sie den Titel, die Beschreibung und andere Features des Ereignisses.
        * Fügen Sie Kontextrollen für Moderatoren, Hosts und andere Rollen hinzu, und entfernen Sie sie.
        * Löschen Sie das Ereignis.
    * **Gruppe:** Wählen Sie über das [Dropdownmenü](group-features.md) aus Ihren privaten Gruppen aus. Wird nur angezeigt, wenn Ihr Konto einer Gruppe erstellt/hinzugefügt wurde.
    * **Tagline:** Dieser präzise Satz wird auf der Ereigniswebseite unter dem Titel angezeigt.
    * **Aus Welt importieren:** Um einen erstellten Weltereignisbereich für die wiederholte Verwendung zu verwenden, ist dies der Abschnitt des Formulars, der zum Importieren des Layouts und der Anpassung dieser Welt in Ihr Ereignis verwendet werden soll. Beachten Sie die folgenden Aspekte:

    **Importieren Sie Ihre eigene Welt:** Um eine Welt zu importieren, haben Sie Erstellt und besitzen:
    * Wählen Sie den Dropdownpfeil aus, um eine Liste der von Ihnen erstellten Welten zu sehen.
    * Wählen Sie die Welt aus.
    * Warten Sie nach Abschluss des restlichen Ereignisformulars mindestens 2 Minuten, bevor Sie den Ereignisbereich in AltspaceVR besuchen, um sicherzustellen, dass die Datenbankinformationen aktualisiert und die Welt generiert wird.
    
    **Verwenden Sie die Welt einer anderen Person:**
    * Wenden Sie sich an den Besitzer der Welt, um die Verwendung des Features **Für Freunde** freigeben in einer individuellen Welt an sie zu bitten, es für Sie zu teilen.

3. **YouTube-Video-ID:** Wird auf der Webseite des Ereignisses angezeigt. Dadurch werden YouTube-Ereignistrailer oder Videos zur Ereigniswebseite und nicht zur weltspezifischen Website hinzufügt. Sie benötigen nur den Video-ID-Teil der URL: dQw4w9WgXcQ
4. **Twitter-Handle:** Dadurch wird Ihr Twitter-Stream zur Webseite des Ereignisses addiert. Wenn es sich bei dem Twitter-Konto um ein persönliches Konto handelt, das nicht mit dem Ereignis oder der Zuordnung zusammenhing, werden Sie möglicherweise zu sehr geteilt. Sie benötigen nur das Handle: @elonmusk
5. **Kontextbezogene Rollen:** Hier steuern Sie die Übergeordneten oder [kontextbezogenen](../world-building/granting-roles.md) Rollen Ihrer Ereignishosts, Moderatoren und anderen Rollen innerhalb des Ereignisses. Um sie hinzuzufügen, geben Sie ihren AltspaceVR-Benutzernamen ein, und weisen Sie ihnen im Dropdownmenü eine Rolle zu. Um sie zu entfernen, aktivieren Sie das Kontrollkästchen Entfernen, und speichern Sie die Ereigniswebseite. HINWEIS: Wenn Sie eine Hostmoderationsfunktion gewähren möchten, müssen Sie sie als Host und Moderator hinzufügen. Die folgenden Kontextrollen sind derzeit verfügbar:
    * **Host:** Fügt der Schnittstelle der Einzelnen in AltspaceVR die [Front Row-Features](../faqs/front-row-events.md) hinzu, um diese Features hinzuzufügen.
    * **Moderator:** Fügt der Benutzeroberfläche der Einzelnen Moderationsfunktionen hinzu, einschließlich der Möglichkeit, jeden Teilnehmer zu texten, ihn global für das Ereignis zu stummschalten oder aus dem Ereignis zu entfernen. Fügen Sie den Host erneut hinzu, und geben Sie ihm Moderationsrollen, wenn Sie möchten, dass er über Moderationsberechtigungen verfügen soll.
    * **Nur Megaphone:** Fügt der Benutzeroberfläche über die Schaltfläche Hosttools die Schaltfläche "Meine Stimme verstärken" hinzu.
    * **Terraformer:** Fügt der Schnittstelle die Schaltfläche "Welt-Editor" hinzu.
    * **Pilot:** Fügt Flugfunktionen für diese Person hinzu. HINWEIS: Sie müssen dies in Einstellungen/Eingabe/Fly aktivieren.
    * **Performer:** Fügt Funktionen und Features hinzu, die mit Musik- und Musikereignissen verknüpft sind.
6. **Blockiert aufgelistete Benutzer:** Wenn Sie den Zugriff eines Benutzers blockieren möchten oder ein Benutzer zuvor von einem Moderator oder Host aus dem Ereignis entfernt und das Ereignis dupliziert wurde, wird der Name des benutzers aufgelistet, der als Block aufgeführt ist. Ereignishosts oder Administratoren können einen block aufgelisteten Benutzer jederzeit hinzufügen oder entfernen.

Nachdem das Formular vollständig und dreifach überprüft wurde, wählen Sie **CREATE EVENT aus.**

> [!IMPORTANT]
> Wenn Ihr Ereignis nicht ordnungsgemäß erstellt wird, stellen Sie sicher, dass ihre Beschreibung mindestens 10 Zeichen enthält und/oder Sie eine Vorlage ausgewählt haben. Der Name der Vorlage wird bei Auswahl von weiß in blau.

## <a name="event-page-actions"></a>Aktionen auf der Ereignisseite

Auf der Webseite Ereignis haben Sie die folgenden Aktionen und Optionen:

1. Wählen Sie **BEARBEITEN** aus, um Änderungen an den Ereigniseinstellungen vorzunehmen.
2. Wählen **Sie END EVENT** (EREIGNIS BEENDEN) aus, um das Ereignis zu beenden (z. B. wenn Ihr Ereignis zu früh beendet ist).
3. Wählen **Sie SET TO DRAFT aus,** um das Ereignis auf Entwurf anstatt auf Aktiv zu setzen.
4. Wenn Sie ein Update für Ihre importierte Welt vorgenommen haben, müssen Sie **RE-IMPORT WORLD** auswählen, damit diese Änderungen in Ihrem Ereignis angezeigt werden. Vergessen Sie nicht, den Speicherplatz im Ereignisbereich :)
5. Wählen **Sie DUPLICATE EVENT** aus, um das Ereignis für zukünftige Ereignisse zu duplizieren. Dieses Duplikat wird dann in Meine Ereignisse/Meine Entwurfsereignisse angezeigt. Sie müssen den neuen Tag/die neue Uhrzeit aktualisieren und von dort aus aktivieren.
6. Wählen Sie ADD AS MAIN EVENT (ADD **AS MAIN EVENT)** aus, um ihr Ereignis auf die Kalenderliste zu setzen.
7. Wählen **Sie DELETE EVENT** aus, wenn Sie das Ereignis vollständig löschen möchten (sie können es nicht wiederherstellen).

Wenn Sie bereit sind, wechseln Sie zum Menü Ereignisse **> Meine** Ereignisse in der AltspaceVR-Schnittstelle in der Welt, und geben Sie den Ereignisbereich zum Zurücksetzen des Speicherplatzes ein, überprüfen Sie Ihre Änderungen, oder fahren Sie mit der Anpassung fort. 

> [!IMPORTANT]
> Dies ist eine Kopie, und Anpassungen am Ereignisbereich gelten nur für dieses Ereignis. Wenn Sie viel Zeit damit verbringen, den Raum Ihres Ereignisses zu anpassen, ist es möglicherweise besser, eine Welt für Ihr **Wiederholtes Verwendungsereignis zu erstellen.**

Weitere Informationen zum Anpassen Ihres Ereignisraums oder zum Erstellen einer ursprünglichen Ereignisraum-Welt für den Import finden Sie hier:

* [Gewusst wie anderen Personen in meiner Welt Rollen zu gewähren?](../world-building/granting-roles.md)
* [Gewusst wie menschen in meiner Welt zu fliegt (oder über andere Fähigkeiten) verfügen?](../world-building/adding-user-abilities.md)
* [Wo finde ich Hilfe beim Erstellen von Welten?](../world-building/getting-help.md)
* [Gewusst wie ich meine Welten verwalten?](../world-building/managing-worlds.md)
* [Häufig gestellte Fragen zu World Building](../world-building/world-building-faq.md)
* [Gewusst wie meinen Welten benutzerdefinierte Spawnpunkte hinzufügen?](../world-building/adding-custom-spawn-points.md)
* [Gewusst wie eigene Kits hoch?](../world-building/uploading-custom-kits.md)
* [Gewusst wie erste Schritte mit dem World Building Toolkit (Unity Uploader)?](../world-building/world-building-toolkit-getting-started.md)

## <a name="using-the-multimedia-console-for-a-slide-presentation"></a>Verwenden der Multimediakonsole für eine Präsentation

Die Multimedia-Konsole ist eine hervorragende Möglichkeit, Ihre Inhalte für eine Präsentation zu organisieren, einschließlich Bildern, Audio oder Video. Befolgen Sie die [Anweisungen in der](multimedia-console.md) Multimedia-Konsole, um dieses Setup für Ihr Ereignis zu erhalten.

## <a name="branding-your-event-with-images"></a>Branding Ihres Ereignisses mit Bildern

Das Hinzufügen von Bildern zu Ihrem Ereignisbereich oder dem Logo und Branding Ihres Unternehmens oder sogar Fotos von sich selbst, Ihrem Team oder anderen visuellen Inhalten ist in AltspaceVR einfach.

Die Imageanforderungen sind:
* JPG- oder PNG-Dateien werden akzeptiert.
* Maximale Bildgröße: 1920 x 1080
* Lösung: 72 DPI
* Dateigröße: Weniger als 250 KB pro Datei

Der Prozess umfasst das Hochladen Ihres Bilds in [AltspaceVR Fotos](https://account.altvr.com/photos)und anschließendes Verwenden des Fotos im World Editor in der Welt, um sie zu importieren und in den Raum der Ereigniswelt zu platzieren.

1. Wechseln Sie [Fotos](https://account.altvr.com/photos) AltspaceVR-Website zu "Web".
2. Klicken Sie auf **Hochladen**.
3. Wählen **Sie Durchsuchen** aus, um ein Dialogfeld auf Ihrem Computer zu öffnen und das optimierte Image zu suchen und auszuwählen.
4. Klicken Sie auf **Öffnen**.
5. Wählen Sie **CREATE PHOTO (FOTO ERSTELLEN) aus.**
6. Wiederholen Sie dies für alle Ihre Images.

Positionieren Sie sich in AltspaceVR und in der Ereigniswelt in der Nähe des Orts, an dem Sie das Bild platzieren möchten. (Wenn Sie dies für ein **Wiederholtes** Verwenden-Ereignis erstellen, stellen Sie sicher, dass Sie sich in Ihrer Welt befinden und nicht im Ereignisbereich!)

1. Wählen Sie auf der Benutzeroberfläche in der unteren rechten Ecke die Option **World Editor/Editor Panel (Welt-Editor/Editor-Bereich) aus.**
2. Klicken Sie **unten auf** die Registerkarte Mine .
3. Wählen **Sie Fotos** aus.
4. Fotos werden in der chronologischen Reihenfolge des Uploads gespeichert, sodass das neueste hochgeladene Bild das erste Bild in der Liste sein sollte. Wählen Sie es aus, um es der Welt hinzuzufügen.
5. Greifen Sie mit dem Gerätecursor auf das Bild, und platzieren Sie es an der Stelle, an der sie sich bewegen möchten.
    * Sie können die Größe mit Ihren Controllern ändern (in der Regel gleiten Sie den Daumen horizontal über das Touchpad in VR oder verwenden Sie die Maus im 2D-Modus).
    * Um die Position und Drehung des Bilds zu optimieren, wählen Sie im Editor das **Zahnradsymbol** auf dem Bild aus, und legen Sie Drehung und Position entsprechend fest.
    * Sie können die Größe des Bilds auch mit dem Skalierungsfeature ändern.

> [!NOTE]
> Wenn der Bearbeitungsmodus aktiviert ist (orangefarbener Text), haben Sie automatisch die Möglichkeit zu fliegt, sodass Bilder leichter in der Ereigniswelt platziert werden können.

6. Wiederholen Sie dies für jede Bildplatzierung.
7. Wenn die Bilder eingerichtet sind, wählen Sie Alle sperren aus, wenn Sie sie nicht einzeln gesperrt haben, und deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den Editor. 
8. Verwenden Sie nur maximal fünf Fotos pro Ereignis.

## <a name="adding-3d-objects-using-world-editor-and-kits"></a>Hinzufügen von 3D-Objekten mit dem World-Editor und Kits

AltspaceVR ermöglicht das Importieren von 3D-Objekten in Welten mit dem World Editor. Es gibt viele World Editors Kits, die derzeit verwendet werden können, und vieles mehr. Es gibt Raumräume, Raketen, animierte Figuren, Wäge, Baumarten, Pflanzen und viele verschiedene Objekte. Oder Sie können Ihre eigenen Kits zur öffentlichen Sammlung oder für Ihre eigene persönliche Nutzung hinzufügen oder eine der [AltspaceVR MRE-Apps](../world-building/using-mixed-reality-extensions.md)verwenden, die interaktionsfähige Objekte in Ihre Welt bringen, z. B. Brillen, Brillen, Brillen, Brillen oder andere interaktionsfähige Objekte. Erwarten Sie, dass die Liste der Objekte bald erweitert wird.

Die Anweisungen hier konzentrieren sich auf die Verwendung von Elementen, die bereits in den Kits enthalten sind. Weitere Informationen zum Hinzufügen und Importieren von 3D-Objekten in AltspaceVR finden Sie unter "Importieren von [glTF-Modellen in meine Welten?"](../world-building/importing-models.md) und ["Gewusst wie eigene Kits hochladen?"](../world-building/uploading-custom-kits.md).

So fügen Sie Ihrer Ereigniswelt ein vorhandenes 3D-Objekt aus den World Building Kits hinzu, wenn der World Editor/Editor Panel geöffnet und der Bearbeitungsmodus aktiviert ist:

1. Erkunden Sie die Kits für das Objekt, das Sie importieren möchten, und wählen Sie es aus.
2. Wählen Sie das Kitobjekt mit dem Cursor aus, und positionieren Sie es. Verwenden Sie das ZAHNRADsymbol für das Objekt im World Editor, um die Optionen Position, Drehen und Skalieren für die manuelle Eingabe von Zahlen zu verwenden.
3. Wenn das Objekt an der rechten Position platziert wird, sperren Sie es, indem Sie auf das Symbol Sperren klicken.
4. Fügen Sie bei Wunsch ein weiteres -Objekt hinzu. Fügen Sie 3D-Objekte mit Umsicht hinzu, und behalten Sie ihre Auswahl auf nicht mehr als Elemente aus fünf verschiedenen einzelnen Kits bei, um die Oculus Quest-Benutzerunterstützung zu verbessern. Verwenden Sie nicht mehr als 200 Objekte auf einer Welt.
5. Wenn Sie fertig sind, sperren Sie alle Elemente, deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den Welt-Editor. Schlendern. Laden Sie einige Tester ein, um es zu besuchen und zu testen, und bereiten Sie sich auf Ihr großartiges Ereignis vor!

Weitere Informationen zu den World Editor Kits und zum Hinzufügen von 3D-Objekten zu AltspaceVR:

* [Was ist das Early Access Program?](../world-building/early-access.md)
* [Importieren von glTF-Modellen in meine Welten](../world-building/importing-models.md)
* [Gewusst wie mrE in meiner Welt verwenden?](../world-building/using-mixed-reality-extensions.md)

## <a name="how-to-record-or-live-stream-my-event"></a>Aufzeichnen oder Live Stream "Mein Ereignis"

Anweisungen zum Aufzeichnen oder Livestreaming Ihres Ereignisses finden Sie im folgenden Supportdokument:

* [Aufzeichnen oder Live Stream "Mein Ereignis"](recording-and-live-streaming.md)