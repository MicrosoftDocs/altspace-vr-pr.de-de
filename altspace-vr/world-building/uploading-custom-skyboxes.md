---
title: Hochladen benutzerdefinierter Skyboxes
description: Hier finden Sie Schritt-für-Schritt-Anweisungen zum Hochladen und Behandeln von Problemen mit ihren benutzerdefinierten Skyboxes in AltspaceVR-Funktionen.
ms.date: 03/11/2021
ms.topic: article
keywords: Skyboxes, Problembehandlung
ms.openlocfilehash: 912df5a4c87b7a5817824c6ee75ec8707439636b83b4d46996bbc4129ee6e9de
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126792"
---
# <a name="uploading-custom-skyboxes"></a>Hochladen benutzerdefinierter Skyboxes

Eine Skybox ist eine Möglichkeit, einen Hintergrund **für** Ihre Welt zu erstellen, der die Umgebung immersiver macht. Es gibt verschiedene Arten von Skyboxes, aber wir unterstützen derzeit **equirectangular**. Hier ist ein Beispiel mit einer 360-Kamera (weitere Beispiele finden Sie [hier):](http://moments.mankindforward.com/) 

![360 equirectangular view of a living room](images/custom-skyboxes-img-01.jpeg)

Sie können auch den [Unity-Uploader verwenden,](world-building-toolkit-getting-started.md) aber dieser Ansatz ist einfacher.

1. Navigieren Sie [zu Worlds > Skyboxes,](https://account.altvr.com/skyboxes) und klicken **Sie** rechts auf die Schaltfläche Erstellen.

![Worlds-Websiteseite im Skyboxes-Bereich geöffnet](images/custom-skyboxes-img-02.png)

2. Geben Sie einen Namen ein, und geben Sie Ihr 360-Bild an. Es muss kein Foto sein, es gibt Programme, mit denen Sie Ihr eigenes zeichnen können, oder Sie können online nach suchen. Wählen Sie **Erstellen** aus, wenn Sie fertig sind. 

![Skybox-Erstellungsformular](images/custom-skyboxes-img-03.png)

3. Sie können optional ein Vorschaubild **hochladen,** damit Sie dieses Skybox-Image leicht identifizieren können. Sie können auch Ambient-Audio im WAV-Format hochladen. 

> [!IMPORTANT]
> Es wird empfohlen, Vorschaubilder und Ambient-Audio separat hochzuladen, nachdem Sie das 360-Bild hochgeladen haben. Wenn Sie sie zusammen hochladen, können die Dateigrößen groß genug sein, um den Prozess zu beschleunigen. [Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) ist ein gutes Beispiel für die Verwendung einer Skybox mit Umgebungsaudio. Beachten Sie, dass der World-Builder die Audiomenge niedrig gehalten hat, und Töne, die Sie hören, sporadisch sind, damit die Menschen nicht verärgert werden. 

4. Geben Sie Ihre Welt ein, und öffnen Sie den World Editor. Wählen Sie unter Skyboxes Ihre neue Skybox aus. In wenigen Sekunden ändert sich der Himmel wörtlich. Andere in Ihrer Welt werden auch den Himmel verändern. Um zurück zu wechseln, wählen Sie die **Standard-Skybox** in derselben Liste aus. 

## <a name="troubleshooting"></a>Problembehandlung

**Am Himmel ist eine Naht oder Linie :-(.** Es ist ein Fehler, den wir bald beheben werden.

**Hochladen fehlgeschlagen**
    * Versuchen Sie, nur das 360-Image selbst hochzuladen.
    * Testen mit einer anderen, kleineren Datei als Test

**Ich kann kein 360-Foto finden.**
    * Dies ist eine gute Quelle (ändern Sie die Filter, um nach creativen Gängigen zu suchen).
    * Nehmen Sie Ihre eigenen! Die Kameras von Ricoh waren erfolgreich. 
**Der Himmel sieht strichend oder blockierend aus** Möglicherweise müssen Sie ein Image mit höherer Auflösung suchen. In der Regel ca. 2–5 MB und ~5.000 px x 2.000 px

**Das schadet der Bildrate meiner Welt!**
Das Bild ist wahrscheinlich zu groß. Einige generierte Skyboxes können 8.000 sein. Sie sind in der Regel mit 2K-Versionen für Mobilgeräte erhältlich. Verwenden Sie dies.

**Hilfe bei der Umgebungsaudiodatei**
    * Verwenden Sie kostenlose Software wie Audacity, um das Volume zu senken oder eigene Schleifen zu erstellen. Denken Sie daran, dass die Audiodaten wiederholt und in den Lästchen der Menschen abspielt werden, damit sie niedrig und nicht lästig bleiben.
    * [Free Sound](https://freesound.org/) ist eine gute Quelle für tstgebührenfreie Sounds.
