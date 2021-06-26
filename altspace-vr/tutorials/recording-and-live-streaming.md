---
title: Aufzeichnung und Livestreaming
description: Erfahren Sie, wie Sie AltspaceVR-Ereignisse von Ihrem PC aufzeichnen und live streamen, um sie zu bewerben und für Ihre Benutzer zu teilen.
ms.date: 04/26/2021
ms.topic: article
keywords: Streaming, Aufzeichnung, Video, Audio, Youtube, Obs
ms.openlocfilehash: 0bf32d8ac7e2d409eb5e2c31a9da8a878e0e5eef
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923017"
---
# <a name="recording-and-live-streaming"></a>Aufzeichnung und Livestreaming

Das Aufzeichnen und Livestreaming Ihrer AltspaceVR-Umgebung, um andere Personen auf der ganzen Welt zu zeigen, ist eine hervorragende Möglichkeit, Ihr Ereignis, AltspaceVR und VR im Allgemeinen zu bewerben! Sehen Sie sich unten die ersten Schritte an:

In diesem Artikel lernen Sie Folgendes:

* [Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Livestream an YouTube in AltspaceVR im 2D-Modus auf dem PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

1. AltspaceVR und OBS müssen installiert sein. Starten Sie AltspaceVR im 2D-Modus, starten Sie OBS, richten Sie OBS so ein, dass AltspaceVR aufzeichnen und entfernt werden kann!

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen Sie **Windows** aus, um OBS herunterzuladen. In diesem Beitrag wird **OBS v22.0.2 verwendet.**
3. Installieren von OBS

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>AltspaceVR im 2D-Modus ausführen, bevor Sie OBS ausführen

1. Laden Sie AltspaceVR von unserer Website herunter, und installieren [Sie altvr.com/get](https://altvr.com/getaltspacevr)
2. Stellen Sie sicher, dass Sie AltspaceVR im 2D-Modus starten, indem Sie das HMD-USB-Kabel von Ihrem PC entpappen oder wenn Sie einen Rift haben: STRG+ALT+ENTF, Dienste, Oculus VR Runtime Service, Rechtsklick, Beenden. 
    * Dadurch wird Oculus deaktiviert und AltspaceVR im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und verwenden Sie Start, um den VR-Modus wieder zu erhalten.

Führen Sie Alt-Tab um zu OBS:

1. Wählen Sie unter Quellen die Option+ **> Game Capture > Create New (Neu erstellen) aus.**
2. Bearbeiten Sie Text in "AltspaceVR Capture", aktivieren Sie **Quelle sichtbar machen,** und wählen Sie OK aus.
3. Doppelklicken Sie unter Quellen **auf AltspaceVR Capture.**
4. Ändern **des Modus in** **"Bestimmtes Fenster erfassen"**
5. Fenster: [AltspaceVR.exe]: AltspaceVR
6. Übereinstimmungspriorität des Fensters: Übereinstimmungstitel, andernfalls Fenster der gleichen ausführbaren Datei suchen
7. Scrollen Sie nach unten zu Capture Cursor: untick
8. Klicken Sie auf „OK“.

Dies sollte dazu sorgen, dass AltspaceVR in OBS auftritt. Um nun die folgenden Eigenschaften in OBS festlegen zu können, wechseln Sie zu **Datei > Einstellungen:**

|Registerkarte|Einstellungen|
|---|---|
| **Allgemein** | Behalten Sie die Standardeinstellung bei. |
| **STREAM** | Behalten Sie die Standardeinstellung bei. |
| Ausgabemodus | Wechseln Sie zu Erweitert. |
| Registerkarte "Streaming" | Audiospur 1 <br> Encoder: x264 <br> Neuskalieren der Ausgabe: unticked <br> Ratensteuerung: CBR <br> Bitrate: 6000 (6000 für 30 Fps oder 9000 für 60 Fps) <br> Keyframe-Intervall = 2 <br> CPU-Auslastungsvoreinstellung = sehr schnell |
| Registerkarte "Aufzeichnung" | Typ: Standard <br> Aufzeichnungspfad: D:/Video (Navigieren Sie zu dem Ort, an dem die Videodatei gespeichert werden soll) <br> Aufzeichnungsformat: mp4 (Wenn Sie bei der Aufzeichnung abstürzen, versuchen Sie hier flv anstelle von mp4, wenn Sie abstürzen, kann das Video weiterhin mit flv verwendet werden.) <br> Audiospur 1 <br> Encoder: Streamencoder verwenden |
| Registerkarte "Audio" | Audiobitrate: 160 (für alle Spuren) |
| Registerkarte "Wiedergabepuffer" | Behalten Sie die Standardeinstellung bei. |
| **Audio** | Abtastrate: 48khz <br> Kanäle: Stereo <br> Desktopaudiogerät: Standard <br> Desktopaudiogerät 2: Deaktivieren <br> Mikrofon-/Hilfsaudiogerät: Standard |
| **Video** | Basisauflösung (Canvas): 1920 x 1080 <br> Ausgabeauflösung (skaliert): 1920 x 1080 <br> Downscale Filter: Bicubic (Schärfere Skalierung, 16 Beispiele) <br> Allgemeine FPS-Werte: 30 |
| **Tastenkürzel** | Behalten Sie die Standardeinstellung bei. |
| **Erweitert** | Prozesspriorität: Normal | <br>

<br>Wählen Sie jetzt Anwenden und dann **OK** aus, um alle OBS-Einstellungen zu speichern. 

1. Alt-Tab zu AltspaceVR, in den richtigen Raum/die richtige Welt/das richtige Ereignis zu kommen und ihre Kamera (d. h. Ihren Avatar) zu stellen, werden wir ein Video aufzeichnen!
2. Alt-Tab auf OBS um, und wenn Sie bereit sind, klicken Sie **auf Aufzeichnung starten.**

Unten rechts in OBS sehen Sie, dass REC: mit dem Aufzählen beginnt und der Punkt rot ist, was bedeutet, dass Sie aufzeichnen!

Führen Sie eine Testaufzeichnung aus: 
1. Öffnen/Schließen/Rollover der Menüs in AltspaceVR, um Benutzeroberflächenklänge zu erzeugen
2. Stellen Sie sicher, dass Sie unveränderlich sind, z. B. "Sibilance, Sibilance", oder lassen Sie einen anderen Benutzer auf einem normalen Volume mit Ihnen sprechen.
3. Sehen Sie sich die Desktopaudio- und Mikrofon-/Hilfsebenen an, um zu sehen, ob es funktioniert.

Wir stummschalten die Mikrofone bei der Aufzeichnung normalerweise. Wählen Sie anschließend das Lautsprechersymbol für Mic/Aux aus, und es wird rot mit einem X angezeigt.

* Es ist sehr schwierig, Ihre Audiodaten und die Audiodaten des anderen Benutzers zu finden, sodass das Mikrofon am besten stumm geschaltet wird, wenn Sie ein Ereignis aufzeichnen.
* Ein weiteres Problem bei Audiodaten ist die Art und Weise, wie OBS eingerichtet wird. Sie erfasst ALLE Audiodaten von Ihrem Computer. Wenn Sie YouTube also auf Ihrem PC ansehen, werden diese Audiodaten oder Benachrichtigungen von Diskotheken erfasst.
* Wenn Sie nur die Audiodaten von AltspaceVR aufzeichnen möchten, wechseln Sie in den Lautstärkemixer (klicken Sie mit der rechten Maustaste auf das Lautsprechersymbol unten rechts in Windows), und stummschalten Sie Systemklang, Browser und so weiter, aber stummschalten Sie OBS oder AltspaceVR nicht.

> [!IMPORTANT]
> Vergessen Sie nicht, diese Einstellungen für den Volumemixer nach der Aufzeichnung wieder zu aktivieren.

Navigieren Sie nun zurück zu OBS, und wählen **Sie Aufzeichnung** aus Datei beenden **>Aufzeichnungen anzeigen aus.** Dadurch wird der Ordner mit Ihren OBS-Videodateien geöffnet, und doppelklicken Sie auf das Testvideo.

Manchmal ist die Aufzeichnung recht laut, also senken Sie den Schieberegler für Desktopaudio, und erstellen Sie eine weitere Aufzeichnung zum Testen.


## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Livestreaming auf YouTube im AltspaceVR 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

AltspaceVR und OBS müssen installiert sein. Starten Sie AltspaceVR im 2D-Modus, starten Sie OBS, entweder Livestream, oder erstellen Sie ein "Neues Liveereignis" auf YouTube, richten Sie OBS mit Ihrem YouTube-Streamschlüssel ein, beginnen Sie mit dem Streamen in OBS, beginnen Sie mit dem Streaming auf YouTube, und Sie sind auf dem Weg zur Strömen!

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen **Sie Windows** aus, um OBS herunterzuladen (in diesem Beitrag wird OBS v22.0.2 verwendet).
3. Installieren von OBS

AltspaceVR im 2D-Modus ausführen lassen, BEVOR Sie OBS ausführen
1. Laden Sie AltspaceVR von unserer Website herunter: [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. Um sicherzustellen, dass Sie AltspaceVR im 2D-Modus starten, trennen Sie entweder das USB-Kabel Ihrer HMD von Ihrem PC, oder wenn Sie einen Rift haben: STRG+ALT+ENTF, Dienste, Oculus VR-Laufzeitdienst, klicken Sie mit der rechten Maustaste auf Beenden. Dadurch wird Oculus Home deaktiviert und AltspaceVR im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und starten Sie erneut, um den VR-Modus abzurufen.

3. Alt-Tab zu OBS

4. Wählen Sie unter Quellen die Option **+** aus, wählen Sie Game Capture, Create new (Spielerfassung), Create new (Neu erstellen), Edit text to "AltspaceVR Capture" (Text in AltspaceVR Capture bearbeiten), make source visible (Quelle sichtbar machen), OK aus.
5. Doppelklicken Sie auf AltspaceVR Capture.
6. Modus: Bestimmtes Fenster erfassen
7. Fenster: [AltspaceVR.exe]: AltspaceVR
8. Fensterübergleichspriorität: Übereinstimmungstitel, andernfalls Fenster derselben ausführbaren Datei suchen
9. Scrollen Sie nach unten zu Aufzeichnungscursor: Untick OK

Dadurch sollte AltspaceVR in OBS angezeigt werden. Sehr schön!

Wechselt nun in OBS zu Datei>Einstellungen:

| Registerkarte | Einstellungen |
|---|---|
| Allgemein | Automatische Aufzeichnung beim Streaming aktivieren (dadurch wird zusätzlich zum Livestreaming eine Videodatei auf Ihrem Computer aufgezeichnet) |
| STREAM | Streamtyp: Streamingdienste <br> Dienst: YouTube/YouTube Gaming (kann auch an Twitch, Mixer, Facebook Live usw. gestreamt werden))<br>Server: Primärer YouTube-Erfassungsserver <br>Streamschlüssel: Fügen Sie Ihren Streamschlüssel von YouTube ein. (Siehe "Einrichten von Livestreaming auf YouTube" weiter unten) |
| Ausgabe | Ausgabemodus: Wechseln Sie zu Erweitert. |
| Streaming | Audiospur 1 <br>Encoder: x264 <br>Erzwingen der Encodereinstellungen des Streamingdiensts: Tick <br>Neuskalierungsausgabe: nicht angezeigt <br>Ratensteuerung: CBR <br>Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br>Keyframeintervall = 2 <br>CPU-Auslastungsvoreinstellung = sehr schnell |
| Aufzeichnung | Typ: Standard <br>Aufzeichnungspfad: D:/Video (Navigieren Sie zu dem Ort, an dem die Videodatei gespeichert werden soll, wenn Sie zuvor "Beim Streaming automatisch aufzeichnen" ausgewählt haben) <br>Aufzeichnungsformat: mp4 (Wenn sie während der Aufzeichnung abstürzt, versuchen Sie hier flv anstelle von mp4, wenn Sie das Video abstürzt, kann es weiterhin mit flv verwendet werden. <br>Audiospur 1 <br>Encoder: Streamencoder verwenden |
| Audio | Audiobitrate: 160 (für alle Spuren) Abtastrate: 48 KHz <br>Kanäle: Stereo <br>Desktopaudiogerät: Standard <br>Desktopaudiogerät 2: Deaktivieren <br>Mic/Aux-Audiogerät: Standard |
| Wiedergabepuffer | Behalten Sie die Standardeinstellung bei. |
| Video | Basisauflösung (Canvas): 1920x1080 <br>Ausgabeauflösung (skaliert): 1920 x 1080 <br>Downscale-Filter: Bicubic (Schärfte Skalierung, 16 Beispiele) <br>Allgemeine FPS-Werte: 30 |
| Tastenkürzel | Behalten Sie die Standardeinstellung bei. |
| Fortgeschrittene | Prozesspriorität: Normal |
|||

<br>Achten Sie nun darauf, auf Übernehmen und dann auf OK zu klicken. Schließen Sie obs, und öffnen Sie obs erneut. Dadurch werden Ihre gesamten OBS-Einstellungen gespeichert. Gute :)

Im Abschnitt "Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC" weiter oben finden Sie Anweisungen zum Testen der Aufzeichnung mithilfe einer lokalen Aufzeichnung anstelle des Livestreams und zum Einrichten der Kameraaufnahme vor der Aufzeichnung.

Ein weiteres Problem bei Audiodaten ist die Einrichtung von OBS. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube ansehen, werden diese Audio- oder Teams-Nachrichten oder Benachrichtigungsgeräusche aufgezeichnet.

Um nur die Audiodaten von AltspaceVR aufzuzeichnen, wechseln Sie zu Volume Mixer (klicken Sie mit der rechten Maustaste auf das Lautsprechersymbol unten rechts unter Windows) und Stummschalten von Systemsounds, Browsern usw., aber stummschalten Sie OBS oder AltspaceVR nicht.

Vergessen Sie nicht, die Audiodaten nach der Aufzeichnung wieder zu aktivieren ;)

Herzlichen Glückwunsch, Sie sind ein AltspaceVR-Videorecorder!

## <a name="setting-up-live-streaming-on-youtube"></a>Einrichten von Livestreaming auf YouTube

Sie können entweder schnell einen Livestream in Betrieb nehmen (**Stream**) oder ein zukünftiges Livestreamereignis einrichten (**Verwalten**). Es kann empfohlen werden, dass Sie die Methode "Verwalten" einrichten.

1. Öffnen Sie Ihren Browser, melden Sie sich [https://www.youtube.com/](https://www.youtube.com/) an, und wechseln Sie dann zu . [https://www.youtube.com/my_live_events](https://www.youtube.com/my_live_events)
2. Klicken Sie oben rechts auf Ihr Kontosymbol, und wählen Sie in der Dropdownleiste Creator Studio aus.
3. LIVE STREAMING auf der linken Seite der Seite.

**'Stream** now'-Methode:

* Wählen Sie BEARBEITEN aus, um Ihre Livestreaminformationen einzugeben.<br>
* Behalten Sie unter Streameinstellungen die Standardwerte bei.<br>
* Streamschlüssel (In Encoder einfügen), "Reveal" auswählen und diesen Schlüssel kopieren, damit Sie ihn in OBS einfügen können<br>
* OBS/Settings/Stream öffnen<br>
* Fügen Sie den Streamschlüssel von YouTube in das Feld Stream Key in OBS ein.<br>
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
* Erstellen neuer oder wiederverwenden von Einstellungen, wenn Sie bereits einen vorherigen verwalteten Livestream eingerichtet haben
* Hinzufügen von Titel, Datum, Startzeit, Beschreibung, Miniaturansicht und Tags hochladen – Vergessen Sie nicht, altspaceVR :)
* Wählen Sie im Dropdownmenü Öffentlich aus (Standardeinstellung: "Nicht aufgeführt")
* Standardwerte verwenden
* Kopieren des Streamschlüssels (Einfügen in den Encoder)
* Um Ihre tatsächliche YouTube-Livestream-Videoseite anzuzeigen, müssen Sie oben rechts das Symbol FREIGEBEN auswählen. Dies ist Ihr YouTube-Livestream-Ereignislink, der auf Social Way vor Ihrem eigentlichen Ereignis freigegeben werden kann.
* Öffnen Sie nun OBS.
* Datei/Einstellungen
* STREAM
* Fügen Sie den kopierten Streamschlüssel in das Feld Streamschlüssel ein.
* Anwenden und dann OK
* Wählen Sie "Streaming starten" aus.
* Zurück zu YouTube sehen Sie, dass das Fenster "Vorschau" Ihren Stream zeigt und GO LIVE jetzt oben rechts angezeigt wird.
* Wählen Sie GO LIVE (LIVE) aus.
* Sie sind jetzt LIVE!
* Wechseln Sie zu Ihrer Browserregisterkarte, und öffnen Sie den Link "Auf Der Seite ansehen", um sicherzustellen, dass das Video gut aussieht. DENKEN SIE DARAN, dass Sie die Audiodaten nicht hören werden, da Sie Audiodaten aus Ihren Browsern deaktiviert haben, wenn Sie sie im Windows-Volumemixer stummgeschaltet haben. Überprüfen Sie die Audiodaten auf Ihrem Telefon, oder bitten Sie einen Freund, die Audiodaten für Sie zu überprüfen.
* Sieht gut aus!
* Alt-Tab zurück zu AltspaceVR, um Ihre Kamera (d. h. Ihren Avatar) in Ihrem Ereignis zu bewegen.
* Wenn Sie mit Ihrem Livestream fertig sind, wechseln Sie zurück zur YouTube-Seite "Live Control Room".
* Wählen Sie "Streaming beenden" aus.
* Das Dialogfeld wird geöffnet, in dem Sie gefragt werden, ob Sie das Liveereignis nicht mehr streamen möchten.
* Wechseln Sie zu OBS, und wählen Sie auch Streaming beenden aus.
* Congchef, Sie sind jetzt ein AltspaceVR-Streamer!

Für Bonuspunkte teilen Sie Ihre Videos in sozialen Medien mit der Welt, und markieren Sie @AltspaceVR uns :)