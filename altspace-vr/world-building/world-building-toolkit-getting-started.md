---
title: Einführung in das World Building Toolkit
description: Erfahren Sie, wie Sie Ihre AltspaceVR-Welten mithilfe von Unity-Szenenvorlagen mit dem World Building Toolkit einrichten und hochladen.
ms.date: 03/11/2021
ms.topic: article
keywords: Toolkit
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125405"
---
# <a name="introducing-the-world-building-toolkit"></a>Einführung in das World Building Toolkit

> [!NOTE]
> Das World Building Toolkit ist ein Communityprojekt, das von unserem ehrfürchtigen [Freund, Antonio Madden,](https://twitter.com/chigamesstudio)mit Unterstützung von uns ausgeführt wird. Wenn Sie daran interessiert sind, treten Sie dem [offiziellen AltspaceVR-Discord](https://discordapp.com/invite/altspacevr) bei, und besuchen Sie den #world-Building-Kanal. Wir verfügen derzeit über eine Betaversion der Mac-Testversion, [weitere Details](https://altvr.com/altspacevr-mac)

Mit dem Uploader können Sie eine Unity-Szene als Vorlage für Ihre Welten verwenden. Sie können ein gepenntes Haus für Einen oder Ihre bevorzugte Erstellung aus Minecraft. Wenn Sie es in Unity importieren können, können Sie es wahrscheinlich auf diese Weise in Altspace importieren. Hier sind einige [Beispiele für Worlds](https://account.altvr.com/worlds/1046572460192825569).

![Beispielwelten](images/unity-uploader-img-01.png)

## <a name="setup"></a>Setup

1. Treten Sie dem [offiziellen AltspaceVR-Discord](https://discordapp.com/invite/altspacevr) bei, und besuchen Sie den #world-Building-Kanal – Friends don't let friends build Worlds alone (Freunde lassen sich nicht allein Welten erstellen).
2. Informationen zu den Grundlagen finden Sie in unserem [World-Building Erste Schritte Guide (World-Building Erste Schritte Guide).](world-building-getting-started.md)
3. [Installieren Sie Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) und **Unity 2020.3.9.** Der Uploader funktioniert nur, wenn Sie genau mit dieser Version übereinstimmen. Sie benötigen ein kostenloses Unity-Konto, wenn Sie nicht über ein Konto verfügen, und wählen **Persönlich** aus, da Sie dies zum Spaß erledigen! Stellen Sie während der Installation sicher, dass Sie die Option **Android-Builds** aktivieren und das automatische Update deaktivieren.
4. [Herunterladen des neuesten Unity-Uploaders](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. Erstellen Sie auf unserer Website [eine Vorlage.](https://account.altvr.com/space_templates/new) Nennen Sie es **Hallo Welt Vorlage**.
6. [Erstellen Sie eine Welt,](https://account.altvr.com/worlds/my) und nennen Sie sie **Hallo Welt**. Wählen Sie **Hallo Welt Vorlage** als Vorlage aus.

![Bildschirm "Welt erstellt"](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Hochladen Ihrer Szene

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Öffnen Sie Unity Hub, und erstellen Sie ein neues Unity 2020.3.9-Projekt.
2. Wenn Ihr Projekt geöffnet ist, importieren Sie den Uploader, indem Sie auf die heruntergeladene Datei doppelklicken (es ist ein Unity-Paket). Nun sollte eine neue Registerkarte mit dem Namen **ALTSPACEVR** angezeigt werden. Sie müssen das Paket für jedes Unity-Projekt importieren, das Sie mit ALTSPACE verwenden möchten.
3. **Menü öffnen > AltspaceVR > Build Einstellungen**
4. Melden Sie sich mit Ihren Altspace-Kontoanmeldeinformationen an.
5. Wählen Sie **Vorlagen laden** und dann **Hallo Welt Vorlage** aus.
6. Fügen Sie Ihrer Szene einen Cube hinzu, und speichern Sie diesen.
7. Aktivieren Sie **Build für Windows?** und deaktivieren **Sie Build für Android?**
8. Klicken Sie auf **Hochladen**. In etwa einer Minute sollte **Hochladen** abgeschlossen sein.
9. Treten Sie **Hallo Welt** bei, indem Sie Altspace starten und über **Menu > Worlds > My Worlds eingeben.**
10. Zurücksetzen der Welt über Menü > Einstellungen > Moderate > Zurücksetzen des **Speicherplatzes**
11. Der Cube sollte angezeigt werden. Wenn Sie dies schnell wie im obigen Video tun, können Sie Änderungen innerhalb von bis zu 10 Sekunden sehen.

## <a name="whats-supported"></a>Unterstützte Funktionen

* Ja: Modelle, Kollisionen, Animationen, Partikeleffekte, Audio, Skyboxen usw.
* Nein: Skripts. Aus Sicherheitsgründen werden Uploads mit Skripts abgelehnt.
* Vielleicht: ausgefallene Dinge wie dynamische globale Füllung
* Hochladen Szenen für verschiedene Plattformen separat oder zusammen
* Weitere Informationen finden Sie unter [Ausgewählte Welten.](https://account.altvr.com/worlds/featured)Viele wurden mit dem Uploader erstellt.

## <a name="tips"></a>Tipps

* Treten Sie dem [offiziellen AltspaceVR-Discord bei.](https://discordapp.com/invite/altspacevr)
* Auf der Seite Vorlage auf der linken Seite werden die neuesten Uploads nach Plattform angezeigt. Wenn dies erfolgreich war, wird **vor 1–2 Minuten** angezeigt. Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![Vorlagenbereich mit hervorgehobenen Uploads geöffnet](images/unity-uploader-img-03.png)

* Sie können in der Welt sein, wenn Sie ein Update durchführen. Sobald der Uploader Hochladen **Abgeschlossen** sagt, können Sie die Welt zurücksetzen, um die Änderungen anzuzeigen.
* Das Erstellen nur für PC mit einer einfachen Szene sollte weniger als eine Minute dauern, bis eine Änderung in Altspace angezeigt wird.
* Legen Sie Ihre Welt auf Privat und Nicht aufgeführt fest, um Ablenkungen zu vermeiden.
* Platzieren Sie einen Cube am Ursprung, damit Sie sehen können, wo die Personen standardmäßig entstehen. Blendet den Cube beim Hochladen aus.

## <a name="troubleshooting"></a>Problembehandlung

Ich fällt oder kann nichts **teleportieren.** Sie müssen Objekten Konflikte hinzufügen, um sie zu teleportieren.

**Nichts geändert**
    * Haben Sie die Szene in Unity gespeichert?
    * Haben Sie die Plattform ausgewählt, auf der Sie testen?
    * Befinden Sie sich in der richtigen Welt? Haben Sie im Format Uploader AND (Welt) die richtige Vorlage ausgewählt?
    * Haben Sie die Statistiken der Vorlagenseite überprüft?

**Hochladen schlägt fehl oder führt zu einem Times out**
    * Der häufigste Uploadfehler ist die falsche Unity-Version. Er muss genau mit der erforderlichen Version übereinstimmen.
    * Ihr Upload ist möglicherweise zu groß. Versuchen Sie, PC-Szenen < 100 MB beizubehalten. Beginnen Sie klein, und erstellen Sie sich. Optimieren, optimieren, optimieren.
    * Probieren Sie es mit einem neuen Projekt mit einem einfachen Cube aus.
    * Erzwingen Sie das Beenden während eines Builds nicht. Dadurch kann Ihre Szene beschädigt werden. Versuchen Sie, erneut zu laden.

**Dies ist ein langsamer Prozess.**
    * Es wird empfohlen, nur für den PC zu erstellen, während Sie und später für Android iterieren.
    * Versuchen Sie, nicht verwendete Dateien zu entfernen. Aus irgendeinem Grund wird Unity manchmal überzeig.

**Ich kann mich nicht mit meinen Altspace-Anmeldeinformationen anmelden.**
    * Bei E-Mails wird die Groß-/Kleinschreibung beachtet.
    * Versuchen Sie es mit einem neuen Projekt.
    * Stellen Sie sicher, dass Ihr Altspace-Konto gut dasteht.

## <a name="see-also"></a>Siehe auch

* [Unity Learn](https://unity3d.com/learn)
* [Unity-Foren](https://forum.unity.com)
