---
title: Hochladen benutzerdefinierter Kits
description: Erfahren Sie, wie Sie Ihre eigenen benutzerdefinierten Kits in AltspaceVR einrichten, generieren und hochladen sowie Hilfe zur Problembehandlung.
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

Der World Editor enthält Kits mit Artifacts, die Sie in Ihrer Welt erstellen können. Zum Beispiel verfügt das [Kits von Dennfire über](https://account.altvr.com/kits/993516233267609824) viele Arten von Strukturen– jeder Baumtyp ist ein Artefakt. Um Ihr eigenes Kit zu erstellen, müssen Sie Unity AssetBundles erstellen und eine .zip-Datei hochladen, die ein Unity Prefab für jedes Artefakt enthält, und jedes Artefakt auf unserer Website registrieren. Glücklicherweise automatisiert der communitygesteuerte Unity Uploader den Großteil des Workflows. Nach dem Hochladen können Sie Objekte aus Ihren eigenen Kits in Ihrer Welt erstellen, und andere Benutzer können sie automatisch sehen. Später können Sie Ihr Kit mit Ihren Freunden oder sogar mit der gesamten Community teilen, indem Sie vorgestellt werden.

## <a name="prerequisites"></a>Voraussetzungen

1. [Installieren von Unity Hub und Unity](world-building-toolkit-getting-started.md)
2. Herunterladen der neuesten Version von [Unity Uploader](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>Setup 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. Erstellen eines Kits auf unserer Website unter [Worlds > Kits](https://account.altvr.com/kits)
2. Kopieren Sie die Kit-ID aus der Adressleiste Ihres Browsers in die Zwischenablage (dieser Schritt ist in Uploaderversionen ab 0.9 einfacher).
3. Erstellen eines neuen Unity-Project
4. Importieren des Unity-Uploaders durch Doppelklicken auf das Paket

![Importiertes Unity-Uploaderpaket](images/custom-kits-img-01.png)

5. Melden Sie sich mit Ihrer ALTSPACE-E-Mail-Adresse und Ihrem Kennwort beim Uploader an.

![AltspaceVR-Anmeldeschnittstelle in Unity](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>Generieren und Hochladen Ihres Kits

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. Geben Sie **kit folder name** (Kitordnername) mit Ihrer Kit-ID als Präfix und einem Design (z.B. **1137484494681408069_pirates)** ein, und geben Sie kit **asset name (Kit-Ressourcenname)** mit Ihrer Kit-ID als Präfix ein. Alle Ressourcen müssen über dieses Präfix verfügen.

![AltspaceVR-Schnittstelle in Unity mit Kit-Ordnername](images/custom-kits-img-03.png)

2. Für jedes Artefakt oder jede Gruppe von Artifacts:
* Ziehen Sie ihre Quell-Prefab(s) auf die Registerkarte Hierarchie.
* Wählen Sie diejenigen aus, die Sie in eine Gruppe einordnen möchten, z. B. fünf Arten von Läufen.
* Aktualisieren des **Kit-Ressourcennamens** mit **"besen"**
* Wählen **Sie Convert GameObject(s) to Kit Prefab (GameObject(s) in Kit Prefab konvertieren aus.**
* Überprüfen Sie, ob neue Prefabs und Screenshots im Ordner Assets/Prefabs erstellt wurden.

![AltspaceVR-Schnittstelle in Unity mit ausgewählten Artefakten](images/custom-kits-img-04.png)

> [!NOTE]
> Wenn Sie Änderungen an einem generierten Prefab vornehmen möchten, ziehen Sie es zurück  in die Hierarchie, nehmen Sie Änderungen vor, und klicken Sie dann auf der Registerkarte Inspektor auf Übernehmen, um das Prefab zu aktualisieren. 

3. Wenn Sie bereit sind, scrollen Sie auf der Registerkarte Uploader nach unten, und bereiten Wir uns darauf vor, eine ZIP-Datei mit dem Asset Bundle zu generieren.
4. Deaktivieren Sie das Build Kit für Android, um eine schnellere **Iteration zu erreichen.** Denken Sie daran, später eine Version für Android zu erstellen und hochzuladen, wenn Sie mit dem Iterieren fertig sind oder Ihr Kit freigeben/nutzen möchten. 
5. Wählen **Sie Load Kit Prefab Directories (Prefab-Verzeichnisse laden) aus.**
6. Klicken **Sie neben dem** Namen Ihres Kitordners auf Erstellen. Es ist üblich, mehrere Kits aus demselben Unity-Projekt zu erstellen. Dies kann je nach Größe Ihres Kits eine Weile dauern. Wenn sie fertig ist, wird der Ordner, der Ihre ZIP-Datei enthält, automatisch geöffnet. 
7. Wechseln Sie zur Website, bearbeiten Sie das kit, das Sie zuvor erstellt haben, und laden Sie die von Ihnen erstellte ZIP-Datei hoch. Dieser Upload kann je nach Dateigröße eine Weile dauern.
    * Wenn dies erfolgreich war, sehen Sie auf der linken Seite unter "Uploads" die Dateigrößen und für PC und Android und wann sie zuletzt aktualisiert wurden.
    * Wenn dies nicht erfolgreich ist, stellen Sie sicher, dass Sie keine Skripts haben, wir unterstützen keine Skripts. Wir überprüfen diese auf Sicherheit und versuchen es erneut.

Glückwunsch! Sie sind bereit, Worlds mit Ihrem eigenen Kit zu erstellen!

## <a name="troubleshooting"></a>Problembehandlung 

**Gibt es Grenzwerte?**
Es gibt noch keine harte Grenze, aber denken Sie daran, dass Benutzer das AssetBundle für ihre Plattform für das gesamte Kit herunterladen müssen, auch wenn nur ein Artefakt verwendet wird. Versuchen Sie, den Download pro Plattform auf 5 MB oder weniger zu halten. Eine Möglichkeit, dies zu tun, besteht in der Aufteilung in kleinere Kits. Beispielsweise sollten 200 Props in die Hälfte aufgeteilt werden. 

**Sehen Sie "Geteiltes Auge"?**
Importieren Sie den neuesten Uploader erneut, um die richtigen Renderingeinstellungen zu erhalten.

**Updates/Änderungen werden nicht widergespiegelt?**
    * Überprüfen der aktualisierten Zeit auf der Seite "Kit"
    * Das erneute Starten der Welt funktioniert nicht– starten Sie den Client neu. Selbst dann kann es einige Minuten dauern, bis das Update
    * Stellen Sie sicher, dass ihre Ordnernamen oder Prefabnamen keine Leerzeichen enthalten, z. B. "party_favors" im Vergleich zu **"Parteivorzug".**

**Es wird immer wieder gesagt, dass ich über ein Skript versinge, aber nicht.** Der AssetBundle-Browser schließt manchmal automatisch Dateien ein. Versuchen Sie, das Modell zu isolieren, das Sie verwenden. Ziehen Sie sie z. B. nicht ein, wenn sie bereits Teil eines anderen Prefab ist.

**Wie sieht es mit Partikelsystemen und Animationen aus?**
Für diese werden sie als Nächstes unter einem 1x1x1-Cube am Ursprung positioniert, bei dem Mesh Rendering und Collision deaktiviert sind. Für Partikelsysteme sollte Schleifen aktiviert sein, und **die Skalierung** sollte auf **Hierarchie** festgelegt werden, damit sie im Altspace ordnungsgemäß skaliert werden können. Nachdem Sie die Prefabs für alle Animationen generiert  haben, deaktivieren Sie die Kollisionen der Kollisionsobjekte für jede.

**Die Artifacts sind dunkel** Haben Sie den Material-Shader des Modells auf **Mobile/Vertex lit-only directional lights festgelegt?**

**Das Artefakt ist nicht auf die richtige Weise ausgerichtet.** Drehen Sie das **Modell und** **den Collider,** und aktualisieren Sie das Prefab. Das Rotieren des übergeordneten Elements hat nichts, was ignoriert wird. Hierzu können Sie das Feld **Rotation Override (Rotationsüberschreibung)** verwenden.

**Können diese Artifacts mit der **CreateFromLibrary-Funktion** des SDK verwendet werden?**
Ja