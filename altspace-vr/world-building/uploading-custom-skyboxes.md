---
title: Hochladen benutzerdefinierter Skyboxes
description: Hier finden Sie schrittweise Anweisungen zum Hochladen und Beheben von Problemen mit Ihren benutzerdefinierten Skyboxes in AltspaceVR-Funktionen.
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

Eine Skybox ist eine Möglichkeit, einen **Hintergrund** für Ihre Welt zu erstellen, der die Erfahrung immersiver macht. Es gibt verschiedene Arten von Skyboxes, aber wir unterstützen derzeit **equirectangular**. Hier sehen Sie ein Beispiel, das mit einer 360-Kamera aufgenommen wurde (weitere Beispiele [finden Sie hier):](http://moments.mankindforward.com/) 

![360 äquirectangulare Ansicht eines Raums](images/custom-skyboxes-img-01.jpeg)

Sie können auch den [Unity-Uploader](world-building-toolkit-getting-started.md) verwenden, aber dieser Ansatz ist einfacher.

1. Navigieren Sie zu [Worlds > Skyboxes,](https://account.altvr.com/skyboxes) und klicken Sie auf der rechten Seite auf die Schaltfläche **Erstellen.**

![Seite der Worlds-Website, die im Bereich "Skyboxes" geöffnet ist](images/custom-skyboxes-img-02.png)

2. Geben Sie einen Namen ein, und geben Sie Ihr 360-Image an. Es muss kein Foto sein, es gibt Programme, mit denen Sie Eigenes zeichnen können, oder Sie können online nach etwas suchen. Wählen Sie **Erstellen** aus, wenn Sie fertig sind. 

![Skybox-Erstellungsformular](images/custom-skyboxes-img-03.png)

3. Sie können optional ein **Vorschaubild** hochladen, damit Sie diese Skybox leicht identifizieren können. Sie können auch Ambient-Audio im WAV-Format hochladen. 

> [!IMPORTANT]
> Es wird empfohlen, Vorschaubilder und Ambient-Audio separat hochzuladen, nachdem Sie das 360-Bild hochgeladen haben. Wenn Sie sie zusammen hochladen, können die Dateigrößen groß genug sein, um den Prozess zu halten. [Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) ist ein gutes Beispiel für die Verwendung einer Skybox mit Ambient-Audio. Beachten Sie, dass der World-Builder die Audiolautstärke niedrig gehalten hat und dass die hörenden Töne sporadisch sind, sodass die Benutzer nicht verärgert werden. 

4. Geben Sie Ihre Welt ein, und öffnen Sie den World Editor. Wählen Sie unter Skyboxes Ihre neue Skybox aus. In wenigen Sekunden ändert sich der Himmel. Für andere Personen in Ihrer Welt ändert sich auch der Himmel. Um zurückzuwechseln, wählen Sie das Standard-Skybox-Feld in derselben Liste aus.  

## <a name="troubleshooting"></a>Problembehandlung

**Es gibt eine Naht oder Linie am Sky :-(.** Es ist ein Fehler, den wir in Kürze beheben werden.

**Fehler bei Hochladen**
    * Versuchen Sie, nur das 360-Image selbst hochzuladen.
    * Testen mit einer anderen, kleineren Datei als Test

**Ich kann kein 360-Foto finden**
    * Flickr ist eine gute Quelle (ändern Sie die Filter, um nach creativen commons-Filtern zu suchen).
    * Nehmen Sie Ihre eigenen! Die Kamera von Ricoh war erfolgreich. 
**Der Sky sieht granular oder blockig aus.** Möglicherweise müssen Sie ein Bild mit höherer Auflösung finden. In der Regel ca. 2–5 MB und ca. 5.000 px x 2.000 px

**Das verletzt die Framerate meiner Welt!**
Das Bild ist wahrscheinlich zu groß. Einige generierte Skyboxes können 8 KB sein. Sie verfügen in der Regel über 2K-Versionen, die für Mobilgeräte geeignet sind. Verwenden Sie dies.

**Hilfe bei der Umgebungsaudio**
    * Verwenden Sie kostenlose Software wie Audacity, um das Volume zu verringern oder eigene Schleifen zu erstellen. Denken Sie daran, dass die Audiodaten wiederholt werden und in den Augen der Menschen wiedergegeben werden, sodass sie niedrig und nicht mühsam bleiben.
    * [Free Sound](https://freesound.org/) ist eine gute Quelle für lizenzfreie Sounds.
