---
title: Importieren von glTF-Modellen
description: Erfahren Sie, wie Sie 3D-GlTF-Modelle ordnungsgemäß in Ihre AltspaceVR-Funktionen importieren und Probleme beheben.
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

Eine Möglichkeit, 3D-Modelle und -Szenen in Altspace zu bringen, ist die Verwendung des [glTF-Standards](https://en.wikipedia.org/wiki/GlTF). Sie können eine GLB-Datei (gepacktes glTF) hochladen, um ein Modell zu erstellen, das Sie später im World Editor erstellen können. Dies ist eine Alternative zum [Hochladen Ihrer eigenen Kits.](uploading-custom-kits.md) Es wird empfohlen, Modelle für schnelle Demos zu erstellen, da Sie Unity und Kits nicht verwenden müssen, wenn Sie die Leistung und Wiederverwendbarkeit maximieren möchten. 

1. Suchen Sie nach einigen glTF 3D-Ressourcen. Ein Ort, an dem Sie suchen können, ist Sketchfab (versuchen Sie, nach **herunterladbaren** Modellen wie diesem zu [filtern).](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models) Sobald Sie es finden, wählen **Sie 3D-Modell herunterladen aus:**

![3D-Hundemodell von Sketchfab](images/importing-models-img-01.png)

2. Kopieren Sie den Link zum Modell, und lesen Sie die Lizenzanforderungen. 
3. Herunterladen der **GlTF-Version (Autoconverted Format)**

![Sketchfab-Downloadoptionen mit hervorgehobenen automatisch konvertierten Formaten](images/importing-models-img-02.png)

4. Öffnen Sie die [GLB Packer-Website,](https://glb-packer.glitch.me) und aktivieren Sie das Kontrollkästchen **Convert PNG to JPEG (beta) (PNG in JPEG konvertieren (Betaversion)).**
5. Dekomprimieren Sie die heruntergeladenen glTF-Dateien, und ziehen Sie sie alle gleichzeitig auf die GLB Packer-Browserregisterkarte.

![Fenster mit Der Dekomprimierung des Modells](images/importing-models-img-03.png)

6. Je nach Anzahl und Größe der Dateien kann die Verarbeitung eine Weile dauern. Wenn die Verarbeitung erfolgt ist, wird die Datei **out.glb** heruntergeladen. Benennen Sie diese Datei in einen informativen Namen um. Dies ist der Name des Objekts in der Welt (z.B. **Low Poly Muss.glb**).
7. Navigieren Sie zu [altvr.com > Weitere > Modelle,](https://account.altvr.com/users/sign_in) und wählen Sie **Erstellen aus.**
8. Geben Sie den Speicherort der GLB-Datei an, und kopieren Sie den Sketchfab-Link zur Zuordnung in die Beschreibung. Sie können ein Vorschaubild angeben, wenn Sie möchten, und dann **Modell erstellen auswählen:**

![Modellvorschau in AltspaceVR](images/importing-models-img-04.png)

9. Wählen Sie **In Zwischenablage kopieren aus.**
10. Öffnen Sie **den World Editor > Altspace > Basics > GLTF.**
11. Fügen Sie Ihre URL ein, und wählen Sie Bestätigen **aus.**

Herzlichen Glückwunsch! Sie haben soeben Ihr erstes Modell entwickelt.

## <a name="troubleshooting"></a>Problembehandlung

**Wenn ich auf Confirm nothing happened **(Nichts** geschehen bestätigen) geklickt habe**
    * Wir haben derzeit einen Polygongrenzwert von 100.000. Wenn ein Fehler auftritt, löschen Sie das Objekt, um potenzielle Probleme mit Benutzern zu vermeiden, die Ihrer Welt beitreten.
    * Möglicherweise gibt es andere Probleme mit der Ressource. Versuchen Sie, Objekte mit möglichst wenigen Polygonen zu verwenden.
    * Das Modell, das Sie verwenden, kann klein oder groß sein. Versuchen Sie, die Skalierung zu erhöhen/zu verringern, oder bewegen Sie Ihren Avatar, möglicherweise stehen Sie im Modell!

**Langsames Laden** Wie schnell andere Benutzer auf der Welt geladen werden, hängt von ihrer Verbindungsgeschwindigkeit ab. Es wird auch nicht wie Kit-Objekte zwischengespeichert. Wenn Sie ein Modell in Ihrer Startseite platzieren, laden Sie das gleiche Modell bei jedem Beitritt erneut ab, was nicht gut ist.

**Es gibt keine Kollision.** Standardmäßig gibt es keine Kollision mit den Objekten, die auf diese Weise gebracht werden.

**Wenn ich es aussuche,** verliere ich meine Steuerelemente auf sechs DOF, oder ich bin drin, sodass es schwierig ist, es zu bearbeiten. Ja, wir sind uns dieser Probleme bewusst und hoffen, sie bald beheben zu können.  