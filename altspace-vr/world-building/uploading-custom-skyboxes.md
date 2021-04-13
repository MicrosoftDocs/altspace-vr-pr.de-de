---
title: Hochladen von benutzerdefinierten Skyboxes
description: Hier finden Sie Schritt-für-Schritt-Anleitungen zum Hochladen und behandeln von benutzerdefinierten Skyboxes-Vorgängen in altspacevr.
ms.date: 03/11/2021
ms.topic: article
keywords: Skyboxes, Problembehandlung
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213262"
---
# <a name="uploading-custom-skyboxes"></a>Hochladen von benutzerdefinierten Skyboxes

Eine Skybox ist eine Möglichkeit, einen **Hintergrund** für Ihre Welt zu erstellen, der die Erfahrung verbessert. Es gibt unterschiedliche Arten von Skyboxes, aber wir unterstützen derzeit **equirecht eckige** Felder. Hier sehen Sie ein Beispiel mit einer 360-Kamera (Weitere Beispiele [finden Sie hier](http://moments.mankindforward.com/)): 

![360 equirecht eckige Ansicht eines Wohnraums](images/custom-skyboxes-img-01.jpeg)

Sie können auch das [Unity-Uploader](world-building-toolkit-getting-started.md) verwenden, aber dieser Ansatz ist einfacher.

1. Navigieren Sie zu [Worlds > Skyboxes](https://account.altvr.com/skyboxes) , und klicken Sie auf der rechten Seite auf die Schaltfläche **Erstellen**

![Die Seite "Website" ist für das Skyboxes-Panel](images/custom-skyboxes-img-02.png)

2. Geben Sie einen Namen ein, und geben Sie Ihr 360-Image an. Es muss kein Foto sein, es gibt Programme, mit denen Sie Ihre eigenen erstellen können, oder Sie können nach einigen Online suchen. Wählen Sie **Erstellen** aus, wenn Sie fertig sind. 

![Erstellungs Formular für Skybox](images/custom-skyboxes-img-03.png)

3. Optional können Sie ein **Vorschaubild** hochladen, damit Sie diese Skybox problemlos identifizieren können. Sie können Ambient-Audiodaten auch im WAV-Format hochladen. 

> [!IMPORTANT]
> Es wird empfohlen, Vorschau Bilder und Ambient-Audiodaten separat hochzuladen, nachdem Sie das 360-Image hochgeladen haben. Wenn Sie Sie hochladen, können die Dateigrößen groß genug sein, um den Prozess zu stoppen. [Jegsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) ist ein gutes Beispiel für die Verwendung von Skybox mit Ambient-Audiodaten. Beachten Sie, dass der Welt-Generator das audiovolume niedrig gehalten hat, und Klänge, die Sie hören, sind sporadisch, damit Menschen nicht verärgert werden. 

4. Geben Sie Ihre Welt ein, und öffnen Sie den World-Editor. Wählen Sie unter Skyboxes die neue Skybox aus. Innerhalb weniger Sekunden wird der Himmel buchstäblich geändert. Andere Benutzer in ihrer Welt sehen auch die Änderung am Himmel. Um zurückzukehren, wählen Sie die **Standard** -Skybox in der gleichen Liste aus. 

## <a name="troubleshooting"></a>Problembehandlung

**Es gibt eine Naht oder eine Linie im Himmel:-(.** Es handelt sich um einen Fehler, den wir bald beheben werden.

**Fehler beim Hochladen.**
    * versuchen Sie, nur das 360-Image eigenständig hochzuladen.
    * versuchen Sie es mit einer anderen, kleineren Datei als Test.

**Ich kann ein 360-Foto nicht finden.**
    * Flickr ist eine gute Quelle (ändern Sie die Filter, um Creative Commons zu finden)
    * Nehmen Sie Ihre eigenen! Die Kameras von Ricoh waren erfolgreich. 
**Der Himmel sieht grau oder grobe aus** . Möglicherweise müssen Sie ein Bild mit höherer Auflösung suchen. Üblicherweise ca. 2-5 MB und ~ 5000 px x 2000 px

**Die Framerate meiner Welt!**
Das Image ist wahrscheinlich zu groß. Einige generierte Skyboxes können 8 KB betragen. Sie sind in der Regel mit Mobil funkfreundlichen 2K-Versionen ausgestattet. verwenden Sie diese Version.

**Hilfe bei der Ambient-Audiodatei**
    * Verwenden Sie die kostenlose Software, wie z. b. Audacity, um das Volume zu verringern oder eigene Schleifen Denken Sie daran, dass das Audiomaterial wiederholt wird und in den Ohren der Menschen wiedergegeben wird.
    * Der [freie Sound](https://freesound.org/) ist eine gute Quelle für kostenlose Sounds.
