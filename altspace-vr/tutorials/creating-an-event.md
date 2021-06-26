---
title: Erstellen einer Veranstaltung
description: Erfahren Sie mehr über AltspaceVR-Ereignisse, deren Erstellung und das Hinzufügen von Branding- und 3D-Objekten mit dem World Editor.
ms.date: 03/11/2021
ms.topic: article
keywords: Events, Terminologie, Konsole, Multimedia, World Editor, Livestream
ms.openlocfilehash: 1e758b35b3bd5d5a580eb04e683d6b1dc4500b43
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923037"
---
# <a name="creating-an-event"></a>Erstellen einer Veranstaltung

Dies ist eine Schritt-für-Schritt-Anleitung zum Erstellen von Ereignissen in AltspaceVR. Es wird dringend empfohlen, an mehreren Veranstaltungen in AltspaceVR teilzunehmen, um ein Gefühl dafür zu bekommen, wie sie funktionieren. Im [AltspaceVR-Ereigniskalender](https://account.altvr.com/events) finden Sie eine Liste aller Ereignisse.

In diesem Artikel lernen Sie Folgendes:

* AltspaceVR-Ereignisterminologie
* Erstellen Ihres Ereignis- und Ereignisraums oder ihrer Welt
* Verwenden der Multimediakonsole für eine Präsentation
* Branding Ihres Ereignisses mit Bildern
* Hinzufügen von 3D-Objekten mit dem World Editor/Kits
* Aufzeichnen oder Live Stream "Mein Ereignis"

## <a name="altspacevr-event-terminology"></a>AltspaceVR-Ereignisterminologie

Im Folgenden finden Sie Begriffe, mit deren Hilfe Sie Ihren Ereignis- und Ereignisbereich erstellen müssen:

</br>

| Begriff | Definition |
|---|---|
| World Building | AltspaceVR bietet die Möglichkeit, virtuelle Welten zu erstellen und anzupassen. AltspaceVR-Hosts unterstützen Dokumentationen, Diskord-Kanäle und in der Welt orientierte Ereignisse, um mehr darüber zu erfahren, wie Sie Hilfe erhalten und mit dem Erstellen von [Welten beginnen können.](../world-building/world-building-faq.md) |
| World | Eine Welt ist ein virtueller Raum in AltspaceVR. Dabei kann es sich um ein Büro oder um einen großen Mountain Range-Bereich(n) geben. Es ist eine hochgradig anpassbare Umgebung. Es befindet sich innerhalb eines Universes, und es kann mehrere Welten in diesem Universe geben. Wenn Sie mehrere Ereignisräume für spezielle Ereignisse, Schulungszentren und verschiedene Besprechungsräume einrichten möchten, fügen Sie die Welten unter demselben Universe hinzu, um sie als Gruppe zusammen zu halten. |
| Universe | Ein Universe in altspaceVR world building vernacular stellt die Kategorisierung Ihrer Welten dar. Jedes Universe kann mehrere Welten besitzen. Die Welten erben die Einstellungen des Weltalls, was das Hinzufügen von Personen zur Liste der Zulässigen für mehrere Welten und andere Steuerungsfeatures einfach macht. Weitere [Informationen finden Sie unter Verwalten](../world-building/managing-worlds.md) Ihrer Welten. |
| Vorlage | Eine Vorlage (oder Raumvorlage) ist eine vorgefertigte Welt oder Umgebung, die verwendet werden kann, anstatt eine Mithilfe der World Building-Features zu erstellen. AltspaceVR bietet eine Vielzahl von Vorlagen für verschiedene Erfahrungen und Ereignisse. |
| Ereignisbereich | Ein Ereignisraum ist ein Synonym für die Welt in AltspaceVR. Im Allgemeinen bezieht er sich auf eine Welt, die zum Hosten von Ereignissen verwendet wird. |
| Website | Verweise auf die "Website" sind auf die [AltspaceVR-Website](https://altvr.com/). Es ist oft einfacher, Ereignisse über die [Webseite Ereignisse](https://account.altvr.com/events/my) auf einem Computer oder Tablet und nicht über Ihr VR-Gerät zu erstellen und zu bearbeiten. Sie müssen auch auf die Website zugreifen, um [die Welt zu](../world-building/managing-worlds.md) erstellen. |
| Kontextbezogene Rollen | [Kontextbezogene Rollen](../getting-started/roles.md) werden vom Ereignisersteller oder World Builder zugewiesen. Diese Rollen bieten Benutzern in einer Welt oder einem Ereignisbereich zusätzliche Features und Funktionen. Derzeit bestehen diese aus Host, Moderator, Pilot (Flight), Terraformer (World Building) und Megaphone Only. Diese können einzeln oder global zugewiesen werden, sodass jeder die gleichen Rollen im Ereignisbereich oder in der Welt haben kann. |
| Benutzeroberfläche (BENUTZEROBERFLÄCHE)/Menü | Wenn Sie sich in AltspaceVR in der Welt befinden, befinden sich in der immersiven Umgebung links und rechts auf dem Bildschirm Menüs. Das Kreis- oder Hauptmenü mit dem AltspaceVR-Logo öffnet die Hauptbenutzeroberfläche (UI) oder das Menü, um auf verschiedene Bildschirme zu zugreifen, um AltspaceVR zu erkunden und Ihre Benutzeroberfläche zu anpassen. Optionale Benutzeroberflächenelemente befinden sich auf der richtigen Bildschirmgröße und enthalten in der Regel Den Welt-Editor und Hosttools. Diese werden geöffnet und mit ihnen interagiert, indem Sie mit dem Cursor darauf klicken. |
| SDK/MRE | Dies sind Begriffe, die mit dem Software Development Kit und den [Mixed Reality-Erweiterungen](../world-building/using-mixed-reality-extensions.md) verbunden sind, die zum Hinzufügen von Features und Funktionen zur Entwicklungserfahrung in der Welt verwendet werden. Diese gelten in der Regel für fortgeschrittene Benutzer. |

## <a name="understanding-events"></a>Grundlegendes zu Ereignissen

AltspaceVR vereinfacht das Erstellen einer Welt, in der Sie einen vorgefertigten Vorlagenbereich verwenden können, um Ihre speziellen Anforderungen zu verwenden oder anzupassen, oder eine Welt von Grund auf neu zu erstellen. In diesem Artikel wird die Verwendung einer vorgefertigten Vorlage zum Erstellen Ihres Ereignisses behandelt. Die folgenden Abschnitte zu [Branding Your Event with Images](#branding-your-event-with-images) (Branding Ihres Ereignisses mit Bildern) und Adding 3D Objects using World Editor and Kits (Hinzufügen von [3D-Objekten](#adding-3d-objects-using-world-editor-and-kits) mit dem World Editor und Kits) enthalten Tipps zur weiteren Anpassung. Um Informationen zum Erstellen einer benutzerdefinierten Welt von Grund auf zu erhalten, besuchen Sie die World Building Tour-Meetups in AltspaceVR, und sehen Sie sich die [Dokumentation zum World Building-Support an.](../world-building/world-editor-getting-started.md)

AltspaceVR bietet zwei Möglichkeiten, einen Raum für Ihr Ereignis zu erstellen.

* **Einmalige Verwendung:** Erstellen Sie ein Ereignis, und wählen Sie eine Vorlagenwelt aus.
* **Wiederholte Verwendung:** Erstellen Sie einen Raum in der Welt, und importieren Sie ihn in das Ereignis.

Der Prozess zum Erstellen eines Ereignisses ist für [](../world-building/managing-worlds.md) beide identisch, mit einer Ausnahme: der Erstellung einer Welt und dem Importieren als Wiederholungsereignisbereich. Außerdem müssen Sie Wissen über Dies wissen:

</br>

| Begriff | Definition |
|---|---|
| World copied | Die Verwendung eines Weltraums für ein wiederholtes Ereignis ermöglicht eine dauerhafte Anpassung. Zeichen, Bilder, Spawnpunkte und andere Anpassungen werden von Ereignis zu Ereignis beibehalten, anstatt den Ereignisraum jedes Mal zu anpassen. |
| Anpassen von Event World | Wenn ein Ereignis erstellt wird, wird die Vorlage oder die importierte Welt kopiert und in dieses Ereignis gesperrt. Möglicherweise nehmen Sie Änderungen an der Ereigniswelt vor und wirken sich nicht auf die ursprüngliche Welt und umgekehrt aus. Erwägen Sie das Hinzufügen von Feiertagsdekorationen, Bildern oder anderen zierlich einmaligen Elementen des Welt-Editors, um den Ereignisraum zierlich und für das Ereignis geeigneter zu gestalten. |

Änderungen, die an der ursprünglichen Welt vorgenommen werden, werden nicht in der Ereigniswelt vorgenommen, es sei denn, der Ereignisbereich wird aktualisiert:
1. Verwenden Sie **die Schaltfläche RE-IMPORT WORLD** auf der Ereigniswebseite.
2. Lassen Sie zwei bis drei Minuten für den Abschluss der Synchronisierung zu. 
3. Wenn sich der Ereignisbereich nicht geändert hat, wechseln Sie zu Einstellungen > Moderate > **Reset Space** (Speicherplatz zurücksetzen), um den Ereignisspeicherplatz zurückzusetzen. Sie werden Speicherplatz viel als Ersteller der Welt zurücksetzen!

Wenn sie technische Probleme haben, z. B. elemente, die nicht ordnungsgemäß geladen werden, wechseln Sie zum AltspaceVR-Menü, und wählen Sie Einstellungen **> Moderate > Reset Space** aus, um den Ereignisbereich zurückzusetzen und die neuen Änderungen zu sehen. Windows-PC-Benutzer in 2D können die Tastenkombination **STRG+ALT+R** in AltspaceVR verwenden, um den Speicherplatz schnell zurückzusetzen.

## <a name="creating-your-event-and-event-space-or-world"></a>Erstellen Ihres Ereignis- und Ereignisraums oder ihrer Welt

Im Folgenden finden Sie eine Schritt-für-Schritt-Anleitung zum Erstellen eines Ereignisses für ein einmaliges oder wiederholtes Ereignis. Durch Auswählen der Vorlage oder Importieren einer Welt für das Ereignis. 

> [!NOTE]
> Die Webseite altspaceVR-Ereignisse bietet Anweisungen zu jedem Aspekt des Formulars mithilfe von grünen Fragezeichenschaltflächen. Bewegen Sie den Cursor auf diese, um bestimmte Anweisungen zu erhalten.

Wählen Sie [auf](https://account.altvr.com/events/my) > der Website von AltspaceVR auf  der Webseite Ereignisse > Meine Ereignisse die Option Ereignis planen aus, oder wechseln Sie direkt zur Webseite Ereignis [in AltspaceVR erstellen.](https://account.altvr.com/events/new)

1. **Ereignistitel:** Geben Sie den Namen des Ereignisses ein. Halten Sie sie für die Anzeige in den verschiedenen Kalenderansichten auf der AltspaceVR-Website und der in der Welt verfügbaren Benutzeroberfläche spezifisch und präzise. Versuchen Sie, Ihren Titel unter 23 Zeichen zu halten, einschließlich Leerzeichen zwischen Wörtern.
2. **Beschreibung:** Geben Sie die Beschreibung des Ereignisses ein.
    * Die Beschreibung muss mindestens 10 Zeichen enthalten, da das Ereignis nicht erstellt wird.
    * Fügen Sie ein leeres Leerzeichen zwischen Absätzen hinzu.
    * Verwenden Sie das folgende Format, um einen Link zur Facebook-, Discord-, Website- oder anderen Ressourcen Ihres Ereignisses hinzuzufügen (dieses Markdown funktioniert nur auf der Promotion-Seite Ihres Ereignisses auf der Website, die in den AltspaceVR-Menüs nicht ordnungsgemäß gerendert wird): `[Event Name](http://example.com/)`

3. **Startdatum/Enddatum:** Legen Sie die Startzeit fest, und stellen Sie sicher, dass die Endzeit nach der Startzeit liegt.
4. **Kategorie:** Wählen Sie die Kategorie aus, die Ihren Ereignistyp am besten beschreibt. 
5. Legen Sie das Ereignis auf **Private oder** **Public fest.**
    * Sichtbarkeit: Öffentliche Ereignisse werden auf der Registerkarte Alle [](https://account.altvr.com/events/all) des AltspaceVR-Website-Ereigniskalenders angezeigt und sind öffentlich zugänglich.
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
    * **Anweisungen:** Die [Anweisungen](../world-building/adding-welcome-messages.md) sind für Text, der bei der Ankunft im Raum ein Begrüßungsbild generiert. Benutzer müssen "OK" auswählen, um sie aus ihrer Ansicht zu entfernen. Dies wird häufig verwendet, um Zielgruppenanweisungen wie "Please stay muted until invited to speak" (Bitte bleiben Sie stumm, bis zum Sprechen eingeladen) oder "Welcome to XYZ event where we'll be covering ABC" zu geben. Dies ist nicht erforderlich, verwenden Sie daher mit Umsicht. Sie können markdown auch verwenden, um die Größe von Farbe und Schriftart hinzuzufügen. Weitere Details: [http://digitalnativestudios.com/textmeshpro/docs/rich-text](http://digitalnativestudios.com/textmeshpro/docs/rich-text)
3. **Erweitert:** Im Folgenden finden Sie eine kurze Erläuterung der erweiterten Funktionen für Ereignisse (einige dieser Features werden erst angezeigt, nachdem Das Ereignis erstellt wurde und Sie das Ereignis bearbeiten):
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
    * Wenden Sie sich an den Besitzer der Welt, um zu fordern, dass er das Feature **Mit** Freunden teilen in einer individuellen Welt verwendet, um es für Sie zu teilen.

3. **YouTube-Video-ID:** Wird auf der Webseite des Ereignisses angezeigt. Dadurch werden YouTube-Ereignistrailer oder Videos zur Ereigniswebseite und nicht zu weltweiten Videos addiert. Sie benötigen nur den Video-ID-Teil der URL: dQw4w9WgXcQ
4. **Twitter-Handle:** Dadurch wird Ihr Twitter-Stream zur Webseite des Ereignisses addiert. Wenn es sich bei dem Twitter-Konto um ein persönliches Konto handelt, das nicht mit dem Ereignis oder der Zuordnung zusammenhing, wird die Freigabe möglicherweise zu hoch sein. Sie benötigen nur das Handle: @elonmusk
5. **Kontextbezogene Rollen:** Hier steuern Sie die Übergeordneten oder [kontextbezogenen](../world-building/granting-roles.md) Rollen Ihrer Ereignishosts, Moderatoren und anderen Rollen innerhalb des Ereignisses. Um sie hinzuzufügen, geben Sie ihren AltspaceVR-Benutzernamen ein, und weisen Sie ihnen im Dropdownmenü eine Rolle zu. Um sie zu entfernen, aktivieren Sie das Kontrollkästchen Entfernen, und speichern Sie die Ereigniswebseite. HINWEIS: Wenn Sie eine Hostmoderationsfunktion gewähren möchten, müssen Sie sie als Host und Moderator hinzufügen. Die folgenden Kontextrollen sind derzeit verfügbar:
    * **Host:** Fügt der Schnittstelle der Einzelnen in AltspaceVR die [Front Row-Features](../faqs/front-row-events.md) hinzu, um diese Features hinzuzufügen.
    * **Moderator:** Fügt der Benutzeroberfläche der Einzelnen Moderationsfunktionen hinzu, einschließlich der Möglichkeit, jeden Teilnehmer zu texten, ihn global für das Ereignis zu stummschalten oder aus dem Ereignis zu entfernen. Fügen Sie den Host erneut hinzu, und geben Sie ihm Moderationsrollen, wenn Sie möchten, dass er über Moderationsberechtigungen verfügen soll.
    * **Nur Megaphone:** Fügt der Benutzeroberfläche über die Schaltfläche Hosttools die Schaltfläche "Meine Stimme verstärken" hinzu.
    * **Terraformer:** Fügt der Schnittstelle die Schaltfläche "Welt-Editor" hinzu.
    * **Pilot:** Fügt Flugfunktionen für diese Person hinzu. HINWEIS: Sie müssen dies unter Einstellungen/Eingabe/Fly aktivieren.
    * **Performer:** Fügt Funktionen und Features hinzu, die mit Musik- und Musikereignissen verknüpft sind.
6. **Blockiert aufgelistete Benutzer:** Wenn Sie den Zugriff eines Benutzers blockieren möchten oder ein Benutzer zuvor von einem Moderator oder Host aus dem Ereignis entfernt wurde und das Ereignis dupliziert wurde, wird der Name des aufgelisteten Benutzers aufgelistet. Ereignishosts oder Administratoren können einen block aufgelisteten Benutzer jederzeit hinzufügen oder entfernen.

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
6. Wählen Sie ADD AS MAIN EVENT (ADD **AS MAIN EVENT)** aus, um Ihr Ereignis auf die Kalenderliste zu setzen.
7. Wählen **Sie DELETE EVENT** aus, wenn Sie das Ereignis vollständig löschen möchten (sie können es nicht wiederherstellen).

Wenn Sie bereit sind, wechseln Sie auf der altspaceVR-Benutzeroberfläche zum Menü Ereignisse **> Meine** Ereignisse, und geben Sie den Ereignisbereich zum Zurücksetzen des Speicherplatzes ein, überprüfen Sie Ihre Änderungen, oder fahren Sie mit der Anpassung fort. 

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

Der Prozess umfasst das Hochladen Ihres Bilds in Ihre [AltspaceVR Photos](https://account.altvr.com/photos)und anschließendes Verwenden der Fotos im World Editor in der Welt, um sie zu importieren und in den Raum der Ereigniswelt zu platzieren.

1. Wechseln Sie [auf der](https://account.altvr.com/photos) AltspaceVR-Website zu Fotos.
2. Klicken Sie auf **Hochladen**.
3. Wählen **Sie Durchsuchen** aus, um ein Dialogfeld auf Ihrem Computer zu öffnen und das optimierte Image zu suchen und auszuwählen.
4. Klicken Sie auf **Öffnen**.
5. Wählen Sie **CREATE PHOTO (FOTO ERSTELLEN) aus.**
6. Wiederholen Sie dies für alle Ihre Images.

Positionieren Sie sich in AltspaceVR und in der Ereigniswelt in der Nähe des Orts, an dem Sie das Bild platzieren möchten. (Wenn Sie dies für ein **Wiederholtes** Verwenden-Ereignis erstellen, stellen Sie sicher, dass Sie sich in Ihrer Welt befinden und nicht im Ereignisbereich!)

1. Wählen Sie auf der Benutzeroberfläche in der unteren rechten Ecke die Option **World Editor/Editor Panel (Welt-Editor/Editor-Bereich) aus.**
2. Klicken Sie **unten auf** die Registerkarte Mine .
3. Wählen Sie **Fotos aus.**
4. Fotos werden in der chronologischen Reihenfolge des Uploads gespeichert, sodass das neueste hochgeladene Bild das erste Bild in der Liste sein sollte. Wählen Sie es aus, um es der Welt hinzuzufügen.
5. Greifen Sie mit ihrem Gerätecursor auf das Bild, und platzieren Sie es an der Stelle, an der sie sich bewegen möchten.
    * Sie können die Größe mit Ihren Controllern ändern (in der Regel gleiten Sie den Daumen horizontal über das Touchpad in VR oder verwenden Sie die Maus im 2D-Modus).
    * Um die Position und Drehung des Bilds zu optimieren, wählen Sie im Editor das **Zahnradsymbol** auf dem Bild aus, und legen Sie Drehung und Position entsprechend fest.
    * Sie können die Größe des Bilds auch mit dem Skalierungsfeature ändern.

> [!NOTE]
> Wenn der Bearbeitungsmodus aktiviert ist (orangefarbener Text), haben Sie automatisch die Möglichkeit zu fliegt, sodass Bilder leichter in der Ereigniswelt platziert werden können.

6. Wiederholen Sie dies für jede Bildplatzierung.
7. Wenn die Bilder eingerichtet sind, wählen Sie Alle sperren aus, wenn Sie sie nicht einzeln gesperrt haben, und deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den Editor. 
8. Verwenden Sie nur maximal fünf Fotos pro Ereignis.

## <a name="adding-3d-objects-using-world-editor-and-kits"></a>Hinzufügen von 3D-Objekten mit dem World Editor und Kits

AltspaceVR ermöglicht das Importieren von 3D-Objekten in Welten mit dem World Editor. Es gibt viele World Editors Kits, die derzeit verwendet werden können, und vieles mehr. Es gibt Raumräume, Raketen, animierte Figuren, Wäge, Baumarten, Pflanzen und viele verschiedene Objekte. Oder Sie können Ihre eigenen Kits der öffentlichen Sammlung oder für Ihre eigene persönliche Nutzung hinzufügen oder eine der [AltspaceVR MRE-Apps](../world-building/using-mixed-reality-extensions.md)verwenden, die interaktionsfähige Objekte in Ihre Welt bringen, z. B. Brillen, Brillen, Brillen, Brillen oder andere interaktionsfähige Objekte. Erwarten Sie, dass die Liste der Objekte bald erweitert wird.

Die Anweisungen hier konzentrieren sich auf die Verwendung von Elementen, die bereits in den Kits enthalten sind. Weitere Informationen zum Hinzufügen und Importieren von 3D-Objekten in AltspaceVR finden Sie unter "Importieren von [glTF-Modellen in meine Welten?"](../world-building/importing-models.md) und ["Gewusst wie eigene Kits hochladen?"](../world-building/uploading-custom-kits.md).

So fügen Sie ihrer Ereigniswelt ein vorhandenes 3D-Objekt aus den World Building Kits hinzu, wenn der World Editor/Editor Panel geöffnet und der Bearbeitungsmodus aktiviert ist:

1. Erkunden Sie die Kits für das Objekt, das Sie importieren möchten, und wählen Sie es aus.
2. Wählen Sie das Kitobjekt mit dem Cursor aus, und positionieren Sie es. Verwenden Sie das ZAHNRADsymbol für das Objekt im World Editor, um die Optionen Position, Drehen und Skalieren für die manuelle Eingabe von Zahlen zu verwenden.
3. Wenn das Objekt an der rechten Position platziert wird, sperren Sie es, indem Sie auf das Symbol Sperren klicken.
4. Fügen Sie bei Wunsch ein weiteres -Objekt hinzu. Fügen Sie 3D-Objekte mit Umsicht hinzu, und halten Sie Ihre Auswahl auf nicht mehr als Elemente aus fünf verschiedenen einzelnen Kits, um die Oculus Quest-Benutzerunterstützung zu verbessern. Verwenden Sie nicht mehr als 200 Objekte auf einer Welt.
5. Wenn Sie fertig sind, sperren Sie alle Elemente, deaktivieren Sie den Bearbeitungsmodus, und schließen Sie den Welt-Editor. Schlendern. Laden Sie einige Tester ein, um es zu besuchen und zu testen, und bereiten Sie sich auf Ihr großartiges Ereignis vor!

Weitere Informationen zu den World Editor Kits und zum Hinzufügen von 3D-Objekten zu AltspaceVR:

* [Was ist das Early Access Program?](../world-building/early-access.md)
* [Importieren von glTF-Modellen in meine Welten](../world-building/importing-models.md)
* [Gewusst wie mrE in meiner Welt verwenden?](../world-building/using-mixed-reality-extensions.md)

## <a name="how-to-record-or-live-stream-my-event"></a>Aufzeichnen oder Live Stream "Mein Ereignis"

Anweisungen zum Aufzeichnen oder Livestreaming Ihres Ereignisses finden Sie im folgenden Supportdokument:

* [Aufzeichnen oder Live Stream "Mein Ereignis"](recording-and-live-streaming.md)