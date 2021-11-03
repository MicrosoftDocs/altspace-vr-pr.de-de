---
title: Aufzeichnung und Livestreaming
description: Erfahren Sie, wie Sie AltspaceVR-Ereignisse von Ihrem PC aufzeichnen und live streamen, um sie für Ihre Benutzer zu bewerben und freizugeben.
author: qianw211
ms.author: v-qianwen
ms.date: 11/1/2021
ms.topic: article
keywords: Streaming, Aufzeichnung, Video, Audio, Youtube, Obs, Live
ms.openlocfilehash: e82960097103df25c50f0b03b76d21e10b1cbbd6
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278978"
---
# <a name="recording-and-live-streaming"></a>Aufzeichnung und Livestreaming

Das Aufzeichnen und Livestreaming Ihrer AltspaceVR-Erfahrung, um anderen Personen auf der ganzen Welt zu zeigen, ist eine hervorragende Möglichkeit, Ihre Ereignisse, AltspaceVR und VR im Allgemeinen zu bewerben! Sehen Sie sich unten die ersten Schritte an.

In diesem Artikel lernen Sie Folgendes:

* [Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC](#recording-altspacevr-in-2d-mode-on-pc)
* [Livestream an YouTube in AltspaceVR im 2D-Modus auf dem PC](#live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc)

## <a name="recording-altspacevr-in-2d-mode-on-pc"></a>Aufzeichnen von AltspaceVR im 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

1. Haben Sie AltspaceVR und OBS (Open Zusender Software) installiert. Starten Sie AltspaceVR im 2D-Modus, starten Sie OBS, legen Sie OBS so fest, dass AltspaceVR erfasst und entfernt wird!

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

1. Besuchen Sie [https://obsproject.com/](https://obsproject.com/).
2. Wählen Sie **Windows** aus, um OBS herunterzuladen. In diesem Beitrag wird **OBS v26.1.1 verwendet.**
3. Installieren von OBS

### <a name="have-altspacevr-running-before-you-run-obs"></a>Führen Sie ALTSPACEVR AUS, BEVOR Sie OBS ausführen.

1. Laden Sie AltspaceVR von unserer Website herunter, und installieren Sie es: [altvr.com/get](https://altvr.com/getaltspacevr)
2. Wenn Sie Ihr VR-Video stabiler machen und ruckartige Kopfbewegungen beseitigen möchten, stellen Sie sicher, dass Sie entweder den 2D-Client verwenden oder AltspaceVR im 2D-Modus starten, indem Sie das USB-Kabel Ihres Headsets von Ihrem PC trennen. Wenn Sie einen Rift haben, drücken Sie STRG+ALT+ENTF, wählen Sie **Dienste**, **Oculus VR Runtime Service**, klicken Sie mit der rechten Maustaste, und wählen Sie **Beenden** aus. Dadurch wird Oculus deaktiviert und AltspaceVR im 2D-Modus gestartet. Wiederholen Sie diese Schritte, und verwenden Sie Start, um den VR-Modus wieder abzurufen.
3. Sie können Ihre Erfahrung auch im VR-Modus aufzeichnen, indem Sie Game Capture mit OBS verwenden.

Jetzt Alt-Tab zu OBS:

1. Wählen Sie unter **Szenen** die neue Szene aus, **+** und benennen Sie sie.
2. Wählen Sie als **Nächstes** unter Quellen folgende Option aus: **+ > Game Capture > Neu erstellen.**
2. Text in "AltspaceVR Capture" bearbeiten, **Quelle sichtbar machen** aktivieren und **OK** auswählen
3. Doppelklicken Sie unter **Quellen** auf **AltspaceVR Capture.**
4. Ändern des **Modus** in **Bestimmtes Fenster erfassen**
5. Fenster: [AltspaceVR.exe]: AltspaceVR
6. Fensterübertrefferpriorität: Übereinstimmungstitel, andernfalls Fenster derselben ausführbaren Datei suchen
7. Scrollen Sie nach unten zu **Capture Cursor**: untick
8. Wählen Sie **OK** aus.
9. Dadurch sollte AltspaceVR in OBS angezeigt werden.

Um nun die folgenden Eigenschaften in OBS festzulegen, wechseln Sie zu **Datei > Einstellungen**:

|Registerkarte|Einstellungen|
|---|---|
| **Allgemein** | Behalten Sie die Standardeinstellung bei. |
| **Stream** | Behalten Sie die Standardeinstellung bei. |
| **Ausgabe** | Wechseln Sie zu Erweitert. |
| **Registerkarte "-Streaming"** | Audiospur 1 <br> Encoder: x264 <br> Neuskalierungsausgabe: nicht angezeigt <br> Ratensteuerung: CBR <br> Bitrate: 6000 (6000 für 30 fps oder 9000 für 60 fps) <br> Keyframeintervall = 2 <br> CPU-Auslastungsvoreinstellung = sehr schnell |
| **Registerkarte "-Recording"** | Typ: Standard <br> Aufzeichnungspfad: D:/Video (Navigieren Sie zu dem Ort, an dem die Videodateien gespeichert werden sollen) <br> Aufzeichnungsformat: mp4 (Wenn während der Aufzeichnung abstürzen, versuchen Sie hier flv anstelle von mp4. Wenn Sie abstürzen, kann das Video weiterhin mit flv verwendet werden.) <br> Audiospur 1 <br> Encoder: Streamencoder verwenden |
| **Registerkarte "-Audio"** | Audiobitrate: 160 (für alle Spuren) |
| **-Replay buffer (Registerkarte "Puffer wiedergeben" )** | Behalten Sie die Standardeinstellung bei. |
| **Audio** | Abtastrate: 44,1 KHz <br> Kanäle: Stereo <br> Desktopaudio: Standard <br> DesktopAudio 2: Deaktivieren <br> Mic/Aux Audio: Standard |
| **Video** | Basisauflösung (Canvas): 1920x1080 <br> Ausgabeauflösung (skaliert): 1920x1080 <br> Downscale-Filter: Bicubic (Schärfte Skalierung, 16 Beispiele) <br> Allgemeine FPS-Werte: 30 (oder 60) |
| **Tastenkürzel** | Behalten Sie die Standardeinstellung bei. |
| **Erweitert** | Prozesspriorität: Normal | <br>

<br>Stellen Sie nun sicher, dass **Sie Übernehmen** und dann **OK** auswählen, um alle OBS-Einstellungen zu speichern. 

1. Alt-Tab zu AltspaceVR, steigen Sie in den richtigen Raum/die richtige Welt/das richtige Ereignis ein, und richten Sie Ihre Kamera (also Ihren Avatar) ein, um ein Video aufzuzeichnen!
2. Alt-Tab zu OBS über, und wenn Sie bereit sind, klicken Sie auf **Aufzeichnung starten.**

Am unteren rechten Rand von OBS sehen Sie, dass **REC:** beginnt zu zählen, und der Punkt ist rot, was bedeutet, dass Sie aufzeichnen!

Erstellen Sie aus diesem Grund eine Testaufzeichnung: 
1. Öffnen/Schließen/Rollover der Menüs in AltspaceVR, um Benutzeroberflächensounds zu erzeugen
2. Stellen Sie sicher, dass Sie unveränderlich sind, z. B. "Sibilance, Sibilance", oder lassen Sie einen anderen Benutzer mit einem normalen Volume sprechen.
3. Sehen Sie sich die **Desktopaudio-** und **Mic/Aux-Ebenen** an, um zu sehen, ob die Audiodaten richtig aufgenommen werden.

In der Regel stummschalten wir mic/Aux bei der Aufzeichnung. Wählen Sie das Lautsprechersymbol für Mic/Aux aus, und es wird rot mit einem X angezeigt.

* Es ist sehr schwierig, ihre Mikrofonaudioebenen mit den Audiodaten des anderen Benutzers abzugleichen, sodass das Mikrofon am besten stummgeschaltet wird, wenn Sie ein Ereignis aufzeichnen.
* Ein weiteres Problem bei Audiodaten ist die Einrichtung von OBS. Es erfasst alle Audiodaten von Ihrem Computer. Wenn Sie also YouTube ansehen oder Benachrichtigungssounds auf Ihrem PC erhalten, werden diese Audiodaten aufgezeichnet.
* Um nur die Audiodaten von AltspaceVR aufzuzeichnen, wechseln Sie zu **Open Volume Mixer** (klicken Sie mit der rechten Maustaste auf das Lautsprechersymbol unten rechts neben Windows), und stummschalten Sie Systemsounds, Browser usw., aber stummschalten Sie OBS oder AltspaceVR nicht.

> [WICHTIG] Vergessen Sie nicht, diese Einstellungen für den Volumemixer nach der Aufzeichnung zu ändern.

Navigieren Sie nun zurück zu OBS, und wählen **Sie Aufzeichnung beenden** aus. Um das soeben aufgezeichnete Video zu finden, wechseln Sie zu **Datei>Aufzeichnungen anzeigen**. Dadurch wird der Ordner mit Ihren OBS-Videodateien geöffnet, und doppelklicken Sie auf das Testvideo.

Manchmal ist die Aufzeichnung ziemlich laut, also setzen Sie den Schieberegler für Desktopaudio in OBS herunter, und nehmen Sie eine weitere Aufzeichnung zum Testen vor.

Pro-tip: Verwenden Sie STRG+ALT+P, um im Fotomodus umzuschalten. Dadurch wird die Benutzeroberfläche aus Ihrer Ansicht entfernt, um einen ansprechenden Cleanshot zu erhalten.

Herzlichen Glückwunsch, Sie sind ein AltspaceVR-Videorecorder!

## <a name="live-streaming-to-youtube-in-altspacevr-2d-mode-on-pc"></a>Livestreaming auf YouTube im AltspaceVR 2D-Modus auf dem PC

### <a name="the-short-version"></a>Die Kurzversion

AltspaceVR und OBS müssen installiert sein. Starten Sie AltspaceVR und OBS. Sie können entweder den Livestream "Right Now" oder "Later date" (Später) streamen. Richten Sie OBS auf YouTube mit Ihrem YouTube-Streamschlüssel ein. Beginnen Sie mit dem Streamen in OBS und auf YouTube, und Sie sind auf dem Weg zu den Strömen!

### <a name="the-slightly-longer-version"></a>Die etwas längere Version

Im Abschnitt [Recording AltspaceVR in 2D mode on PC](#recording-altspacevr-in-2d-mode-on-pc) (Aufzeichnung von AltspaceVR im 2D-Modus auf dem PC) oben auf dieser Seite finden Sie Anweisungen zum Testen der Aufzeichnung mithilfe einer lokalen Aufzeichnung anstelle des Livestreams und zum Einrichten Ihres Kamerabilds.

## <a name="setting-up-live-streaming-on-youtube"></a>Einrichten von Livestreaming auf YouTube

Sie können entweder einen Livestream "Right Now" erhalten oder einen zukünftigen Livestream mit "Later date" einrichten.

1. Öffnen Sie Ihren Browser, melden Sie sich [https://www.youtube.com/](https://www.youtube.com/) an, und wechseln Sie dann zu . [https://studio.youtube.com/](https://studio.youtube.com/)
2. Suchen Sie nach oben rechts, und wählen Sie **CREATE** und dann **Go live (Live) aus.**

**"Right now"-Methode:**

1. Wählen **Sie Jetzt starten aus.**
1. Auswählen **von Streamingsoftware/GO**
1. Klicken **Sie oben** rechts auf BEARBEITEN, um Ihre Videodetails und Anpassungen zu bearbeiten.
1. Behalten **Sie unter Stream Einstellungen** die Standardwerte bei.
1. Kopieren Sie den Schlüssel neben  Stream key (paste in encoder) (Streamschlüssel **(in Encoder einfügen)),** damit Sie ihn in OBS einfügen können.
1. ÖFFNEN VON **OBS/Einstellungen**  /  **Stream**
1. Wählen Sie **im Dropdownmenü** Dienst die Option **YouTube – RTMPS aus.**
1. Fügen Sie den Streamschlüssel von YouTube in das **Feld StreamSchlüssel** in OBS ein.
1. Klicken **Sie auf Übernehmen** und dann auf **OK.**
1. Wählen Sie **Streaming in** OBS starten aus.
1. Wechseln Sie zu YouTube, und Sie werden sehen, dass Sie jetzt live auf YouTube sind!
1. Um Ihre tatsächliche YouTube-Livestream-Videoseite anzuzeigen, müssen Sie oben rechts das Symbol FREIGEBEN auswählen.
1. Klicken Sie auf den Link "Video", um Ihren YouTube-Livestream zu sehen und zu hören. 
1. Diese URL ist Ihr Livestreamlink und kann für alle Kanäle in sozialen Netzwerken freigegeben :)
1. Um den Livestream zu beenden, wählen Sie END STREAM auf YouTube und dann Stop Streaming on OBS (Streaming bei OBS beenden) aus.

Methode **"Späteres** Datum":
1. Klicken Sie oben links auf das **Symbol Verwalten.**
1. Wählen Sie **SCHEDULE STREAM** oben rechts aus.
1. Hinzufügen von Titel, Beschreibung, Kategorie, Miniaturansicht (1280 x 720) und dann **WEITER**
1. Livechatoptionen und dann **WEITER**
1. Privat, Nicht aufgelistet oder Öffentlich (wählen Sie Öffentlich)
1. Planen Sie das Datum und die Uhrzeit, zu der Sie live gehen möchten, und dann **FERTIG.**

 **Wenn Sie bereit sind, Ihren Livestream in der Zukunft zu starten:**
1. Behalten Sie unter Stream Einstellungen die Standardwerte bei.
1. Kopieren Sie den Schlüssel neben  Stream key (paste in encoder) (Streamschlüssel **(in Encoder einfügen)),** damit Sie ihn in OBS einfügen können.
1. ÖFFNEN VON **OBS/Einstellungen**  /  **Stream**
* Wählen Sie **im Dropdownmenü** Dienst die Option **YouTube – RTMPS aus.**
1. Fügen Sie den Streamschlüssel von YouTube in das **Feld StreamSchlüssel** in OBS ein.
1. Klicken **Sie auf Übernehmen** und dann auf **OK.**
1. Wählen Sie **Streaming in** OBS starten aus.
1. Wechseln Sie zu YouTube, und Sie werden sehen, dass Sie jetzt live auf YouTube sind!
1. Um Ihre tatsächliche YouTube-Livestream-Videoseite anzuzeigen, müssen Sie oben rechts das Symbol FREIGEBEN auswählen.
1. Klicken Sie auf den Link "Video", um Ihren YouTube-Livestream zu sehen und zu hören. 
1. Diese URL ist Ihr Livestreamlink und kann für alle Kanäle in sozialen Netzwerken freigegeben :)
1. Um den Livestream zu beenden, wählen Sie **END STREAM** auf YouTube und dann Stop Streaming on OBS **(Streaming bei** OBS beenden) aus.

Um Bonuspunkte zu erhalten, teilen Sie Ihre Videos in sozialen Netzwerken mit, und markieren Sie @AltspaceVR uns :)