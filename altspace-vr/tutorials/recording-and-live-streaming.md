---
title: Aufzeichnen und Live Streaming
description: Erfahren Sie, wie Sie Ihre altspacevr-Ereignisse von Ihrem PC aufzeichnen und streamen, um Sie für Ihre Benutzer zu bewerben und freizugeben.
ms.date: 02/10/2021
ms.topic: article
keywords: Streaming, Aufzeichnung
ms.openlocfilehash: 80d54407915af1a0d4b7783858446f54205e6a2a
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213502"
---
# <a name="recording-and-live-streaming"></a>Aufzeichnen und Live Streaming

Das Aufzeichnen und Live Streaming ihrer altspacevr-Umgebung, um andere Personen auf der ganzen Welt anzuzeigen, ist eine großartige Möglichkeit, Ihre Veranstaltung, altspacevr und VR im Allgemeinen zu bewerben! Sehen Sie sich die folgenden Informationen an, um zu beginnen:

In diesem Artikel lernen Sie Folgendes:

* [Aufzeichnen von altspacevr im 2D-Modus auf dem PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Live Streaming von Stream auf YouTube in altspacevr im 2D-Modus auf dem PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Aufzeichnen von altspacevr im 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

Sie haben altspacevr und OBS installiert. Starten Sie altspacevr im 2D-Modus, starten Sie obs, und legen Sie für "obs" den Wert für "altspacevr" und den Datensatz

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen Sie **Windows** zum Herunterladen von OBS aus. Dieser Beitrag verwendet **obs v 22.0.2**
3. Installieren von obs

### <a name="have-altspacevr-running-in-2d-mode-before-you-run-obs"></a>Ausführen von "altspacevr" im 2D-Modus vor der Ausführung von obs

1. Laden Sie altspacevr von unserer Website herunter, und installieren Sie es: [altvr.com/Get](https://altvr.com/getaltspacevr)
2. Stellen Sie sicher, dass Sie altspacevr im 2D-Modus starten, indem Sie das USB-Kabel Ihres HMD von Ihrem PC aufheben, oder wenn Sie über einen Riss verfügen: STRG + ALT + ENTF, Dienste, oculus VR-Lauf Zeit Dienst, klicken Sie mit der rechten Maustaste, und klicken Sie 
    * Dadurch wird Oculus deaktiviert und altspacevr im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und verwenden Sie "Start", um den VR-Modus wieder zurück

Jetzt Alt-Tab zu obs:

1. Wählen Sie unter Quellen die Option **+ > Spiele Erfassung > neu erstellen** aus.
2. Text in ' altspacevr Capture ' bearbeiten, Tick- **Quelle sichtbar machen** und OK auswählen
3. Doppelklicken Sie auf " **altspacevr Capture** " unter Quellen.
4. **Modus** ändern, um **bestimmtes Fenster zu erfassen**
5. Fenster: [AltspaceVR.exe]: altspacevr
6. Fenster Übereinstimmungs Priorität: übereinstimmende Titel, andernfalls Fenster der gleichen ausführbaren Datei suchen
7. Scrollen Sie nach unten zum Erfassungs Cursor: untick OK

Dadurch sollte altspacevr in obs angezeigt werden. Wechseln Sie nun zu **Datei > Einstellungen**, um die folgenden Eigenschaften in obs festzulegen:

| Registerkarte | Einstellungen |
|---|---|
| Allgemein | Behalten Sie die Standardeinstellung bei. |
| Datenstrom | Behalten Sie die Standardeinstellung bei. |
| Ausgabemodus: zu erweitert wechseln | Streaming-Registerkarte <br> Audiospur 1 <br> Encoder: x264 <br> Streaming Service Encoder-Einstellungen erzwingen: Tick <br> Ausgabe neu skalieren: nicht getickt <br> Raten Steuerung: CBR <br> Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br> Keyframe-Intervall = 2 <br> Voreinstellung für CPU-Auslastung = veryfast |
| Aufzeichnung | Typ: Standard <br> Aufzeichnungs Pfad: D:/Video (navigieren Sie zu dem Ort, an dem die Video Datei gespeichert werden soll) <br> Aufzeichnungs Format: MP4 (wenn beim Aufzeichnen ein Absturz aufgetreten ist, versuchen Sie hier hier nicht mit der MP4-Datei, wenn Sie abstürzen. <br> Audiospur 1 <br> Encoder: Stream Encoder verwenden |
| Audio | Audiobitrate: 160 (für alle Spuren) |
| Wiedergabe Puffer | Behalten Sie die Standardeinstellung bei. |
| Audio | Abtast Rate: 48kHz <br> Kanäle: Stereo <br> Desktopaudiogerät: Standard <br> Desktop Audiogerät 2: Deaktivieren <br> MIC/aux-Audiogerät: Standard |
| Video | Basis-(Canvas) Auflösung: 1920 × 1080 <br> Ausgabeauflösung (skaliert): 1920 × 1080 <br> Downscale-Filter: Bikubisch (verstärkte Skalierung, 16 Stichproben) <br> Allgemeine FPS-Werte: 30 |
| Hotkeys | Behalten Sie die Standardeinstellung bei. |
| Erweitert | Prozesspriorität: normal |

OK, wählen Sie jetzt **anwenden** aus, und klicken Sie dann auf **OK** , um alle ihre obs-Einstellungen zu speichern. 

1. Alt-Tab zu altspacevr, machen Sie sich mit dem richtigen Raum bzw. der richtigen Welt/dem aktuellen Ereignis vertraut, und halten Sie Ihre Kamera (d. h. Ihren Avatar) an einem Video.
2. Alt-Tab auf "obs", und wenn Sie bereit sind, klicken Sie auf **Aufzeichnung starten**.

Sie sehen unten rechts von OBS, dass REC: beginnt, die Zählung durchführt, was bedeutet, dass Sie aufzeichnen!

Erstellen Sie Folgendes: 
1. In altspacevr öffnen/schließen/Rollover die Menüs zum Erstellen von Benutzeroberflächen Sounds
2. Sagen Sie "sibilance, sibilance", und holen Sie sich einen weiteren Benutzer, der auf einem normalen Volume mit Ihnen spricht, oder sehen Sie sich ein Video auf der 2D-Anzeige an.
3. Sehen Sie sich die Desktop-Audiofunktionen und die MIC/aux-Ebenen an, um zu sehen, ob Ihre Arbeit funktioniert.

Bei der Aufzeichnung werden die MIC/aux in der Regel stumm geschaltet. Wählen Sie das Redner Symbol für MIC/aux aus, und es wird mit einem X rot angezeigt.

* Es ist sehr schwierig, ihre Audiodaten und die Audiodaten des anderen Benutzers abzugleichen, damit das MIC-Format am besten stumm geschaltet wird.
* Ein weiteres Problem bei der Audioinstallation ist die Einrichtung von obs. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube ansehen, werden diese Audiodaten, Slack-Nachrichten oder Benachrichtigungs Geräusche aufgezeichnet.
* Wenn Sie nur die Audiodaten aus altspacevr aufzeichnen möchten, können Sie den volumemixer aufrufen (Klicken Sie mit der rechten Maustaste auf das Redner Symbol unten rechts in Windows), und stumm schalten Sie System Sounds, Browser usw., aber nicht "obs" oder "altspacevr" stumm schalten.

> [!IMPORTANT]
> Vergessen Sie nicht, diese volumemixer-Einstellungen nach der Aufzeichnung wieder zu aktivieren.

Navigieren Sie nun zurück zu obs, und wählen Sie **Aufzeichnung** aus **Datei>Aufzeichnung anzeigen** aus. Dadurch wird der Ordner mit ihren obs-Videodateien geöffnet. Doppelklicken Sie auf das Testvideo.

Manchmal ist die Aufzeichnung sehr laut, sodass Sie den Schieberegler für die Desktop-Audiodaten verringern und eine weitere Aufzeichnung testen können.

<!-- Missing image -->

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Live Streaming auf YouTube im altspacevr 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

Sie haben altspacevr und OBS installiert. Starten Sie "altspacevr" im 2D-Modus, starten Sie "obs", entweder Live Stream, oder erstellen Sie ein "Neues Live-Ereignis" auf YouTube, richten Sie obs mit Ihrem YouTube-streamschlüssel ein, beginnen Sie mit dem Streaming in obs, starten Sie das Streaming auf YouTube.

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Klicken Sie auf **Windows** , um obs herunterzuladen (dieser Beitrag verwendet obs v 22.0.2).
3. Installieren von obs

Ausführen von "altspacevr" im 2D-Modus vor der Ausführung von obs
1. Laden Sie altspacevr von unserer Website herunter: [https://account.altvr.com/downloads](https://account.altvr.com/downloads)
2. Um sicherzustellen, dass Sie altspacevr im 2D-Modus starten, müssen Sie entweder das USB-Kabel Ihres HMD von Ihrem PC entfernen, oder wenn Sie über einen Riss verfügen: STRG + ALT + ENTF, Dienste, oculus VR Runtime Service, klicken Sie mit der rechten Maustaste, und klicken Sie auf Dadurch wird Oculus Home deaktiviert und altspacevr im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und starten Sie den VR-Modus erneut.

Alt-Tab zu obs

1. Wählen Sie unter Quellen die Option **+** , wählen Sie Spiel Erfassung, neu erstellen, Text in "altspacevr Capture", Teil Strich Quelle sichtbar, OK aus.
2. Doppelklicken Sie auf altspacevr Capture.
3. Modus: bestimmtes Fenster erfassen
4. Fenster: [AltspaceVR.exe]: altspacevr
5. Fenster Übereinstimmungs Priorität: übereinstimmende Titel, andernfalls Fenster der gleichen ausführbaren Datei suchen
6. Scrollen Sie nach unten zum Erfassungs Cursor: untick OK

Dadurch sollte altspacevr in obs angezeigt werden. Sehr schön!

In obs wechselt nun zu Datei>Einstellungen.

| Registerkarte | Einstellungen |
|---|---|
| Allgemein | Tick beim Streaming automatisch aufzeichnen (Dadurch wird neben Live Streaming eine Videodatei auf Ihrem Computer aufgezeichnet) |
| Datenstrom | Streamtyp: Streamingdienste <br> Dienst: YouTube/YouTube Gaming (kann auch an Twitch, Mixer, Facebook Live usw. gestreamt werden)<br>Server: primärer YouTube-Erfassungs Server <br>Stream Key: Fügen Sie Ihren streamschlüssel aus YouTube * * _ ein (siehe "Einrichten von Live <br>Streaming auf YouTube "unten) |
| Ausgabe | Ausgabemodus: zu erweitert wechseln |
| Streaming | Audiospur 1 <br>Encoder: x264 <br>Tick-streamingdienstencodereinstellungen erzwingen <br>Ausgabe neu skalieren: nicht getickt <br>Raten Steuerung: CBR <br>Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br>Keyframe-Intervall = 2 <br>Voreinstellung für CPU-Auslastung = veryfast |
| Aufzeichnung | Typ: Standard <br>Aufzeichnungs Pfad: D:/Video (navigieren Sie zu dem Speicherort, an dem die Video Datei gespeichert ist, wenn Sie zuvor "automatisch aufzeichnen" beim Streaming ausgewählt haben). <br>Aufzeichnungs Format: MP4 (wenn beim Aufzeichnen ein Absturz aufgetreten ist, versuchen Sie hier hier nicht mit der MP4-Datei, wenn Sie abstürzen. <br>Audiospur 1 <br>Encoder: Stream Encoder verwenden |
| Audio | Audiobitrate: 160 (für alle Spuren) Sample Rate: 48kHz <br>Kanäle: Stereo <br>Desktopaudiogerät: Standard <br>Desktop Audiogerät 2: Deaktivieren <br>MIC/aux-Audiogerät: Standard |
| Wiedergabe Puffer | Behalten Sie die Standardeinstellung bei. |
| Video | Basis-(Canvas) Auflösung: 1920 × 1080 <br>Ausgabeauflösung (skaliert): 1920 × 1080 <br>Downscale-Filter: Bikubisch (verstärkte Skalierung, 16 Stichproben) <br>Allgemeine FPS-Werte: 30 |
| Hotkeys | Behalten Sie die Standardeinstellung bei. |
| Erweitert | Prozesspriorität: normal |

OK, klicken Sie jetzt auf anwenden, dann auf OK und dann auf Schließen und erneut öffnen. Dadurch werden alle ihre obs-Einstellungen gespeichert. Gute:)

Anweisungen zum Testen der Aufzeichnung mithilfe einer lokalen Aufzeichnung anstelle des Livestreams finden Sie im Abschnitt "Aufzeichnen von altspacevr im 2D-Modus auf dem PC". Außerdem wird erläutert, wie Sie die Kamera vor der Aufzeichnung vor der Aufzeichnung einrichten.

Ein weiteres Problem bei der Audioinstallation ist die Einrichtung von obs. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube ansehen, werden diese Audionachrichten oder Team Nachrichten oder Benachrichtigungs Geräusche aufgezeichnet.

Wenn Sie nur die Audiodaten aus altspacevr aufzeichnen möchten, können Sie den volumemixer aufrufen (Klicken Sie mit der rechten Maustaste auf das Redner Symbol unten rechts in Windows), und stumm schalten Sie System Sounds, Browser usw., aber nicht "obs" oder "altspacevr" stumm schalten.

Vergessen Sie nicht, diese nach dem Aufzeichnen wieder einzuschalten;)

### <a name="setting-up-live-streaming-on-youtube"></a>Einrichten von Live Streaming auf YouTube

Sie können entweder einen Live-Stream (Live Streaming) direkt aufrufen oder ein zukünftiges Live-streamereignis einrichten (neues Live Ereignis). Ich kann vorschlagen, dass Sie die "neue Live Veranstaltung"-Methode einrichten.

1. Öffnen Sie Ihren Browser, und melden Sie sich an [https://www.youtube.com/](https://www.youtube.com/)
2. Wählen Sie auf Ihrem Konto Symbol, oben rechts, Creator Studio aus der Dropdown-Dropdown-Option aus.
3. Live Streaming auf der linken Seite der Seite.

"Stream Now"-Methode ändern Sie die Miniaturansicht, wenn Sie die URL des grundlegenden Info-Encoders für die Server-URL als standardmäßigen _ * *-Streamnamen/-Schlüssel ändern müssen, klicken Sie auf "anzeigen", und kopieren Sie diesen Schlüssel.
Um Ihre tatsächliche YouTube-Live Stream-Videoseite anzuzeigen, müssen Sie einen Bildlauf nach unten durchführen und unten rechts für den Link freigeben suchen.
Kopieren Sie diese Datei, und fügen Sie Sie in eine neue Browser Registerkarte ein, und klicken Sie dann auf Videos. in der Liste, in der Sie Ihr Video sehen, wird jetzt Live angezeigt.
Diese URL ist Ihr Live Datenstrom Link und kann für alle sozialen Netzwerke freigegeben werden:) Wenn Sie den Livestream beenden möchten, klicken Sie auf "Streaming beenden" auf "obs". Dadurch wird der Livestream auf YouTube beendet.

' Events '-Methode: https://www.youtube.com/my_live_events Klicken Sie auf ' New Live Event ' Titel hinzufügen, Datum, Startzeit, Beschreibung und Tags – vergessen Sie nicht, altspacevr zu markieren:) Wählen Sie im Dropdown Menü den Typ Public aus: Benutzer definiert klicken Sie auf "Ereignis erstellen", wenn Sie eine benutzerdefinierte Miniaturansicht hinzufügen möchten, klicken Sie auf Durchsuchen, und laden Sie das Bild (1280X720 funktioniert am besten) Select: Single-Use Stream Key Select your Encoder: Other Encoder Copy Stream Name (Stream Key)

Klicken Sie nun mit der rechten Maustaste auf die Seite "View on Watch", und öffnen Sie den Link in der neuen Registerkarte.

Dies ist Ihr YouTube Live Stream-Ereignis Link, der auf soziale Weise vor ihrer eigentlichen Veranstaltung freigegeben werden kann.

Öffnen Sie nun die Datei "obs File>Settings Stream", und fügen Sie den Stream-Schlüssel, den Sie gerade kopiert haben, in das Feld "Stream Key" ein. Klicken Sie anschließend auf "OK", "Änderungen speichern". Klicken Sie mit der rechten Maustaste auf "Live Control Room", und klicken Sie auf "Link in neuer Registerkarte öffnen" zurück Sie sehen, dass die Schaltfläche "Vorschau" nun blau ist. Klicken Sie auf die Schaltfläche "Vorschau", um zu sehen, ob Sie das Live Ereignis anzeigen möchten, und klicken Sie dann auf die Schaltfläche "Streaming starten". Klicken Sie auf das Dialogfeld "Streaming starten", um zu Fragen, ob Sie das Live Ereignis streamen möchten.

Sie sind jetzt Live!

Navigieren Sie zur Registerkarte Browser, und klicken Sie auf den Link "View on Watch Page", um sicherzustellen, dass das Video gut aussieht. Denken Sie daran, dass Sie das Audiogerät nicht hören, weil Sie die Audiodaten aus ihren Browsern ausgeschaltet haben, als Sie Sie in Windows Volume Mixer mutiert haben Überprüfen Sie die Audiodaten auf Ihrem Telefon, oder bitten Sie einen Freund, das Audiomaterial zu überprüfen.

Wir sehen gut aus!

Alt-Tab zurück zu altspacevr, um Ihre Kamera (also Ihren Avatar) in Ihrem Ereignis zu verschieben.

Wenn Sie mit Ihrem Livestream fertig sind, kehren Sie zur Seite "Live Control Room" von YouTube zurück.

Klicken Sie auf "Streaming Abbrechen".

Öffnet das Dialog Feld, in dem Sie gefragt werden, ob Sie das Streaming des Live Ereignisses abbrechen möchten. OK

Wechseln Sie zu obs, und klicken Sie auch auf Streaming abbrechen.

Herzlichen Glückwunsch, Sie sind jetzt ein altspacevr-Streamer!


Recording_AltspaceVR_.png


Für Bonuspunkte teilen Sie Ihre Videos auf der ganzen Welt auf sozialen Medien auf, und stellen Sie sicher, dass wir uns @AltspaceVR :)