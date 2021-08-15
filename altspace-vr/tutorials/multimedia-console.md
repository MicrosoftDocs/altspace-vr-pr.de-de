---
title: Verwenden der Multimediakonsole
description: Erfahren Sie, wie Sie mit dem Konfigurieren, Veröffentlichen und Steuern der Multimediakonsole in Ihren AltspaceVR-Funktionen beginnen.
ms.date: 03/11/2021
ms.topic: article
keywords: Konsole, Multimedia
ms.openlocfilehash: a24b3700f1687aed6bc00fd218aacd7cc12908e521af6239fac0ae97f48b4b9a
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127367"
---
# <a name="using-the-multimedia-console"></a>Verwenden der Multimediakonsole

Die Multimedia-Konsole ist ein Tool, das die Medienfreigabe in Ereignissen und Welten ermöglicht. Sie können es verwenden, um Dinge wie Bilder, Präsentationsfolien, Livestreams, Videos, Wiedergabelisten und mehr zu teilen. Im Folgenden finden Sie eine Schritt-für-Schritt-Anleitung zur Verwendung der Multimedia-Konsole **v0.5.0+**. 

## <a name="getting-started"></a>Erste Schritte

Die ersten Schritte mit der Multimedia-Konsole sind ein zweiteiler Prozess.  Zuerst gibt es das Webportal, mit dem Sie eine Konfiguration für die Multimedia-Konsolensitzung generieren und veröffentlichen, die Sie in Ihrer Umgebung platzieren.  Die zweite ist die Platzierung der tatsächlichen Multimedia-Konsolen-App in Ihrer Umgebung und das Festlegen des Konfigurationscodes, den sie verwenden soll.

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Konfigurieren der Multimedia-Konsole mit dem Webportal

