---
title: Importieren von gltf-Modellen
description: Erfahren Sie, wie Sie 3D-gltf-Modelle ordnungsgemäß in Ihre altspacevr-Erfahrungen importieren und Probleme beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Modelle, gltf, Import, schräl, Problembehandlung
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213259"
---
# <a name="importing-gltf-models"></a>Importieren von gltf-Modellen

> [!NOTE]
> Diese Funktion ist zurzeit für ausgewählte Benutzer im frühzeitigen Zugriffs Programm verfügbar.

Eine Möglichkeit zum bringen von 3D-Modellen und-Szenen in altspace ist die Verwendung des [gltf-Standards](https://en.wikipedia.org/wiki/GlTF). Sie können eine GLB-Datei (gepacktes gltf) hochladen, um ein Modell zu erstellen, das Sie später im World-Editor erzeugen können. Es ist eine Alternative zum [Hochladen Ihrer eigenen Kits](uploading-custom-kits.md). Wir empfehlen die Erstellung von Modellen für schnelle Demos, da Sie Unity nicht verwenden müssen, und Kits, wenn Sie die Leistung und Wiederverwendbarkeit maximieren möchten. 

1. Suchen Sie nach einigen gltf 3D-Assets. Ein Ort für die Suche ist "schrätchfab" (Filtern Sie nach **herunterladbaren** Modellen wie [diesem](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)). Wenn Sie ihn gefunden haben, wählen Sie **3D-Modell herunterladen** aus:

![3D-Hunde Modell aus "schrätchfab"](images/importing-models-img-01.png)

2. Kopieren Sie den Link in das Modell, und lesen Sie die Lizenzanforderungen. 
3. Herunterladen der Version des **Auto konvertierten Formats (gltf)**

![Optionen zum Herunterladen von "schrätchfab" mit hervorgehobenem Format](images/importing-models-img-02.png)

4. Öffnen Sie die [GLB Packer](https://glb-packer.glitch.me) -Website, und aktivieren Sie das Kontrollkästchen **PNG in JPEG konvertieren (Beta)** .
5. Deinstalkomprimieren Sie die heruntergeladenen gltf-Dateien, und ziehen Sie Sie nacheinander auf die Browser Registerkarte GLB Packer.

![Fenster mit unkomprimierung des Modells](images/importing-models-img-03.png)

6. Abhängig von der Anzahl und Größe der Dateien kann es eine Weile dauern, bis Sie verarbeitet wird. Wenn die Verarbeitung abgeschlossen ist, wird eine **out. GLB** -Datei heruntergeladen. Benennen Sie diese Datei in eine informative Datei um. Dies ist der Name des Objekts auf der Welt (z **. b. "Low Poly. GLB**").
7. Navigieren Sie zu [altvr.com > weitere > Modelle](https://account.altvr.com/users/sign_in) , und wählen Sie **Erstellen** aus.
8. Geben Sie den Speicherort der GLB-Datei an, und stellen Sie sicher, dass Sie den Link "schrätchfab" in die Beschreibung für die Zuordnung kopieren. Wenn Sie möchten, können Sie ein Vorschaubild angeben und dann **Modell erstellen** auswählen:

![Modell Vorschau in altspacevr](images/importing-models-img-04.png)

9. **In Zwischenablage kopieren** auswählen
10. Öffnen des **World Editors > altspace > Grundlagen > gltf**
11. Fügen Sie die URL ein, und wählen Sie **bestätigen** aus.

Herzlichen Glückwunsch! Sie haben soeben das erste Modell erzeugt.

## <a name="troubleshooting"></a>Problembehandlung

**Beim Anklicken **bestätigen** , dass nichts passiert ist**
    * Wir haben derzeit ein Polygon Limit von 100 KB. Wenn dies nicht möglich ist, löschen Sie das Objekt, um potenzielle Probleme mit Benutzern zu vermeiden, die ihrer Welt beitreten
    * Möglicherweise gibt es andere Probleme mit dem Asset. Versuchen Sie, Ressourcen mit möglichst wenigen Polygonen zu verwenden.
    * Das Modell, das Sie einbinden, kann klein oder groß sein. Versuchen Sie, die Skalierung zu vergrößern oder zu verringern oder den Avatar zu verschieben. möglicherweise sind Sie im Modell.

**Die Auslastung ist langsam** . Wie schnell andere Benutzer weltweit laden, hängt von der Verbindungsgeschwindigkeit ab. Sie wird auch nicht wie Kit-Assets zwischengespeichert. Wenn Sie einen in Ihrem Zuhause platzieren, können Sie das gleiche Modell jedes Mal erneut herunterladen, wenn Sie beitreten, was nicht gut ist.

**Es gibt keine Kollision** . Standardmäßig gibt es keine Konflikte mit den Objekten, die auf diese Weise eingeführt werden.

**Wenn ich Sie verwende, verliere ich meine Steuerelemente auf sechs DOF-Daten, oder ich bin darin, dass es schwierig ist, Sie zu bearbeiten** . Ja, wir kennen diese Probleme und hoffen, Sie bald zu beheben.  