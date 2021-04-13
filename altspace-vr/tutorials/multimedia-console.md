---
title: Verwenden der Multimedia-Konsole
description: Erfahren Sie, wie Sie mit der Konfiguration, Veröffentlichung und Steuerung der Multimedia-Konsole in ihren altspacevr-Erfahrungen beginnen.
ms.date: 03/11/2021
ms.topic: article
keywords: Konsole, Multimedia
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212236"
---
# <a name="using-the-multimedia-console"></a>Verwenden der Multimedia-Konsole

Die Multimedia-Konsole ist ein Tool, das die Medien Freigabe in Ereignissen und Welten ermöglicht. Sie können Sie verwenden, um Dinge wie Bilder, Präsentationsfolien, Livestreams, Videos, Wiedergabelisten usw. gemeinsam zu nutzen. Im folgenden finden Sie eine Schritt-für-Schritt-Anleitung zur Verwendung der Multimedia Console **v 0.5.0 +**. 

## <a name="getting-started"></a>Erste Schritte

Die ersten Schritte mit der Multimedia-Konsole sind ein zwei teilige Prozess.  Zuerst wird das Webportal verwendet, mit dem Sie eine Konfiguration für die Multimedia-Konsolen Sitzung generieren und veröffentlichen können, die Sie in Ihrer Umgebung platzieren.  Zweitens ist die Platzierung der eigentlichen Multimedia-Konsolen-app in Ihrer Umgebung und das Festlegen des zu verwendenden Konfigurations Codes.

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Konfigurieren der Multimedia-Konsole mit dem Webportal

