---
title: Hilfe zum Unity-Uploader
description: Bleiben Sie auf dem neuesten Stand mit den neuesten häufig gestellten Fragen und Lösungen für das altspacevr Unity Uploader.
ms.date: 02/10/2021
ms.topic: article
keywords: Hilfe, häufig gestellte Fragen
ms.openlocfilehash: 814ff293cb98490900cd929f33477d15d3d668ae
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213387"
---
# <a name="unity-uploader-help"></a>Hilfe zum Unity-Uploader

**1. wie großartig ist das Tool?**

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/cheyenne-mountain-gate-room-v1/player]

Das ist meine Stargate Unity-Szene mit einer SDK-APP, die das Gate und DND antreibt.

**2. Ich bin ein Video Lernmodul, in dem meine Videos angezeigt werden?**

[Sehen Sie sich unsere Videos an](https://youtu.be/km9CnVYPzoM)

**3. wo finde ich Beispiele?**

[](https://account.altvr.com/worlds/featured) Die [Beispiele von Beispielen und Jimmy](https://account.altvr.com/worlds/1046572460192825569) sind gute Ausgangspunkte.

**4. wird dies mit Kits und dem neuen SDK funktionieren?**
Ja, Sie können alle Tools in der gewünschten Weise verwenden. Wir versuchen, Sie so zu entwickeln, dass Sie nahtlos zusammenarbeiten.

**5. unterstützt er Partikeleffekte?**

![GIF von Schnee Partikel Effekten](images/uploader-faq-img-01.gif)

**6. kann ich spatialisierte Audiodaten erhalten?**
Nicht momentan, aber Sie können Audioquellen für die Wiedergabe in lokalisierten Bereichen platzieren. 

**7. funktioniert die gebrannte Beleuchtung?**
Ja, aber Ihre Beleuchtung muss auf "gebacken" und nicht "gemischt" festgelegt werden.

**8. funktioniert die globale Beleuchtung?**
Ja

**9. müssen Sie die Welt immer zurücksetzen?**
Ja. Wir müssen die Unity-Asset-Bündel jedes Mal neu laden. 

**10. kann ich meine eigenen benutzerdefinierten Materialien und Shader verwenden?**

![GIF von benutzerdefinierten Materialien und Shadern](images/uploader-faq-img-02.gif)

**11. kann ich nur auf eine Plattform hochladen?**
Ja, mit dem Uploader-Tool. Personen, die sich auf Android befinden, werden jedoch erst dann in ihrer Welt angezeigt, wenn Sie die Szene für Ihre Plattform hochgeladen haben. 

**12. sind Skripts zulässig?**
Nein. aus Sicherheitsgründen können keine Skripts oder Skript Verweise zugelassen werden. Wenn Ihr Upload Skripts oder Skript Verweise enthält, wird das Paket zurückgewiesen. Sehen Sie sich das neue SDK an, wenn Sie eine Skripterstellung benötigen. 

**13. wie groß ist eine Szene, die hochgeladen werden kann?**
Wir empfehlen Ihnen, klein zu beginnen und die Menschen in altspace zu berücksichtigen, die keine Monster-PCs haben. Das heißt, wir haben Spiele in Ihre Karten für Livestreams gebracht (z. b. ein VR-Shooter-Spiel).

![Screenshot des VR-Spiels in altspacevr](images/uploader-faq-img-03.png)

**14. muss ich die Szenen Dateien hosten?**
Nein, die Dateien werden von "altspace" nach dem Hochladen nach hochgeladen.

**15. sind Schatten zulässig?**
Ja

**16. wie schnell kann ich mit dem Uploader iterieren?**
Wenn Sie sich bereits in ihrer Welt befinden, können Sie im Uploader hochladen drücken, ihre Welt zurücksetzen und die aktualisierte Szene in bis zu 10 Sekunden sehen. In der Regel sehen Sie Schleifen von 30 Sekunden bis zu einigen Minuten, je nach Komplexität Ihrer Szene. Sie haben einen Drink, den Sie für eine Welt-Builder-Umgebung verdient haben!

**17. Wo erhalte ich 3D-Modelle?**
"Schrägerfab", "schief", "minecraft", "Unity Asset Store" usw.

**18. unterstützt es Animationen?**

![GIF benutzerdefinierter Animationen, die ausgeführt werden](images/uploader-faq-img-04.gif)

**19. wie kann ich räumliche Audiodaten einrichten?** Importieren Sie die gewünschte WAV-Datei, erstellen Sie ein leeres Spielobjekt in der Szene, und wählen Sie dieses Objekt aus. Verschieben Sie den importierten Sound per Drag & amp; Drop in den Inspektor des Objekts, und es wird eine Audioquelle erstellt. Passen Sie anschließend das Volume auf nicht mehr als 0,5 an, ändern Sie die räumliche Mischung in 3D, und passen Sie die minimale und maximale Entfernung an, um einen passenden Sound Bereich zu erstellen. Dies wird in der Standardeinstellung als Kugel ähnlich wie Colliders angezeigt. Um einen echten Dropdown zu erhalten, müssen Sie die Dropdown Kurve entsprechend anpassen. [(via @IsThatToasted )](https://www.youtube.com/watch?v=ktb2vAAwknw&list=PLGmYIROty-5bpzKQNK3mRMi4pmh_LinV4&t=642s&index=29)

**20. wie kommt es zu einer über-und ausblendheit?**
Manchmal überschreibt das Uploader ihre renderingeinstellungen nicht erfolgreich. "Wechseln Sie zu Edit > Project Settings > Player". Stellen Sie sicher, dass "XR-Einstellungen > Virtual Reality unterstützt" aktiviert ist, und "Stereo Rendering Method" für PC und Android "Single Pass" oder "Single Pass (Preview)" (Wählen Sie das Roboter Symbol aus). Anschließend erstellen Sie neu und laden Sie erneut hoch. 