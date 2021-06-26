---
title: Verwenden der Multimediakonsole
description: Erfahren Sie, wie Sie mit dem Konfigurieren, Veröffentlichen und Steuern der Multimediakonsole in Ihren AltspaceVR-Funktionen beginnen.
ms.date: 03/11/2021
ms.topic: article
keywords: Konsole, Multimedia
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923007"
---
# <a name="using-the-multimedia-console"></a>Verwenden der Multimediakonsole

Die Multimediakonsole ist ein Tool, das die Medienfreigabe in Ereignissen und Welten ermöglicht. Sie können damit u. a. Bilder, Präsentationsfolien, Livestreams, Videos, Wiedergabelisten und vieles mehr freigeben. Im Folgenden finden Sie eine schrittweise Anleitung zur Verwendung der Multimedia-Konsole **v0.5.0+**. 

## <a name="getting-started"></a>Erste Schritte

Die ersten Schritte mit der Multimediakonsole sind ein zweiteiler Prozess.  Zuerst gibt es das Webportal, mit dem Sie eine Konfiguration für die Multimediakonsolensitzung generieren und veröffentlichen, die Sie in Ihrer Umgebung platzieren.  Das zweite ist die Platzierung der eigentlichen Multimediakonsolen-App in Ihrer Umgebung und das Festlegen des Konfigurationscodes, den sie verwenden soll.

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Konfigurieren der Multimediakonsole mit dem Webportal

