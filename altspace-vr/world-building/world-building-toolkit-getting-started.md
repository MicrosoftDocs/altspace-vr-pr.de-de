---
title: Einführung in das World Building Toolkit
description: Erfahren Sie, wie Sie Ihre altspacevr-Welten mithilfe von Unity-Szenen Vorlagen mit dem World Building Toolkit einrichten und hochladen.
ms.date: 03/11/2021
ms.topic: article
keywords: ations
ms.openlocfilehash: cf4660f46d93ca5c5f23de3f567ff04b12519617
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212114"
---
# <a name="introducing-the-world-building-toolkit"></a>Einführung in das World Building Toolkit

> [!NOTE]
> Das World Building Toolkit ist ein Communityprojekt, das von unserem tollen Freund, [Anthony Madden](https://twitter.com/chigamesstudio), mit Unterstützung von uns ausgeführt wird. Wenn Sie interessiert sind, treten Sie der [offiziellen altspacevr-Zwietracht](https://discordapp.com/invite/altspacevr) bei, und besuchen Sie den #World bauchannel. Zurzeit haben wir eine Mac-Testversion mit [weiteren Details](https://altvr.com/altspacevr-mac) .

Mit dem Uploader können Sie eine Unity-Szene als Vorlage für ihre Welten verwenden. Sie können ein heimgesuchte Haus für Halloween oder Ihre bevorzugte Erstellung aus minecraft einbringen. Wenn Sie Sie in Unity importieren können, können Sie diese auf diese Weise in altspace erhalten. Im folgenden finden Sie einige [Beispiel Welten](https://account.altvr.com/worlds/1046572460192825569).

![Beispiel Welten](images/unity-uploader-img-01.png)

## <a name="setup"></a>Einrichten

1. Treten Sie der [offiziellen altspacevr-Zwietracht](https://discordapp.com/invite/altspacevr) bei, und besuchen Sie die #World Building Channel-friends lassen Sie Freunde nicht allein erstellen.
2. Informationen zu den Grundlagen finden Sie unter Einführung in die ersten Schritte der [Welt](world-building-getting-started.md) .
3. [Installieren](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) Sie den Unity-Hub, und installieren Sie **Unity 2019.4.2 F1**. Das Uploader funktioniert nicht, es sei denn, Sie passen diese Version genau an. Sie benötigen ein kostenloses Unity-Konto, wenn Sie noch nicht über ein Konto verfügen, und wählen Sie " **persönlich** ", da Sie dies für Spaß machen! Vergewissern Sie sich bei der Installation, dass Sie die Option **Android Builds** aktivieren und die automatische Aktualisierung deaktivieren.
4. [Herunterladen des aktuellen Unity-Uploader](https://aka.ms/AsvrCommunityUploader)
5. Erstellen Sie auf unserer Website [eine Vorlage](https://account.altvr.com/space_templates/new) . Nennen Sie Sie **Hallo Welt Vorlage**.
6. [Erstellen Sie eine Welt](https://account.altvr.com/worlds/my) , und benennen Sie Sie **Hallo Welt**. Wählen Sie **Hallo Welt Vorlage** als Vorlage aus.

![Bildschirm "erstellt"](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Hochladen der Szene

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Öffnen Sie den Unity-Hub, und erstellen Sie ein neues Unity 2019.4.2 F1-Projekt.
2. Wenn Ihr Projekt geöffnet ist, importieren Sie das Uploader, indem Sie auf die Datei doppelklicken, die Sie heruntergeladen haben (es ist ein Unity-Paket). Nun sollte eine neue Registerkarte mit dem Namen " **altspacevr**" angezeigt werden. Sie müssen das Paket für jedes Unity-Projekt importieren, das Sie mit "altspace" verwenden möchten.
3. **Menü öffnen > altspacevr > Buildeinstellungen**
4. Mit ihren altspace-Konto Anmelde Informationen anmelden
5. Wählen Sie **Vorlagen laden** und dann **Hallo Welt Vorlage** aus.
6. Fügen Sie Ihrer Szene einen Cube hinzu, und speichern Sie Sie.
7. Überprüfen Sie **Build für Windows?** , und deaktivieren Sie **Build für Android?**
8. Klicken Sie auf **Hochladen**. In ungefähr einer Minute sollte " **Upload** Complete" angezeigt werden.
9. Verknüpfen Sie **Hallo Welt** , indem Sie altspace starten und aus dem **Menü > Welten > meine Welten** wechseln.
10. Die Welt wird aus dem **Menü > Einstellungen > mittleren > zurückgesetzt** .
11. Der Cube sollte angezeigt werden. Wenn Sie dies schnell wie im obigen Video tun, sehen Sie Änderungen innerhalb von nur 10 Sekunden.

## <a name="whats-supported"></a>Unterstützte Funktionen

* Ja: Modelle, Kollisionen, Animationen, Partikeleffekte, Audiodaten, Skyboxes usw.
* Nein: Skripts. Aus Sicherheitsgründen werden Uploads, die Skripts enthalten, zurückgewiesen.
* Vielleicht: praktische Dinge wie dynamische globale Beleuchtung
* Hintergrund-oder zusammenlade Szenen für verschiedene Plattformen
* Weitere Informationen finden Sie unter " [vorgestellte Welt](https://account.altvr.com/worlds/featured)"

## <a name="tips"></a>Tipps

* Treten Sie der [offiziellen altspacevr-Zwietracht](https://discordapp.com/invite/altspacevr)bei.
* Auf der Seite "Vorlage" auf der linken Seite zeigen wir Ihnen die neuesten Uploads nach Plattform. Wenn der Vorgang erfolgreich war, werden **vor 1-2 Minuten** angezeigt. Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![Vorlagen Panel mit hervorgehobenen Uploads geöffnet](images/unity-uploader-img-03.png)

* Sie können sich in der Welt befinden, wenn Sie aktualisieren. In dem Moment, in dem Uploader den **Upload vervollständigen** hat, können Sie die Welt zurücksetzen, um die Änderungen anzuzeigen.
* Das Erstellen für PCs mit einer einfachen Szene sollte weniger als 1 Minute dauern, um eine Änderung in altspace zu sehen.
* Legen Sie Ihre Welt als privat und nicht aufgelistet fest, um Ablenkungen zu vermeiden.
* Platzieren Sie einen Cube am Ursprung, damit Sie sehen können, wo Benutzer standardmäßig erzeugen werden. Blenden Sie den Cube beim Hochladen aus.

## <a name="troubleshooting"></a>Problembehandlung

**Ich kann auf nichts** zurückgreifen. Sie müssen einen Konflikt zu Objekten hinzufügen, um diese teleportieren zu können.

**Nichts geändert**
    * Haben Sie die Szene in Unity gespeichert?
    * Haben Sie die Plattform ausgewählt, auf der Sie testen?
    * Sind Sie in der richtigen Welt? Haben Sie die richtige Vorlage im Uploader und im Formular "World" ausgewählt?
    * Haben Sie die Statistik der Vorlagen Seite überprüft?

**Fehler beim Hochladen oder Timeout**
    * Der häufigste Fehler beim Hochladen weist die falsche Unity-Version auf. Er muss genau mit der erforderlichen Version übereinstimmen.
    * Der Upload ist möglicherweise zu groß. Versuchen Sie, die PC-Szenen < 100 MB zu halten. Fangen Sie klein an, und bauen Sie auf. Optimieren, optimieren und optimieren.
    * Probieren Sie es mit einem neuen Projekt mit einem einfachen Cube aus.
    * Erzwingen Sie das Beenden während eines Builds nicht, da die Szene beschädigt werden kann. Versuchen Sie erneut, hochzuladen.

**Es handelt sich um einen langsamen Prozess**
    * Wir empfehlen, nur für PC zu erstellen, während Sie später und für Android ausführen.
    * Entfernen Sie nicht verwendete Dateien. Aus irgendeinem Grund ist Unity manchmal übereifrig.

**Ich kann mich nicht mit meinen altspace-Anmelde Informationen anmelden.**
    * Bei e-Mails wird die Groß-/Kleinschreibung beachtet
    * Versuchen Sie es mit einem neuen Projekt.
    * Stellen Sie sicher, dass Ihr altspace-Konto in Ordnung ist.

## <a name="see-also"></a>Siehe auch

* [Erlernen von Unity](https://unity3d.com/learn)
* [Unity-Foren](https://forum.unity.com)
