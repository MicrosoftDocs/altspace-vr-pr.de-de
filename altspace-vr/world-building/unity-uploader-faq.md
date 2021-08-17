---
title: Hilfe zum Unity-Uploader
description: Bleiben Sie über die neuesten häufig gestellten Fragen und Lösungen für den AltspaceVR Unity Uploader auf dem Laufenden.
ms.date: 02/10/2021
ms.topic: article
keywords: Hilfe, häufig gestellte Fragen
ms.openlocfilehash: cb983ba4e23186f7cc62043f75e7ea1b2969e92b6bd30b132f1733b5e25e92dd
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125695"
---
# <a name="unity-uploader-help"></a>Hilfe zum Unity-Uploader

**1. Wie toll ist dieses Tool?**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

Das ist meine Stargate Unity-Szene mit einer SDK-App, die gate und DND unterstützt

**2. Ich bin videolernend, wo sind meine Videos?**

[Sehen Sie sich unsere Videos an.](https://youtu.be/km9CnVYPzoM)

**3. Wo finde ich Beispiele?**

[Empfohlene Welten](https://account.altvr.com/worlds/featured) und [Beispiele von Jimmy](https://account.altvr.com/worlds/1046572460192825569) sind gute Ausgangspunkte.

**4. Funktioniert dies mit Kits und dem neuen SDK?**
Ja, Sie können alle Tools zusammen verwenden, wenn Sie möchten. Wir versuchen, sie so zu entwickeln, dass sie nahtlos zusammenarbeiten.

**5. Werden Partikeleffekte unterstützt?**

![GIF mit Schneeteilcheneffekten](images/uploader-faq-img-01.gif)

**6. Kann ich räumliche Audiodaten abrufen?**
Derzeit nicht, aber Sie können Audioquellen für die Wiedergabe in lokalisierten Bereichen platzieren. 

**7. Funktioniert die baked-Beleuchtung?**
Ja, aber Ihre Beleuchtung muss auf "baked" und nicht auf "gemischt" festgelegt werden.

**8. Funktioniert die globale Verarbeitung?**
Ja

**9. Müssen Sie die Welt immer zurücksetzen?**
Ja. Die Unity Asset Bundles müssen jedes Mal neu geladen werden. 

**10. Kann ich meine eigenen benutzerdefinierten Materialien und Shader verwenden?**

![GIF von benutzerdefinierten Materialien und Shadern](images/uploader-faq-img-02.gif)

**11. Kann ich nur auf eine Plattform hochladen?**
Ja, mit dem Uploadertool. Personen unter Android sehen jedoch erst dann etwas in Ihrer Welt, wenn Sie die Szene für ihre Plattform hochladen. 

**12. Sind Skripts zulässig?**
Nein, aus Sicherheitsgründen können wir keine Skripts oder Skriptverweise zulassen. Wenn Ihr Upload Skripts oder Skriptverweise enthält, wird er abgelehnt. Sehen Sie sich das neue SDK an, wenn Sie weltweit Skripts benötigen. 

**13. Wie groß kann ich eine Szene hochladen?**
Wir empfehlen Ihnen, klein zu beginnen und auf Personen in Altspace zu achten, die keine PCs besitzen. Das heißt, wir haben Spiele ihre Karten für Livestreams (z.B. Onward, ein VR-Spiel) in die Karten gebracht.

![Screenshot des VR-Spiels in AltspaceVR](images/uploader-faq-img-03.png)

**14. Muss ich die Szenendateien hosten?**
Nein, Altspace stellt die Dateien nach dem Hochladen zur

**15. Sind Schatten zulässig?**
Ja

**16. Wie schnell kann ich mit dem Uploader iterieren?**
Wenn Sie bereits in Ihrer Welt sind, können Sie Hochladen im Uploader drücken, Ihre Welt zurücksetzen und die aktualisierte Szene in nur 10 Sekunden anzeigen. In der Regel werden Schleifen von 30 Sekunden bis zu einigen Minuten angezeigt, je nach Komplexität Ihrer Szene. Sie haben ein Trank, sie sind welterstellerlich!

**17. Wo erhalte ich 3D-Modelle?**
Sketchfab, Sketchup, Minecraft, Unity Asset Store usw.

**18. Werden Animationen unterstützt?**

![GIF von benutzerdefinierten Animationen, die ausgeführt werden](images/uploader-faq-img-04.gif)

**19. Wie kann ich räumliche Audiodaten einrichten?** Importieren Sie die wav-Datei Ihrer Wahl, erstellen Sie ein leeres Spielobjekt in der Szene, und wählen Sie dieses Objekt aus. Ziehen Sie den importierten Sound per Drag & Drop in den Inspektor des Objekts, und es wird eine Audioquelle erstellt. Passen Sie anschließend die Lautstärke auf maximal 0,5 an, ändern Sie die räumliche Mischung in 3D, und passen Sie den mindesten und maximalen Abstand an, um einen richtigen Soundbereich zu erstellen. Dies wird standardmäßig als Kugel wie Collider angezeigt. Um eine echte Ablage zu erhalten, müssen Sie die Ablagekurve nach Ihren Wünschen anpassen. [(über @IsThatToasted )](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. Wie erkenne ich Augenübergreifend/Uneinsichtigkeit?**
Manchmal überschreibt der Uploader Ihre Renderingeinstellungen nicht erfolgreich. "Gehe zu > Project Einstellungen > Player bearbeiten". Stellen Sie sicher, dass "XR Einstellungen > Virtual Reality Supported" aktiviert ist und "Stereo Rendering Method" für PC und Android "Single Pass" oder "Single Pass (Preview)" ist (wählen Sie das Robotersymbol aus). Erstellen Sie anschließend erneut , und laden Sie sie hoch, und setzen Sie Ihre Welt zurück. 