1. Zunächst müssen Sie sicherstellen, dass Ihre Inhalte online gehostet werden, da Sie eine URL benötigen. (Sie können Fotos in altvr.com hochladen, ein Video .mp4 Datei online hosten oder einen Dlive-Livestreamlink verwenden: https://dlive.tv/yourlivestream) 
2. Navigieren Sie zum Webportal für die Multimediakonsole unter . [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. Über das Webportal können Sie eine Konfiguration für die Multimediakonsole generieren und veröffentlichen.  (Weitere Informationen zu den verschiedenen Eigenschaften finden Sie unten.)
4. Nachdem Sie die Medien in die Medienliste eingegeben und die allgemeinen Einstellungen konfiguriert haben, wählen Sie oben rechts in der App die Schaltfläche Veröffentlichen aus.
5. Sobald die Veröffentlichung abgeschlossen ist, wird ein Dialogfeld mit einem Zwei-Wort-Code angezeigt, den Sie in die von Ihnen platzierte Multimediakonsole eingeben können.
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>Platzieren der Multimediakonsole in Ihrer Umgebung

1. Wählen Sie **> Editor-Bereich > SDK-Apps > Multimedia-Konsole** die Option World Editor aus. (Wechseln Sie nicht zu **World Editor > Basics > SDK-App**, die für nicht registrierte Apps gilt.)  
2. Positionieren Sie die Multimediakonsole so, dass Ihr Raum und Ihre Zielgruppe am besten geeignet sind.
3. Wechseln Sie aus dem Bearbeitungsmodus, indem Sie auf die orangefarbene Schaltfläche Edit Mode (Bearbeitungsmodus) klicken.
4. Sie werden **gefragt, sind Sie der Besitzer des Media Player?** Wenn Sie die Person sind, die der offizielle Besitzer dieser Multimediakonsolensitzung sein soll, bestätigen Sie dies, und fahren Sie fort. (Weitere rollenberechtigungen sind ebenfalls verfügbar. Eine ausführliche Liste finden Sie unten.)
5. Wählen Sie Ja aus, um zu bestätigen, dass Sie der primäre Host sind.  
6. Es sollte ein Dialogfeld angezeigt werden, in dem Sie aufgefordert werden, einen Code aus dem Webportal oder gültigen JSON-Code einzugeben.  Geben Sie den Zwei-Wort-Code aus dem Webportal ein, einschließlich des Bindestrichs, und drücken Sie OK. (JSON ist eine weiter unten beschriebene erweiterte Konfiguration.)
7. Die Multimediakonsole sollte nach einigen Sekunden mit der Konfiguration geladen werden, die Sie im Webportal erstellt haben.

### <a name="controlling-the-multimedia-console"></a>Steuern der Multimediakonsole

1. Nachdem Sie Ihren Code eingegeben und den Konfigurationsprozess abgeschlossen haben, werden Steuerelementschaltflächen unterhalb einer Medienanzeige angezeigt. 
    * **Wiedergabe** startet den Medien-Viewer (oder startet beim aktuellen Eintrag neu, falls er zuvor beendet wurde) 
    * **Beenden** beendet die Medienanzeige und blendet aktuelle Medien aus.  
    * **Next/Prev** überspringt das nächste oder vorherige Medium. 
    * **x/x**   zeigt den aktuellen Index in der Medienliste an und ermöglicht es Ihnen, zu einem beliebigen Punkt in der Liste zu springen.
    * **Die Konfiguration** ermöglicht das erneute Eingeben eines neuen Codes aus dem Webportal, um eine neue Konfiguration in der Konsole festzulegen. 

Jetzt können Sie mit der Freigabe über die Multimediakonsole beginnen.  
 
## <a name="working-with-the-web-portal"></a>Arbeiten mit dem Webportal

Das Webportal ist eine Web-App, mit der die verschiedenen Funktionen der Multimediakonsole konfiguriert werden können.  Diese Features lassen sich in zwei Kategorien unterteilen: Allgemeine Medienkonsoleneinstellungen und die Medienwiedergabeliste.

### <a name="multimedia-console-general-settings"></a>Allgemeine Einstellungen der Multimediakonsole

**Wiedergabeeinstellungen**

Allgemeine Wiedergabeeinstellungen für die Medienliste

* **Schleifenmedienliste:** Bestimmt, ob die Medienliste eine Schleife durchlaufen soll, sobald Sie das Ende der Liste erreicht haben.
* **Methode starten:** Wählt die Methode aus, mit der die Multimediakonsole gestartet werden soll.
    * Manuell: Wartet, bis die Wiedergabeschaltfläche gedrückt wird, bevor das Medium gestartet wird.
    * Automatisch von Anfang starten: Starten Sie die Medienliste automatisch am Anfang der Liste.
    * Auto Start Random : Startet die Medien automatisch von einem zufälligen Startpunkt in der Liste

**Rollen**

Rollenzuweisungen zum Steuern und Konfigurieren der Multimediakonsole.    Diese Rollen sind in folgende Gruppe unterteilt:

* **Nur Besitzer:** Der Benutzer, der Besitzer der Multimediakonsolensitzung ist
* Benutzer mit **erhöhten Rechten:** Benutzer mit Moderator- oder Hostrollen in dem Bereich, in dem die Multimediakonsole ursprünglich konfiguriert wurde
* **Alle Benutzer** – Alle Benutzer

Diese Rollen stapeln sich in dem Sinne, dass allen Rollen, die über der in dieser Liste ausgewählten Rolle liegen, auch die Berechtigung zum Verwenden dieses Features erteilt wird.  Beispiel: Benutzer mit **erhöhten Rechten** enthalten den **Besitzer,** auch wenn sie kein Moderator oder Host** in AltspaceVR sind. Funktionen, die durch Rollenzuweisungen gesteuert werden, sind wie folgt:

* **Kann den Medienplayer steuern:** Bestimmt, welche Rollen die Medienwiedergabeschaltflächen für die Multimediakonsole steuern können.
* **Kann den Media Player konfigurieren:** Bestimmt, welche Rollen die Multimediakonsole konfigurieren können, indem Zugriff auf die Schaltfläche **"Konfiguration"** gewährt wird.

### <a name="adding-photos-and-videos-to-the-media-list"></a>Hinzufügen von Fotos und Videos zur Medienliste

Medien sind das Kernstück der Multimediakonsole.  Bilder und Videolinks werden in der Multimediakonsole als Medientypen unterstützt.  Um neue Medien hinzuzufügen, wählen Sie entweder das Symbol **Bild hinzufügen** oder **Video hinzufügen** aus, damit ein Dialogfeld angezeigt wird, in dem die Medieninformationen und -einstellungen eingegeben werden.  Im Folgenden finden Sie eine Aufschlüsselung der Medientypen und der zugehörigen Einstellungen.

**Image**

Bilder sollten ein Standardbildtyp wie jpeg, png und son on sein. Sie müssen an einem Ort mit einem öffentlichen Link gehostet werden.

* **Name:** (Erforderlich) Der Name, mit dem Sie das Bild identifizieren möchten.
* **Bild-URL** – (erforderlich) Die öffentliche URL des Bilds
* **Überspringen nach:** Die Anzahl von Sekunden, nach der das Bild übersprungen werden soll

**Video**

Videos können über Twitch und DLive gehostet werden.  (Andere Unterstützung kann mit zusätzlichem Aufwand funktionieren, um die richtige Stream-URL abzurufen, wird jedoch nicht vollständig in der Multimediakonsole unterstützt.)

* **Name:** (Erforderlich) Der Name, mit dem Sie das Video identifizieren möchten.
* **Video-URL** : (Erforderlich) Die öffentliche URL, unter der das Video gehostet wird oder von der aus der Livestream bereitgestellt wird.
* **Überspringen nach** : Die Anzahl von Sekunden, nach der das Video übersprungen werden soll

> [!NOTE]
> ERFORDERLICH: Geben Sie die Zeit ein, die der Länge des Videos entspricht, damit Videos ordnungsgemäß weitergeleitet werden können. Wenn Ihr Video beispielsweise 5 Minuten lang ist, legen Sie 300 Sekunden ein, andernfalls wird Ihr Video nicht mit dem nächsten Inhaltsteil übersprungen.

* **Volume:** Das Videovolumen von 0 (min) bis 1 (max) Werten.
* **Startzeit:** Die Anzahl von Sekunden ab dem Anfang des Videos.
* **Roll Off Start Distance** :Die Entfernung in Metern auf der Welt, bei der das Volumen abfällt, wenn Sie sich von der Multimediakonsole wegbewegt haben.
* **Videoendeaktion:** Die Aktion, die nach Erreichen des Videoendes erfolgen soll.
    * Beenden: Die Medienliste wird beendet, nachdem das Video beendet wurde.
    * Schleife: Das Video führt eine Schleife durch, bis es manuell übersprungen wird.
    * Weiter wiedergeben: Die nächsten Medien in der Medienliste werden gestartet, nachdem das aktuelle Video beendet wurde.

## <a name="working-with-json-directly-advancedoptional"></a>Direktes Arbeiten mit JSON (erweitert/optional)

Die Multimediakonsole unterstützt das direkte Eingeben von JSON in die Eingabeaufforderung der Konsole in AltspaceVR.  JSON ist der interne Mechanismus, mit dem Media Player-Konfigurationen aktiviert werden. Die Möglichkeit, JSON direkt festzulegen, ermöglicht es erweiterten Benutzern, ihre eigenen Workflows zu erstellen, die ihre Anforderungen erfüllen und mit JSON vertraut sind.  Es folgt eine kurze Beschreibung der JSON-Struktur und des Schemas, nach dem der JSON-Code überprüft wird. Ausführlichere Beschreibungen der folgenden Eigenschaften finden Sie in den obigen Abschnitten zum Konfigurieren der Multimediakonsole.  Dieser Abschnitt konzentriert sich hauptsächlich auf die Schemabeispiele und die Strukturierung für die JSON-Daten.

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

Die Medienliste ist eine Eigenschaft, die im Stammverzeichnis der JSON-Struktur festgelegt ist, z. B. Rollen und Wiedergabeeinstellungen.  Es ist ein einfaches Array, das eine der folgenden Medienkonfigurationsstrukturen enthalten kann. (Ausführliche Informationen zu den einzelnen Eigenschaften finden Sie oben in den Eigenschaftenbeschreibungen.)

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
> Aktuelle Version von Multimedia Console v0.5.0