1. Zunächst müssen Sie sicherstellen, dass Ihre Inhalte online gehostet werden, da Sie eine URL benötigen. (Sie können Fotos in die altvr.com hochladen, eine Videodatei .mp4 online hosten oder einen Dlive-Livestreamlink verwenden: https://dlive.tv/yourlivestream) 
2. Navigieren Sie unter zum Webportal für die Multimediakonsole. [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. Über das Webportal können Sie eine Konfiguration für die Multimedia-Konsole generieren und veröffentlichen.  (Weitere Informationen zu den verschiedenen Eigenschaften finden Sie weiter unten.)
4. Nachdem Sie die Medien in die Medienliste eingegeben und die allgemeinen Einstellungen konfiguriert haben, wählen Sie oben rechts in der App die Schaltfläche Veröffentlichen aus.
5. Nachdem die Veröffentlichung abgeschlossen ist, wird ein Dialogfeld mit einem Zwei-Wort-Code angezeigt, den Sie in die von Ihnen platzierte Multimedia-Konsole eingeben können.
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>Platzieren der Multimedia-Konsole in Ihrer Umgebung

1. Wählen Sie in der Multimedia-Konsole > Editor-Bereich für > **SDK-Apps > Aus.** (Wechseln Sie nicht zu **World Editor > Basics > SDK-App**– das ist für nicht registrierte Apps.)  
2. Positionieren Sie die Multimedia-Konsole so, dass sie Ihren Bereich und Ihre Zielgruppe am besten geeignet ist.
3. Wechseln Sie aus dem Bearbeitungsmodus, indem Sie auf die orangefarbene Schaltfläche Bearbeitungsmodus klicken.
4. Sie werden gefragt, **ob Sie der Media Player-Besitzer sind?** Wenn Sie die Person sind, die der offizielle Besitzer dieser Multimedia-Konsolensitzung sein sollte, bestätigen Und fahren Sie fort. (Es sind auch andere Rollen mit Berechtigungen verfügbar. Eine ausführliche Liste finden Sie weiter unten.)
5. Wählen Sie Ja aus, um zu bestätigen, dass Sie der primäre Host sind.  
6. Es sollte ein Dialogfeld angezeigt werden, in dem Sie aufgefordert werden, einen Code aus dem Webportal oder einen gültigen JSON-Code ein.  Geben Sie den zwei Wortcode aus dem Webportal ein, einschließlich des Bindestrichs, und klicken Sie auf OK. (JSON ist eine erweiterte Konfiguration, die unten beschrieben wird.)
7. Die Multimedia-Konsole sollte nach einigen Sekunden mit der Konfiguration geladen werden, die Sie im Webportal erstellt haben.

### <a name="controlling-the-multimedia-console"></a>Steuern der Multimedia-Konsole

1. Nachdem Sie Ihren Code eingegeben und den Konfigurationsprozess abgeschlossen haben, werden Unterhalb einer Medienanzeige Steuerschaltflächen angezeigt. 
    * **Wiedergabe** startet den Medien-Viewer (oder startet beim aktuellen Eintrag neu, wenn er zuvor beendet wurde). 
    * **Beenden** beendet den Medien-Viewer und blendet aktuelle Medien aus.  
    * Next/Prev skips to next or previous media **(Nächster/vorheriger** Datenträger wird mit dem nächsten oder vorherigen Medium übersprungen) 
    * **x/x**   zeigt den aktuellen Index in der Medienliste an und ermöglicht es Ihnen, zu einem beliebigen Punkt in der Liste zu springen.
    * **Die Konfiguration** ermöglicht das erneute Eingeben eines neuen Codes aus dem Webportal, um eine neue Konfiguration in der Konsole festlegen zu können. 

Jetzt können Sie mit der Freigabe über die Multimedia-Konsole beginnen.  
 
## <a name="working-with-the-web-portal"></a>Arbeiten mit dem Webportal

Das Webportal ist eine Web-App, mit der die verschiedenen Features der Multimediakonsole konfiguriert werden können.  Diese Features lassen sich in zwei Kategorien unterteilen: Allgemeine Medienkonsoleneinstellungen und die Medienplayliste.

### <a name="multimedia-console-general-settings"></a>Allgemeine Einstellungen der Multimediakonsole

**Wiedergabeeinstellungen**

Allgemeine Wiedergabeeinstellungen für die Medienliste

* **Schleifenmedienliste:** Bestimmt, ob die Medienliste eine Schleife durchschleifen soll, sobald Sie das Ende der Liste erreichen.
* **Start-Methode:** Wählt die Methode aus, mit der die Multimediakonsole gestartet werden soll.
    * Manuell: Wartet, bis die Wiedergabeschaltfläche gedrückt wird, bevor die Medien gestartet werden
    * Automatischer Start vom Anfang : Automatisches Starten der Medienliste am Anfang der Liste
    * Automatischer Start zufällig: Das Medium wird automatisch von einem zufälligen Startpunkt in der Liste gestartet.

**Rollen**

Rollenzuweisungen zum Steuern und Konfigurieren der Multimediakonsole.    Diese Rollen sind in den folgenden Satz aufgeschlüsselt:

* **Nur Besitzer:** Der Benutzer, der Besitzer der Multimedia-Konsolensitzung ist
* **Benutzer mit erhöhten Rechten:** Benutzer mit Moderator- oder Hostrollen in dem Bereich, in dem die Multimediakonsole ursprünglich konfiguriert ist
* **Alle Benutzer** – Alle Benutzer

Diese Rollen stapeln sich in dem Sinne, dass allen Rollen oberhalb der in dieser Liste ausgewählten Rollen auch die Berechtigung zur Verwendung dieses Features erteilt wird.  Beispiel: **Benutzer mit erhöhten Rechten** enthalten den **Besitzer** auch dann, wenn sie kein Moderator oder Host** in AltspaceVR sind. Funktionen, die durch Rollenzuweisungen gesteuert werden, lauten wie folgt:

* **Kann Media Player steuern:** Bestimmt, welche Rollen die Medienwiedergabeschaltflächen für die Multimediakonsole steuern können.
* **Kann den Media Player konfigurieren:** Bestimmt, welche Rollen die Multimedia-Konsole konfigurieren können, indem zugriff auf die Schaltfläche **"Konfiguration" gewährt** wird.

### <a name="adding-photos-and-videos-to-the-media-list"></a>Hinzufügen von Fotos und Videos zur Medienliste

Medien sind das Herzstück der Multimediakonsole.  Bilder und Videolinks werden in der Multimedia-Konsole als Medientypen unterstützt.  Um neue Medien hinzuzufügen,  wählen Sie entweder das Symbol Bild hinzufügen oder **Video** hinzufügen aus, um ein Dialogfeld zum Eingeben der Medieninformationen und -einstellungen anzuzeigen.  Im Folgenden finden Sie eine Aufschlüsselung der Medientypen und der zugehörigen Einstellungen.

**Bild**

Bilder sollten ein Standardbildtyp sein, z. B. jpeg, png und son on. Sie müssen über einen öffentlichen Link gehostet werden.

* **Name** : (Erforderlich) Name, mit dem Sie das Image identifizieren möchten.
* **Bild-URL** : (erforderlich) Die öffentliche URL des Bilds
* **Skip After** : Die Anzahl von Sekunden, nach der das Bild übersprungen werden soll

**Video**

Videos können über Twitch und DLive gehostete Videos oder Livestreams sein.  (Andere Unterstützung kann mit zusätzlicher Arbeit funktionieren, um die richtige Stream-URL zu erhalten, wird jedoch in der Multimedia-Konsole nicht vollständig unterstützt.)

* **Name** : (Erforderlich) Name, mit dem Sie das Video identifizieren möchten.
* **Video-URL** : (Erforderlich) Die öffentliche URL, unter der das Video gehostet wird oder von der der Livestream bereitgestellt wird.
* **Skip After** : Die Anzahl von Sekunden, nach der das Video übersprungen werden soll

> [!NOTE]
> ERFORDERLICH: Geben Sie die Zeit ein, die der Länge des Videos entspricht, damit Videos ordnungsgemäß weitergeleitet werden können. Wenn Ihr Video beispielsweise 5 Minuten lang ist, legen Sie 300 Sekunden ein, andernfalls springt Ihr Video nicht mit dem nächsten Inhaltsteil.

* **Volume:** Das Volumen des Videos von 0 (Min.) bis 1 (max.) Werten.
* **Startzeit:** Die Anzahl der Sekunden ab dem Anfang des Videos.
* **Roll Off Start Distance (Startabstand** abrollen) – Die Entfernung in Meter in der Welt, auf die das Volume absturzt, wenn Sie sich von der Multimediakonsole weg bewegen.
* **Ende der Videoaktion:** Die Aktion, die nach Dem Ende des Videos zu ergreifen ist.
    * Beenden: Die Medienliste wird beendet, nachdem das Video beendet wurde.
    * Schleife: Das Video wird schleife, bis es manuell übersprungen wird.
    * Weiter abspielen: Die nächsten Medien in der Medienliste werden gestartet, nachdem das aktuelle Video beendet wurde.

## <a name="working-with-json-directly-advancedoptional"></a>Direktes Arbeiten mit JSON (erweitert/optional)

Die Multimedia-Konsole unterstützt die direkte Eingabe von JSON in die Eingabeaufforderung der Konsole in AltspaceVR.  JSON ist der interne Mechanismus, mit dem wir Media Player-Konfigurationen aktivieren. Wenn Sie die Möglichkeit zum direkten Festlegen von JSON verfügbar machen, können fortgeschrittene Benutzer eigene Workflows erstellen, die ihren Anforderungen und ihrer Vertrautheit mit JSON entsprechen.  Im Folgenden finden Sie eine kurze Beschreibung der JSON-Struktur und des Schemas, anhand dessen der JSON-Code überprüft wird. Ausführlichere Beschreibungen der eigenschaften unten finden Sie in den obigen Abschnitten, in denen die Konfiguration der Multimediakonsole erläutert wird.  Dieser Abschnitt konzentriert sich hauptsächlich auf die Schemabeispiele und die Strukturierung für die JSON-Daten.

### <a name="global-media-settings"></a>Globale Medieneinstellungen

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>Medienliste

Die Medienliste ist eine Eigenschaft, die im Stammverzeichnis der JSON-Struktur festgelegt ist, z. B. rollen- und wiedergabe Einstellungen.  Es ist ein einfaches Array, das eine der folgenden Medienkonfigurationsstrukturen enthalten kann. (Ausführliche Informationen zu den einzelnen Funktionen finden Sie in den obigen Eigenschaftenbeschreibungen.)

**Bildbeispiel**

*Erforderliche Felder: "name" und "imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**Videobeispiel**

*Erforderliche Felder: "name" und "videoUrl"*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>JSON-Beispiel

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>Schema

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> Aktuell mit Multimedia Console v0.5.0