1. Zunächst müssen Sie sicherstellen, dass Ihre Inhalte online gehostet werden, da Sie eine URL benötigen. (Sie können Fotos in altvr.com hochladen, eine Video-MP4-Datei Online hosten oder den Link Twitch Live Stream verwenden: https://www.twitch.tv/ninja) 
2. Navigieren Sie zum Webportal für die Multimedia-Konsole unter. [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. Über das Webportal können Sie eine Konfiguration für die Multimedia-Konsole generieren und veröffentlichen.  (Weitere Informationen zu den verschiedenen Eigenschaften finden Sie unten.)
4. Nachdem Sie das Medium in die Medien Liste eingegeben und die allgemeinen Einstellungen konfiguriert haben, wählen Sie im oberen rechten Bereich der APP die Schaltfläche veröffentlichen aus.
5. Sobald die Veröffentlichung abgeschlossen ist, wird ein Dialogfeld mit einem zwei Word-Code angezeigt, in dem Sie die von Ihnen eingestellte Multimedia-Konsole eingeben können.
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>Platzieren der Multimedia-Konsole in Ihrer Umgebung

1. Wählen Sie auf der **Welt-Editor > Editor Panel > SDK-apps > Multimedia Console** aus. (Wechseln Sie nicht zum **Welt-Editor > Grundlagen > SDK-App**, die für nicht registrierte Apps steht.)  
2. Positionieren Sie die Multimedia-Konsole, um ihren Platz und Ihre Zielgruppe am besten zu platzieren
3. Klicken Sie auf die Schaltfläche orangefarbener Bearbeitungsmodus, um den Bearbeitungsmodus zu verlassen.
4. Sie werden gefragt, dass **Sie der Media Player-Besitzer sind?** Wenn Sie die Person sind, die der offizielle Besitzer dieser Multimedia-Konsolen Sitzung sein soll, bestätigen Sie den Vorgang, und fahren Sie fort. (Es sind auch weitere Rollen bezogene Rollen verfügbar. Eine ausführliche Liste finden Sie unten.)
5. Wählen Sie ja aus, um zu bestätigen, dass Sie der primäre Host sind.  
6. Daraufhin wird ein Dialogfeld angezeigt, in dem Sie aufgefordert werden, einen Code aus dem Webportal oder aus einem gültigen JSON-Code einzugeben.  Geben Sie den beiden Wort Code aus dem Webportal ein, einschließlich des Bindestrichs, und drücken Sie OK. (JSON ist eine erweiterte Konfiguration, die unten beschrieben ist.)
7. Die Multimedia-Konsole sollte nach einigen Sekunden mit der Konfiguration geladen werden, die Sie im Webportal erstellt haben.

### <a name="controlling-the-multimedia-console"></a>Steuern der Multimedia-Konsole

1. Nachdem Sie den Code eingegeben und den Konfigurationsprozess fertiggestellt haben, werden die Kontroll Schaltflächen unterhalb einer Medien Anzeige angezeigt. 
    * Wiedergeben startet den Media Viewer ( **oder startet beim** aktuellen Eintrag neu, wenn er zuvor beendet wurde). 
    * **Beenden** beendet die Medien Anzeige und blendet die aktuellen Medien aus.  
    * **Next/Prev** springt auf das nächste oder vorherige Medium. 
    * **x/x**   zeigt den aktuellen Index in der Medien Liste an und ermöglicht es Ihnen, zu einem beliebigen Punkt in der Liste zu springen.
    * **Config** ermöglicht das erneute Eingeben eines neuen Codes aus dem Webportal, um eine neue Konfiguration in der-Konsole festzulegen. 

Nun haben Sie festgelegt, dass Sie über die Multimedia-Konsole mit der Freigabe beginnen!  
 
## <a name="working-with-the-web-portal"></a>Arbeiten mit dem Webportal

Das Webportal ist eine Web-App, die die Konfiguration der verschiedenen Features der Multimedia-Konsole ermöglicht.  Diese Funktionen sind in zwei Kategorien unterteilt: Allgemeine Medien Konsolen Einstellungen und die Liste der Medienwiedergabe.

### <a name="multimedia-console-general-settings"></a>Allgemeine Einstellungen der Multimedia-Konsole

**Wiedergabeeinstellungen**

Allgemeine Wiedergabe Einstellungen für die Medien Liste

* **Schleifen Medien Liste**: bestimmt, ob die Medien Liste eine Schleife durchlaufen soll, sobald Sie das Ende der Liste erreicht haben.
* **Start Methode** : wählt die Methode aus, mit der die Multimedia-Konsole gestartet werden soll.
    * Manuell: wartet, bis die Wiedergabe Schaltfläche gedrückt wird, bevor die Medien gestartet werden.
    * Automatischer Start von Anfang an: Automatisches Starten der Medien Liste am Anfang der Liste
    * Automatisches Starten von Random: Automatisches Starten des Mediums von einem zufälligen Startpunkt in der Liste

**Rollen**

Rollenzuweisungen zum Steuern und Konfigurieren der Multimedia-Konsole.    Diese Rollen sind in den folgenden Satz untergliedert:

* **Nur Besitzer** : der Benutzer, der Besitzer der Multimedia-Konsolen Sitzung ist.
* **Erhöhte Benutzer** : Benutzer, die über Moderator-, Host-oder präsentatorrollen im Bereich verfügen, in dem die Multimedia-Konsole ursprünglich konfiguriert ist
* **Alle Benutzer** -alle Benutzer

Diese Rollen Stapeln in dem Sinn, dass alle Rollen oberhalb der in dieser Liste ausgewählten Rollen auch die Berechtigung zur Verwendung dieses Features erhalten.  Beispiel: **Benutzer mit erhöhten** rechten enthalten den **Besitzer** , auch wenn Sie kein Moderator, Host oder Presenter * * in altspacevr sind. Folgende Features werden durch Rollenzuweisungen gesteuert:

* **Kann Media Player Steuern** : legt fest, welche Rollen die Medienwiedergabe Schaltflächen für die Multimedia-Konsole steuern können.
* **Kann den Media Player konfigurieren** : legt fest, welche Rollen die Multimedia-Konsole konfigurieren können, indem Sie Zugriff auf die **Konfigurations** Schaltfläche erhält.

### <a name="adding-photos-and-videos-to-the-media-list"></a>Hinzufügen von Fotos und Videos zur Medien Liste

Medien sind das Herzstück der Multimedia-Konsole.  Bilder und Video Links werden als Medientypen in der Multimedia-Konsole unterstützt.  Wenn Sie neue Medien hinzufügen möchten, wählen Sie entweder die Symbole **Bild hinzufügen** oder **Video hinzufügen** aus, um ein Dialogfeld zum Eingeben der Medieninformationen und-Einstellungen anzuzeigen.  Im folgenden finden Sie eine Aufschlüsselung der Medientypen und der zugehörigen Einstellungen.

**Image**

Bilder sollten ein Standard Bildtyp wie JPEG, PNG und Son in sein. Sie müssen an einem Ort mit einer öffentlichen Verknüpfung gehostet werden.

* **Name** (erforderlich) Name, mit dem Sie das Bild identifizieren möchten.
* **Bild-URL** -(erforderlich) die öffentliche URL des Bilds
* Über **springen nach** : die Anzahl der Sekunden, nach der das Bild ausgelassen werden soll.

**Video**

Videos können mithilfe von Twitch und dlive als gehostete Videos oder Livestreams angezeigt werden.  (Andere Unterstützung kann mit zusätzlicher Arbeit funktionieren, um die richtige Stream-URL zu erhalten, wird jedoch in der Multimedia-Konsole nicht vollständig unterstützt.)

* **Name** (erforderlich) der Name, mit dem Sie das Video identifizieren möchten.
* **Video-URL** : (erforderlich) die öffentliche URL, unter der das Video gehostet wird, oder der Livestream wird von bereitgestellt.
* Über **springen nach** : die Anzahl der Sekunden, nach der das Video übersprungen werden soll.
* **Volume** : das Volume des Videos von 0 (min.)-1 (max)-Werten.
* **Startzeit** : die Anzahl von Sekunden ab dem Beginn des Videos ab.
* **Start Distanz ausschalten** : die Distanz in Meter der Welt, an der das Volume beginnt, wenn Sie von der Multimedia-Konsole Weg wechseln.
* **Ende der Video Aktion** : die Aktion, die nach dem Ende des Videos ausgeführt wird, wird erreicht.
    * Beenden: die Medien Liste wird beendet, nachdem das Video beendet wurde.
    * Schleife: das Video führt eine Schleife aus, bis es manuell übersprungen wird
    * Weitergeben: das nächste Medium in der Medien Liste wird nach dem Ende des aktuellen Videos gestartet.

## <a name="working-with-json-directly-advancedoptional"></a>Direktes Arbeiten mit JSON (erweitert/optional)

Die Multimedia-Konsole unterstützt die direkte Eingabe von JSON in die Eingabeaufforderung der Konsole in altspacevr.  JSON ist der interne Mechanismus, mit dem wir die Media Player-Konfigurationen aktivieren. Die Möglichkeit, JSON direkt festzulegen, ist eine Möglichkeit, mit der Erweiterte Benutzer ihre eigenen Workflows erstellen können, die Ihre Bedürfnisse und Vertrautheit mit JSON Auflistungen gestalten.  Im folgenden finden Sie eine kurze Beschreibung der JSON-Struktur und des Schemas, mit dem der JSON-Code überprüft wird. Ausführlichere Beschreibungen der unten aufgeführten Eigenschaften finden Sie in den obigen Abschnitten, in denen die Konfiguration der Multimedia-Konsole erläutert wird.  Dieser Abschnitt konzentriert sich hauptsächlich auf die Schema Beispiele und die Strukturierung der JSON-Daten.

### <a name="global-media-settings"></a>Globale Medien Einstellungen

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>Medien Liste

Die Medien Liste ist eine Eigenschaft, die im Stammverzeichnis der JSON-Struktur wie die Rollen und Wiedergabe Einstellungen festgelegt ist.  Dabei handelt es sich um ein einfaches Array, das eine der folgenden Medien Konfigurations Strukturen enthalten kann. (Ausführliche Informationen zu den einzelnen Funktionen finden Sie in den oben aufgeführten Eigenschaften Beschreibungen.)

**Bildbeispiel**

*Erforderliche Felder: "Name" und "ImageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**Video Beispiel**

*Erforderliche Felder: "Name" und "videourl"*

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
> Auf dem neuesten Stand mit der Multimedia Console v 0.5.0