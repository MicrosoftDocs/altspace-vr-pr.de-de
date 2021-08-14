---
title: Aufzeichnung und Livestreaming
description: Erfahren Sie, wie Sie AltspaceVR-Ereignisse von Ihrem PC aufzeichnen und live streamen, um sie für Ihre Benutzer zu bewerben und freizugeben.
ms.date: 04/26/2021
ms.topic: article
keywords: Streaming, Aufzeichnung, Video, Audio, Youtube, Obs
ms.openlocfilehash: 95a742cb2bfe5c277e698175bd9f657fcac5923d181c3eeb6905004d25f81aa6
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126106"
---
# <a name="recording-and-live-streaming"></a>Aufzeichnung und Livestreaming

Das Aufzeichnen und Livestreaming Ihrer AltspaceVR-Erfahrung, um anderen Personen auf der ganzen Welt zu zeigen, ist eine hervorragende Möglichkeit, Ihre Ereignisse, AltspaceVR und VR im Allgemeinen zu bewerben! Sehen Sie sich die folgenden Schritte an:

In diesem Artikel lernen Sie Folgendes:

* [Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Livestream an YouTube in AltspaceVR im 2D-Modus auf dem PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

1. AltspaceVR und OBS müssen installiert sein. Starten Sie AltspaceVR im 2D-Modus, starten Sie OBS, legen Sie OBS so fest, dass AltspaceVR erfasst und entfernt wird!

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen Sie **Windows** aus, um OBS herunterzuladen. In diesem Beitrag wird **OBS v22.0.2** verwendet.
3. Installieren von OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>Führen Sie ALTSPACEVR im 2D-Modus aus, BEVOR Sie OBS ausführen.

1. Laden Sie AltspaceVR von unserer Website herunter, und installieren Sie es: [altvr.com/get](https://altvr.com/getaltspacevr)
2. Stellen Sie sicher, dass Sie AltspaceVR im 2D-Modus starten, indem Sie das USB-Kabel Ihrer HMD von Ihrem PC trennen, oder wenn Sie einen Rift-Fehler haben: STRG+ALT+ENTF, Dienste, Oculus VR-Laufzeitdienst, Rechtsklick, Beenden. 
    * Dadurch wird Oculus deaktiviert und AltspaceVR im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und verwenden Sie Start, um den VR-Modus wieder abzurufen.

Jetzt Alt-Tab zu OBS:

1. Wählen Sie unter Quellen die Option **+ > Game Capture > Neu erstellen** aus.
2. Text in "AltspaceVR Capture" bearbeiten, **Quelle sichtbar machen** aktivieren und OK auswählen
3. Doppelklicken Sie unter Quellen auf **AltspaceVR Capture.**
4. Ändern des **Modus** in **Bestimmtes Fenster erfassen**
5. Fenster: [AltspaceVR.exe]: AltspaceVR
6. Fensterübertrefferpriorität: Übereinstimmungstitel, andernfalls Fenster derselben ausführbaren Datei suchen
7. Scrollen Sie nach unten zu Aufzeichnungscursor: untick
8. Klicken Sie auf „OK“.

Dadurch sollte AltspaceVR in OBS angezeigt werden. Um nun die folgenden Eigenschaften in OBS festzulegen, wechseln Sie zu **Datei > Einstellungen**:

|Registerkarte|Einstellungen|
|---|---|
| **Allgemein** | Behalten Sie die Standardeinstellung bei. |
| **Stream** | Behalten Sie die Standardeinstellung bei. |
| Ausgabemodus | Wechseln Sie zu Erweitert. |
| Registerkarte "Streaming" | Audiospur 1 <br> Encoder: x264 <br> Neuskalierungsausgabe: nicht angezeigt <br> Ratensteuerung: CBR <br> Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br> Keyframeintervall = 2 <br> CPU-Auslastungsvoreinstellung = sehr schnell |
| Registerkarte "Aufzeichnung" | Typ: Standard <br> Aufzeichnungspfad: D:/Video (Navigieren Sie zu dem Ort, an dem die Videodatei gespeichert werden soll) <br> Aufzeichnungsformat: mp4 (Wenn sie während der Aufzeichnung abstürzt, versuchen Sie hier flv anstelle von mp4. Wenn Sie einen Absturz erstellen, kann das Video weiterhin mit flv verwendet werden. <br> Audiospur 1 <br> Encoder: Streamencoder verwenden |
| Registerkarte "Audio" | Audiobitrate: 160 (für alle Spuren) |
| Registerkarte "Wiedergabepuffer" | Behalten Sie die Standardeinstellung bei. |
| **Audio** | Abtastrate: 48KHz <br> Kanäle: Stereo <br> Desktopaudiogerät: Standard <br> Desktopaudiogerät 2: Deaktivieren <br> Mic/Aux-Audiogerät: Standard |
| **Video** | Basisauflösung (Canvas): 1920x1080 <br> Ausgabeauflösung (skaliert): 1920x1080 <br> Downscale-Filter: Bicubic (Schärfte Skalierung, 16 Beispiele) <br> Allgemeine FPS-Werte: 30 |
| **Tastenkürzel** | Behalten Sie die Standardeinstellung bei. |
| **Erweitert** | Prozesspriorität: Normal | <br>

<br>Stellen Sie nun sicher, dass **Sie Übernehmen** und dann **OK** auswählen, um alle OBS-Einstellungen zu speichern. 

1. Alt-Tab zu AltspaceVR über, steigen Sie in den richtigen Raum/die richtige Welt/das richtige Ereignis ein, und stellen Sie Ihre Kamera (d. h. Ihren Avatar) ein, in dem wir ein Video aufzeichnen werden!
2. Alt-Tab zu OBS über, und wenn Sie bereit sind, klicken Sie auf **Aufzeichnung starten.**

Am unteren rechten Rand von OBS sehen Sie, dass REC: beginnt zu zählen, und der Punkt ist rot, was bedeutet, dass Sie aufzeichnen!

Erstellen Sie aus diesem Grund eine Testaufzeichnung: 
1. Öffnen/Schließen/Rollover der Menüs in AltspaceVR, um Benutzeroberflächensounds zu erzeugen
2. Stellen Sie sicher, dass Sie unveränderlich sind, z. B. "Sibilance, Sibilance", oder lassen Sie einen anderen Benutzer mit einem normalen Volume sprechen.
3. Sehen Sie sich die Desktopaudio- und Mic/Aux-Ebenen an, um zu sehen, ob sie funktioniert.

In der Regel stummschalten wir mic/Aux bei der Aufzeichnung. Wählen Sie das Lautsprechersymbol für Mic/Aux aus, und es wird rot mit einem X angezeigt.

* Es ist sehr schwierig, Ihre Audiodaten und die Audiodaten des anderen Benutzers abzugleichen, sodass das Mikrofon am besten stummgeschaltet wird, wenn Sie ein Ereignis aufzeichnen.
* Ein weiteres Problem bei Audiodaten ist die Einrichtung von OBS. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube auf Ihrem PC ansehen, werden diese Audio- oder Discord-Benachrichtigungen aufgezeichnet.
* Um nur die Audiodaten von AltspaceVR aufzuzeichnen, wechseln Sie zu Volume Mixer (klicken Sie mit der rechten Maustaste auf das Lautsprechersymbol unten rechts neben Windows), und stummschalten Sie Systemsounds, Browser usw., aber stummschalten Sie OBS oder AltspaceVR nicht.

> [!IMPORTANT]
> Vergessen Sie nicht, diese Volume Mixer-Einstellungen nach der Aufzeichnung wieder zu aktivieren.

Navigieren Sie nun zurück zu OBS, und wählen **Sie Aufzeichnung** aus Datei **beenden>Aufzeichnungen anzeigen** aus. Dadurch wird der Ordner mit Ihren OBS-Videodateien geöffnet, und doppelklicken Sie auf das Testvideo.

Manchmal ist die Aufzeichnung ziemlich laut, also setzen Sie den Schieberegler für Desktopaudio herunter, und erstellen Sie eine weitere Aufzeichnung zum Testen.


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Livestreaming auf YouTube im AltspaceVR 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

AltspaceVR und OBS müssen installiert sein. Starten Sie AltspaceVR im 2D-Modus, starten Sie OBS, entweder Livestreams, oder erstellen Sie ein "Neues Liveereignis" auf YouTube, richten Sie OBS mit Ihrem YouTube Stream Key ein, starten Sie das Streaming in OBS, starten Sie das Streaming auf YouTube, und Sie sind auf dem Spiel.

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen Sie **Windows** aus, um OBS herunterzuladen (in diesem Beitrag wird OBS v22.0.2 verwendet).
3. Installieren von OBS

Führen Sie ALTSPACEVR im 2D-Modus aus, BEVOR Sie OBS ausführen.
1. Laden Sie AltspaceVR von unserer Website herunter: [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. Um sicherzustellen, dass Sie AltspaceVR im 2D-Modus starten, trennen Sie entweder das USB-Kabel Ihrer HMD von Ihrem PC, oder wenn Sie einen Rift haben: STRG+ALT+ENTF, Dienste, Oculus VR-Laufzeitdienst, klicken Sie mit der rechten Maustaste auf Beenden. Dadurch wird Oculus Home deaktiviert und AltspaceVR im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und starten Sie erneut, um den VR-Modus abzurufen.

3. Alt-Tab zu OBS

4. Wählen Sie unter Quellen die Option **+** aus, wählen Sie Game Capture aus, Neu erstellen, Text in "AltspaceVR Capture" bearbeiten, Häkchen Quelle sichtbar machen, OK
5. Doppelklicken Sie auf AltspaceVR Capture.
6. Modus: Bestimmtes Fenster erfassen
7. Fenster: [AltspaceVR.exe]: AltspaceVR
8. Fensterübertrefferpriorität: Übereinstimmungstitel, andernfalls Fenster derselben ausführbaren Datei suchen
9. Scrollen Sie nach unten zu Aufzeichnungscursor: untick OK

Dadurch sollte AltspaceVR in OBS angezeigt werden. Sehr schön!

In OBS geht nun zu Datei>Einstellungen:

| Registerkarte | Einstellungen |
|---|---|
| Allgemein | Automatische Aufzeichnung beim Streaming aktivieren (dadurch wird zusätzlich zum Livestreaming eine Videodatei auf Ihrem Computer aufgezeichnet) |
| STREAM | Streamtyp: Streamingdienste <br> Dienst: YouTube/YouTube Gaming (kann auch an Twitch, Mixer, Facebook Live usw. gestreamt werden))<br>Server: Primärer YouTube-Erfassungsserver <br>Streamschlüssel: Fügen Sie Ihren Streamschlüssel von YouTube ein. (Siehe "Einrichten von Livestreaming auf YouTube" weiter unten) |
| Output | Ausgabemodus: Wechseln Sie zu Erweitert. |
| Streaming | Audiospur 1 <br>Encoder: x264 <br>Erzwingen der Encodereinstellungen des Streamingdiensts: Tick <br>Neuskalierungsausgabe: nicht angezeigt <br>Ratensteuerung: CBR <br>Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br>Keyframeintervall = 2 <br>CPU-Auslastungsvoreinstellung = sehr schnell |
| Aufzeichnung | Typ: Standard <br>Aufzeichnungspfad: D:/Video (Navigieren Sie zu dem Ort, an dem die Videodatei gespeichert werden soll, wenn Sie zuvor "Beim Streaming automatisch aufzeichnen" ausgewählt haben) <br>Aufzeichnungsformat: mp4 (Wenn sie während der Aufzeichnung abstürzt, versuchen Sie hier flv anstelle von mp4. Wenn Sie einen Absturz erstellen, kann das Video weiterhin mit flv verwendet werden. <br>Audiospur 1 <br>Encoder: Streamencoder verwenden |
| Audio | Audiobitrate: 160 (für alle Spuren) Abtastrate: 48 KHz <br>Kanäle: Stereo <br>Desktopaudiogerät: Standard <br>Desktopaudiogerät 2: Deaktivieren <br>Mic/Aux-Audiogerät: Standard |
| Wiedergabepuffer | Behalten Sie die Standardeinstellung bei. |
| Video | Basisauflösung (Canvas): 1920x1080 <br>Ausgabeauflösung (skaliert): 1920x1080 <br>Downscale-Filter: Bicubic (Schärfte Skalierung, 16 Beispiele) <br>Allgemeine FPS-Werte: 30 |
| Tastenkürzel | Behalten Sie die Standardeinstellung bei. |
| Fortgeschrittene | Prozesspriorität: Normal |
|||

<br>Stellen Sie nun sicher, dass Sie auf Übernehmen, dann auf OK und dann auf OBS schließen und erneut öffnen. Dadurch werden Ihre gesamten OBS-Einstellungen gespeichert. Gut :)

Im Abschnitt "Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC" weiter oben finden Sie Anweisungen zum Testen der Aufzeichnung mithilfe einer lokalen Aufzeichnung anstelle des Livestreams und zum Einrichten der Kameraaufnahme vor der Aufzeichnung.

Ein weiteres Problem bei Audiodaten ist die Einrichtung von OBS. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube ansehen, zeichnet es diese Audiodaten auf, Teams Nachrichten oder Benachrichtigungsgeräusche.

Um nur die Audiodaten von AltspaceVR aufzuzeichnen, wechseln Sie zu Volume Mixer (klicken Sie mit der rechten Maustaste auf das Lautsprechersymbol unten rechts neben Windows) und Stummschalten von Systemsounds, Browsern usw., aber stummschalten Sie OBS oder ALTSPACEVR nicht.

Vergessen Sie nicht, die Audiodaten nach der Aufzeichnung wieder zu aktivieren ;)

Herzlichen Glückwunsch, Sie sind ein AltspaceVR-Videorecorder!

## <a name="setting-up-live-streaming-on-youtube"></a>Einrichten von Livestreaming auf YouTube

Sie können entweder schnell einen Livestream in Betrieb nehmen (**Stream**) oder ein zukünftiges Livestreamereignis einrichten (**Verwalten**). Es kann empfohlen werden, dass Sie die Methode "Verwalten" einrichten.

1. Öffnen Sie Ihren Browser, melden Sie sich [https://www.youtube.com/](https://www.youtube.com/) an, und wechseln Sie dann zu . [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. Klicken Sie oben rechts auf Ihr Kontosymbol, und wählen Sie in der Dropdownleiste Creator Studio aus.
3. LIVE STREAMING auf der linken Seite der Seite.

**'Stream** now'-Methode:

* Wählen Sie BEARBEITEN aus, um Ihre Livestreaminformationen einzugeben.<br>
* Behalten Sie unter Stream Einstellungen die Standardwerte bei.<br>
* Streamschlüssel (In Encoder einfügen), "Reveal" auswählen und diesen Schlüssel kopieren, damit Sie ihn in OBS einfügen können<br>
* Öffnen von OBS/Einstellungen/Stream<br>
* Fügen Sie den Stream-Schlüssel von YouTube in das Feld Stream Key in OBS ein.<br>
* Anwenden und dann OK<br>
* Wählen Sie Streaming in OBS starten aus.<br>
* Wechseln Sie zu YouTube, und Sie werden sehen, dass Sie jetzt LIVE auf YouTube sind!<br>
* Um Ihre tatsächliche YouTube-Livestream-Videoseite anzuzeigen, müssen Sie oben rechts das Symbol FREIGEBEN auswählen.<br>
* Kopieren Sie den Link "Video", und fügen Sie ihn in eine neue Browserregisterkarte ein. Daraufhin wird Ihre YouTube-Livestreamseite angezeigt.<br>
* Diese URL ist Ihr Livestreamlink und kann für alle Ihre Social Media-Kanäle freigegeben :)<br>
* Um den Livestream zu beenden, wählen Sie Streaming auf OBS beenden aus. Dadurch wird der Livestream auf YouTube beendet.<br>
* Beenden Sie dann den Stream auf YouTube.<br>

**"Manage"-Methode:**
* Wählen Sie "Stream planen" aus.
* Erstellen eines neuen oder wiederverwenden Einstellungen, wenn Sie bereits einen vorherigen verwalteten Livestream eingerichtet haben
* Hinzufügen von Titel, Datum, Startzeit, Beschreibung, Hochladen Miniaturansicht und Tags – Vergessen Sie nicht, altspaceVR :)
* Wählen Sie im Dropdownmenü Öffentlich aus (Standardwert ist "Nicht aufgeführt").
* Standardwerte verwenden
* Kopieren des Streamschlüssels (Einfügen in den Encoder)
* Um Ihre tatsächliche YouTube-Livestream-Videoseite anzuzeigen, müssen Sie oben rechts das Symbol FREIGEBEN auswählen. Dies ist Ihr YouTube-Livestream-Ereignislink, der auf Social Way vor Ihrem eigentlichen Ereignis freigegeben werden kann.
* Jetzt OBS öffnen
* Datei/Einstellungen
* STREAM
* Fügen Sie den kopierten Streamschlüssel in das Feld Streamschlüssel ein.
* Anwenden und dann OK
* Wählen Sie "Streaming starten" aus.
* Zurück zu YouTube wird das Fenster "Vorschau" mit Ihrem Stream angezeigt, und GO LIVE wird jetzt oben rechts angezeigt.
* Wählen Sie GO LIVE (LIVE) aus.
* Sie sind jetzt LIVE!
* Wechseln Sie zu Ihrer Browserregisterkarte, und öffnen Sie den Link "Auf Überwachungsseite anzeigen", um sicherzustellen, dass das Video gut aussieht. DENKEN Sie daran, dass Sie die Audiodaten nicht hören, da Sie audio von Ihren Browsern ausgeschaltet haben, wenn Sie sie in Windows Volume Mixer stummgeschaltet haben. Überprüfen Sie die Audiodaten auf Ihrem Telefon, oder bitten Sie einen Freund, die Audiodaten für Sie zu überprüfen.
* Gut aussehen!
* Alt-Tab zurück zu AltspaceVR, um Ihre Kamera (d. h. Ihren Avatar) in Ihrem Ereignis zu bewegen.
* Wenn Sie mit dem Livestream fertig sind, kehren Sie zur YouTube-Seite "Live Control Room" zurück.
* Wählen Sie "Streaming beenden" aus.
* Das Dialogfeld wird geöffnet, und Sie werden gefragt, ob Sie das Streaming des Liveereignisses beenden möchten. OK
* Wechseln Sie zu OBS, und wählen Sie auch Streaming beenden aus.
* Herzlichen Glückwunsch, Sie sind jetzt ein AltspaceVR-Streamer!

Um Bonuspunkte zu erhalten, teilen Sie Ihre Videos in sozialen Medien mit der Welt, und markieren Sie uns @AltspaceVR :)