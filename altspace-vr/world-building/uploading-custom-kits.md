---
title: Hochladen von benutzerdefinierten Kits
description: Erfahren Sie, wie Sie eigene benutzerdefinierte Kits in altspacevr einrichten, generieren und hochladen sowie Hilfe zur Problembehandlung erhalten.
ms.date: 03/11/2021
ms.topic: article
keywords: Kits, Upload, Problembehandlung
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213507"
---
# <a name="uploading-custom-kits"></a>Hochladen von benutzerdefinierten Kits

Der Welt-Editor verfügt über Kits, die Artefakte enthalten, die Sie in ihrer Welt erzeugen können. Beispielsweise hat das [Lager Lager-Kit](https://account.altvr.com/kits/993516233267609824) viele Arten von Strukturen, wobei jeder Typ von Tree ein Element ist. Zum Erstellen eines eigenen Kits müssen Sie Unity assetbundles erstellen und eine ZIP-Datei hochladen, die eine Unity-vorfab für jedes Element enthält, und jedes Element auf unserer Website registrieren. Glücklicherweise automatisiert der Community-gesteuerte Unity-Uploader den größten Teil des Workflows. Nach dem Hochladen können Sie Objekte aus ihren eigenen Kits in ihrer Welt erzeugen, und andere Benutzer können diese automatisch sehen. Später können Sie Ihr Kit für Ihre Freunde oder sogar für die gesamte Community freigeben.

## <a name="prerequisites"></a>Voraussetzungen

1. [Installieren von Unity-Hub und Unity](world-building-toolkit-getting-started.md)
2. Herunterladen der neuesten Version des [Unity-Uploader](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>Einrichten 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. Erstellen eines Kits auf unserer Website in den [Welten > Kits](https://account.altvr.com/kits)
2. Kopieren Sie die Kit-ID aus der Adressleiste Ihres Browsers in die Zwischenablage (dieser Schritt ist in den Uploader-Versionen 0.9 und höher einfacher).
3. Erstellen eines neuen Unity-Projekts
4. Importieren des Unity-Uploader durch Doppelklicken auf das Paket

![Importiertes Unity-Uploader-Paket](images/custom-kits-img-01.png)

5. Anmelden beim Uploader mit ihrer altspace-e-Mail

![Altspacevr-Anmelde Schnittstelle in Unity](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>Generieren und Hochladen des Kits

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. Geben Sie den **Namen des Kit-Ordners** mit ihrer Kit-ID als Präfix und ein Design (z. b. **1137484494681408069_pirates**) ein, und geben Sie den **Kit Asset Name** mit ihrer Kit-ID als Präfix ein. Alle Assets müssen über dieses Präfix verfügen.

![Altspacevr-Schnittstelle in Unity mit dem Kit-Ordnernamen](images/custom-kits-img-03.png)

2. Für jedes Artefakt oder jeden Satz von Artefakten:
* Ziehen Sie die Quell präfab auf die Registerkarte Hierarchie.
* Wählen Sie die Gruppen aus, die Sie in eine Menge einschließen möchten, beispielsweise fünf Arten von Fässern.
* Aktualisieren des **Kit-Asset-namens** mit " **Barrel** "
* Wählen Sie **gameobject (e) in Kit Prefab konvertieren** aus.
* Vergewissern Sie sich, dass im Ordner "Assets/Prefabs" neue präfabs und Screenshots erstellt wurden.

![Altspacevr-Schnittstelle in Unity mit ausgewählten Artefakten](images/custom-kits-img-04.png)

> [!NOTE]
> Wenn Sie Änderungen an einer generierten vorfab vornehmen möchten, ziehen Sie Sie zurück in die Hierarchie, nehmen Sie Änderungen vor, und klicken Sie dann auf der Registerkarte Inspektor auf **anwenden** , um die vorfab zu aktualisieren. 

3. Wenn Sie bereit sind, führen Sie einen Bildlauf nach unten auf der Uploader-Registerkarte aus, und bereiten Sie die Generierung einer ZIP-Datei mit dem Asset
4. Deaktivieren Sie für eine schnellere Iterationen das **Build-Kit für Android?**. Denken Sie daran, eine Version für Android zu einem späteren Zeitpunkt zu erstellen und hochzuladen, wenn Sie die Iteration abgeschlossen haben oder das Kit freigeben bzw. Feature nutzen möchten 
5. Aktivieren der **Prefab-Verzeichnisse für Load Kit**
6. Wählen Sie **Build** neben dem Ordner aus, der dem Namen des Kit-Ordners entspricht. Es ist üblich, mehrere Kits aus demselben Unity-Projekt zu entwickeln. Dies kann je nach Größe Ihres Kits einige Zeit in Anspruch nehmen. Wenn dies der Fall ist, wird der Ordner, der die ZIP-Datei enthält, automatisch geöffnet. 
7. Wechseln Sie zur Website, bearbeiten Sie das Kit, das Sie zuvor erstellt haben, und laden Sie die erstellte ZIP-Datei hoch. Der Upload kann je nach Dateigröße einige Zeit in Anspruch nehmen.
    * Wenn der Vorgang erfolgreich ist, wird auf der linken Seite unter "Uploads" die Dateigrößen und für PC und Android und Zeitpunkt der letzten Aktualisierung angezeigt.
    * Wenn Sie nicht erfolgreich sind, stellen Sie sicher, dass Sie keine Skripts haben, wir unterstützen keine Skripts, überprüfen Sie die Sicherheit, und versuchen Sie es erneut

Glückwunsch! Sie sind bereit, mit Ihrem eigenen Kit Welten zu erstellen!

## <a name="troubleshooting"></a>Problembehandlung 

**Gibt es Einschränkungen?**
Es gibt noch keine festen Grenzwerte, aber denken Sie daran, dass Benutzer das assetbundle für Ihre Plattform für das gesamte Kit herunterladen müssen, auch wenn nur ein Element verwendet wird. Versuchen Sie, den Download pro Plattform auf 5 MB oder weniger zu beschränken. Eine Möglichkeit besteht darin, Dinge in kleinere Kits aufzuteilen. 200-Eigenschaften sollten z. b. in der Hälfte aufgeteilt werden. 

**Sehen Sie "Split Eye"?**
Neuimportieren des neuesten Uploader-Vorgangs, um die richtigen renderingeinstellungen zu erhalten

**Updates/Änderungen werden nicht widergespiegelt?**
    * Überprüfen Sie die aktualisierte Zeit auf der Kit-Seite.
    * Das erneute Eingeben der Welt funktioniert nicht--Client neu starten. Auch dann kann es einige Minuten dauern, bis die Aktualisierung abgeschlossen ist.
    * Stellen Sie sicher, dass keine Leerzeichen in den Ordnernamen oder präfab-Namen enthalten sind, z. b. **"party_favors" und "Partei begünstigt"** .

**Das heißt, ich habe ein Skript, aber ich habe es nicht** Der assetbundle-Browser schließt manchmal automatisch Dateien ein. Versuchen Sie, das Modell zu isolieren, das Sie einbinden. Ziehen Sie diese z. b. nicht in den, wenn Sie bereits Teil einer anderen Prefab ist.

**Wie sieht es mit Partikelsystemen und Animationen aus?**
Anschließend werden diese unter einem 1x1x1-Cube am Ursprung positioniert, wobei das Gitter Rendering und die Kollision deaktiviert sind. Für Partikelsysteme sollten Schleifen aktiviert sein, und die **Skalierung** sollte auf **Hierarchie** festgelegt werden, damit wir Sie ordnungsgemäß in altspace skalieren können. Nachdem Sie die Prefabs für alle Animationen generiert haben, deaktivieren Sie die Konflikte bei den **Kollisions** Objekten für jeden.

**Die Artefakte sind dunkel** Haben Sie den materialshader des Modells auf das **nur-Text-direktionale/Scheitel** Punkt Diagramm festgelegt?

**Das Element ist nicht auf die richtige Weise** sichtbar. Drehen Sie das **Modell** , und **kollidieren** Sie, und aktualisieren Sie die vorfab. Wenn Sie das übergeordnete Element drehen, wird nichts Unternehmen, das ignoriert wird. Sie können das Feld " **Rotation override** " verwenden, um dies zu erreichen.

**Können diese Artefakte mit **der Funktion "** -Funktion von SDK" verwendet werden?**
Ja