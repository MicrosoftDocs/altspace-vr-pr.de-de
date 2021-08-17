---
title: Importieren von glTF-Modellen
description: Erfahren Sie, wie Sie 3D glTF-Modelle ordnungsgemäß in Ihre AltspaceVR-Funktionen importieren und Probleme beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: models, glTF, importing, sketchfab, troubleshooting
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127059"
---
# <a name="importing-gltf-models"></a>Importieren von glTF-Modellen

> [!NOTE]
> Dieses Feature ist derzeit für ausgewählte Benutzer im Early Access-Programm verfügbar.

Eine Möglichkeit, 3D-Modelle und Szenen in Altspace zu integrieren, ist die Verwendung des [glTF-Standards](https://en.wikipedia.org/wiki/GlTF). Sie können eine GLB-Datei (gepackte glTF) hochladen, um ein Modell zu erstellen, das Sie später im World Editor erzeugen können. Es ist eine Alternative zum [Hochladen Ihrer eigenen Kits.](uploading-custom-kits.md) Es wird empfohlen, Modelle für schnelle Demonstrationen zu erstellen, da Sie Unity und Kits nicht verwenden müssen, wenn Sie die Leistung und Wiederverwendebarkeit maximieren möchten. 

1. Suchen Sie nach einigen glTF-3D-Ressourcen. Ein Ort für die Suche ist Sketchfab (versuchen Sie, nach **herunterladbaren** Modellen wie [diesem](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)zu filtern). Sobald Sie es gefunden haben, wählen **Sie 3D-Modell herunterladen** aus:

![3D-Hundemodell von Sketchfab](images/importing-models-img-01.png)

2. Kopieren Sie den Link zum Modell, und lesen Sie die Lizenzierungsanforderungen. 
3. Herunterladen der **GlTF-Version (Autoconverted Format)**

![Sketchfab-Downloadoptionen mit hervorgehobener Option für automatisch konvertiertes Format](images/importing-models-img-02.png)

4. Öffnen Sie die [GLB Packer-Website,](https://glb-packer.glitch.me) und aktivieren Sie das Kontrollkästchen **Convert PNG to JPEG (beta) (PNG in JPEG konvertieren (Betaversion)).**
5. Dekomprimieren Sie die heruntergeladenen glTF-Dateien, und ziehen Sie sie alle gleichzeitig auf die GLB Packer-Browserregisterkarte.

![Fenster, in dem die Modellkomprimierung angezeigt wird](images/importing-models-img-03.png)

6. Je nach Anzahl und Größe der Dateien kann die Verarbeitung eine Weile dauern. Wenn die Verarbeitung abgeschlossen ist, wird eine **out.glb-Datei** heruntergeladen. Benennen Sie diese Datei in einen informativen Namen um. Dies ist der Name des Objekts auf der ganzen Welt (z.B. **Low Poly Soll.glb**).
7. Navigieren Sie zu [altvr.com > Weitere > Modelle,](https://account.altvr.com/users/sign_in) und wählen **Sie Erstellen** aus.
8. Geben Sie den Speicherort der GLB-Datei an, und stellen Sie sicher, dass Sie den Sketchfab-Link zur Zuordnung in die Beschreibung kopieren. Sie können bei Bedarf ein Vorschaubild angeben und dann **Modell erstellen** auswählen:

![Modellvorschau in AltspaceVR](images/importing-models-img-04.png)

9. Wählen Sie **In Zwischenablage kopieren aus.**
10. Öffnen Sie den **World Editor > Altspace > Basics > GLTF.**
11. Fügen Sie Ihre URL ein, und wählen Sie **Bestätigen** aus.

Herzlichen Glückwunsch! Sie haben gerade Ihr erstes Modell ausgelöst.

## <a name="troubleshooting"></a>Problembehandlung

**Wenn ich auf **Bestätigen** klicke, dass nichts passiert ist**
    * Derzeit gilt ein Polygongrenzwert von 100.000. Wenn der Fehler auftritt, löschen Sie das Objekt, um potenzielle Probleme mit Benutzern zu vermeiden, die Ihrer Welt beitreten.
    * Es kann andere Probleme mit dem Medienobjekt geben. Versuchen Sie, Ressourcen mit so wenigen Polygonen wie möglich zu verwenden.
    * Das Modell, das Sie einbringen, kann klein oder groß sein. Versuchen Sie, die Skalierung zu erhöhen oder zu verringern, oder bewegen Sie Ihren Avatar, da Sie möglicherweise im Modell stehen!

**Das Laden ist langsam.** Wie schnell andere Benutzer in der Welt geladen werden, hängt von ihrer Verbindungsgeschwindigkeit ab. Es wird auch nicht wie Kit-Ressourcen zwischengespeichert. Wenn Sie ein Modell in Ihrer Startseite platzieren, laden Sie das gleiche Modell jedes Mal erneutherunter, wenn Sie beitreten. Dies ist nicht besonders gut.

**Es kommt zu keinem Konflikt.** Standardmäßig kommt es nicht zu einem Konflikt bei den Objekten, die auf diese Weise geschaltet werden.

**Wenn ich sie auswähle, verliere ich meine Steuerelemente auf sechs DOF oder ich bin darin, sodass es schwierig ist, sie zu bearbeiten.** Ja, wir sind uns dieser Probleme bewusst und hoffen, sie bald beheben zu können.  