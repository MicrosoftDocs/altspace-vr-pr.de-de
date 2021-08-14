---
title: Hochladen benutzerdefinierter Kits
description: Erfahren Sie, wie Sie Ihre eigenen benutzerdefinierten Kits in AltspaceVR einrichten, generieren und hochladen sowie Hilfe zur Problembehandlung erhalten.
ms.date: 03/11/2021
ms.topic: article
keywords: Kits, Hochladen, Problembehandlung
ms.openlocfilehash: 9a90bff2360d854dc398a35501f07cddcbce5c6c66ef8230f2e412a022f8aed0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125525"
---
# <a name="uploading-custom-kits"></a>Hochladen benutzerdefinierter Kits

Der World Editor verfügt über Kits, die Artifacts enthalten, die Sie in Ihrer Welt erstellen können. Beispielsweise verfügt das [Kits für die Feuersuche](https://account.altvr.com/kits/993516233267609824) über viele Arten von Strukturen– jeder Strukturtyp ist ein Artefakt. Um Ihr eigenes Kit zu erstellen, müssen Sie Unity AssetBundles erstellen und eine .zip-Datei mit einem Unity Prefab für jedes Artefakt hochladen und jedes Artefakt auf unserer Website registrieren. Glücklicherweise automatisiert der communitygesteuerte Unity Uploader den Großteil des Workflows. Nach dem Hochladen können Sie Objekte aus Ihren eigenen Kits in Ihrer Welt erstellen, und andere Benutzer können sie automatisch sehen. Später können Sie Ihr Kit für Ihre Freunde oder sogar für die gesamte Community freigeben, indem Sie es verwenden.

## <a name="prerequisites"></a>Voraussetzungen

1. [Installieren von Unity Hub und Unity](world-building-toolkit-getting-started.md)
2. Laden Sie die neueste Version des [Unity-Uploaders herunter.](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>Einrichten 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. Erstellen Eines Kits auf unserer Website unter [Worlds > Kits](https://account.altvr.com/kits)
2. Kopieren Sie die Kit-ID aus der Adressleiste Ihres Browsers in die Zwischenablage (dieser Schritt ist in Uploaderversionen 0.9 und höher einfacher)
3. Erstellen eines neuen Unity-Project
4. Importieren Sie den Unity-Uploader, indem Sie auf das Paket doppelklicken.

![Importiertes Unity-Uploaderpaket](images/custom-kits-img-01.png)

5. Melden Sie sich mit Ihrer Altspace-E-Mail-Adresse und Ihrem Kennwort beim Uploader an.

![AltspaceVR-Anmeldeschnittstelle in Unity](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>Generieren und Hochladen Ihres Kits

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. Geben Sie kit **folder name (Kit-Ordnername)** mit Ihrer Kit-ID als Präfix und einem Design (z. **B. 1137484494681408069_pirates)** und **kit asset name (Kit-Ressourcenname)** mit Ihrer Kit-ID als Präfix ein. Alle Ressourcen müssen über dieses Präfix verfügen.

![AltspaceVR-Schnittstelle in Unity mit Dem Namen des Kit-Ordners](images/custom-kits-img-03.png)

2. Für jedes Artefakt oder jede Gruppe von Artifacts:
* Ziehen Sie Ihre Quell-Prefab(s) auf die Registerkarte Hierarchie.
* Wählen Sie diejenigen aus, die Sie in eine Gruppe einschließen möchten, z. B. fünf Arten von Schlägen.
* Aktualisieren des **Kit-Medienobjektnamens** mit **"euro"**
* Wählen Sie **Convert GameObject(s) to Kit Prefab (GameObject(s) in Kit Prefab konvertieren aus.**
* Überprüfen Sie, ob neue Prefabs und Screenshots im Ordner Assets/Prefabs erstellt wurden.

![AltspaceVR-Schnittstelle in Unity mit ausgewählten Artefakten](images/custom-kits-img-04.png)

> [!NOTE]
> Wenn Sie Änderungen an einem generierten Prefab vornehmen möchten, ziehen Sie es zurück in die Hierarchie, nehmen Sie Änderungen vor, und klicken Sie dann auf der Registerkarte Inspektor auf **Übernehmen,** um das Prefab zu aktualisieren. 

3. Wenn Sie fertig sind, scrollen Sie auf der Registerkarte Uploader nach unten, und bereiten Sie sich darauf vor, eine ZIP-Datei mit dem Medienobjektpaket zu generieren.
4. Deaktivieren Sie das **Build Kit für Android,** um eine schnellere Iteration zu erzielen. Denken Sie daran, später eine Version für Android zu erstellen und hochzuladen, wenn Sie mit dem Iterieren fertig sind oder Ihr Kit freigeben/featureen möchten. 
5. Wählen Sie **Load Kit Prefab Directories (Prefab-Verzeichnisse** laden) aus.
6. Wählen  Sie Neben dem Build aus, der ihrem Kit-Ordnernamen entspricht. Es ist üblich, mehrere Kits aus dem gleichen Unity-Projekt zu erstellen. Dies kann je nach Größe Ihres Kits eine Weile dauern. Anschließend wird der Ordner, der Ihre ZIP-Datei enthält, automatisch geöffnet. 
7. Wechseln Sie zur Website, bearbeiten Sie das zuvor erstellte Kit, und laden Sie die zip-Datei hoch, die Sie erstellt haben. Dieser Upload kann je nach Dateigröße eine Weile dauern.
    * Wenn dies erfolgreich ist, werden auf der linken Seite unter "Uploads" die Dateigrößen und für PC und Android sowie deren zeitpunkt der letzten Aktualisierung angezeigt.
    * Wenn dies nicht erfolgreich ist, stellen Sie sicher, dass Sie keine Skripts haben, wir unterstützen keine Skripts. Wir überprüfen diese auf Sicherheit, und versuchen Sie es erneut.

Herzlichen Glückwunsch! Sie sind bereit, Worlds mit Ihrem eigenen Kit zu erstellen!

## <a name="troubleshooting"></a>Problembehandlung 

**Gibt es Grenzwerte?**
Es gibt noch keine harte Grenze, aber denken Sie daran, dass Benutzer das AssetBundle für ihre Plattform für das gesamte Kit herunterladen müssen, auch wenn nur ein Artefakt verwendet wird. Versuchen Sie, den Download pro Plattform auf 5 MB oder weniger zu halten. Eine Möglichkeit besteht darin, die Dinge in kleinere Kits aufzuteilen. Beispielsweise sollten 200 Props halbiert werden. 

**Sehen Sie "Split Eye"?**
Importieren Sie den neuesten Uploader erneut, um die richtigen Renderingeinstellungen zu erhalten.

**Updates/Änderungen werden nicht widergespiegelt?**
    * Überprüfen der aktualisierten Zeit auf der Kit-Seite
    * Das erneute Starten der Welt funktioniert nicht: Starten Sie den Client neu. Selbst dann kann es einige Minuten dauern, bis das Update erfolgt.
    * Stellen Sie sicher, dass ihre Ordnernamen oder Prefabnamen keine Leerzeichen **enthalten, z. B. "party_favors" oder "Parteivorlieben".**

**Es wird immer wieder gesagt, dass ich ein Skript habe, aber nicht** Der AssetBundle-Browser enthält manchmal automatisch Dateien. Versuchen Sie, das modell, das Sie einbringen, zu isolieren. Ziehen Sie es beispielsweise nicht ein, wenn es bereits Teil eines anderen Prefab ist.

**Was ist mit Partikelsystemen und Animationen?**
Für diese werden sie als Nächstes unter einem 1x1x1-Cube am Ursprung positioniert, wobei Mesh Rendering und Collision deaktiviert sind. Für Partikelsysteme sollte Schleifen aktiviert sein, und **die Skalierung** sollte auf **Hierarchy** festgelegt werden, damit sie in Altspace ordnungsgemäß skaliert werden können. Nachdem Sie die Prefabs für alle Animationen generiert haben, deaktivieren Sie die Konflikte für die **einzelnen Kollisionsobjekte.**

**Die Artifacts sind dunkel** Haben Sie den Material-Shader des Modells auf **"Mobile/Vertex lit-only directional lights"** festgelegt?

**Das Artefakt ist nicht auf die richtige Weise zu sehen.** Drehen Sie das **Modell** und **den Collider,** und aktualisieren Sie das Prefab. Das Rotieren des übergeordneten Elements wird ignoriert. Sie können dazu das Feld **Rotationsüberschreibung** verwenden.

**Können diese Artifacts mit der **CreateFromLibrary-Funktion** des SDK verwendet werden?**
Ja