---
title: Einführung in das World Building Toolkit
description: Erfahren Sie, wie Sie Ihre AltspaceVR-Welten mithilfe von Unity-Szenenvorlagen mit dem World Building Toolkit einrichten und hochladen.
ms.date: 03/11/2021
ms.topic: article
keywords: Toolkit
ms.openlocfilehash: 3b41f02aec1077a37b95a6826c105e1cd31974e3
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923077"
---
# <a name="introducing-the-world-building-toolkit"></a>Einführung in das World Building Toolkit

> [!NOTE]
> Das World Building Toolkit ist ein Communityprojekt, das von unserem großartigen [Freund, Mad Madden,](https://twitter.com/chigamesstudio)mit Unterstützung von uns ausgeführt wird. Wenn Sie daran interessiert sind, treten Sie der offiziellen [AltspaceVR-Diskothek bei,](https://discordapp.com/invite/altspacevr) und besuchen Sie den #world-Building-Kanal. Wir haben derzeit eine Betaversion der Mac-Testversion, weitere [Details](https://altvr.com/altspacevr-mac)

Mit dem Uploader können Sie eine Unity-Szene als Vorlage für Ihre Welten verwenden. Sie können ein eigenes Haus für Oder Ihre bevorzugte Erstellung von Minecraft einbringen. Wenn Sie sie in Unity importieren können, können Sie sie wahrscheinlich auf diese Weise in Altspace importieren. Hier sind einige Beispiele [für Worlds](https://account.altvr.com/worlds/1046572460192825569).

![Beispielwelten](images/unity-uploader-img-01.png)

## <a name="setup"></a>Einrichten

1. Treten Sie der [offiziellen AltspaceVR-Diskothek](https://discordapp.com/invite/altspacevr) bei, und besuchen Sie den #world-Building-Kanal – Friends don't let friends build Worlds alone (Freunde lassen Freunde nicht allein Welten erstellen).
2. Lesen Sie [unseren Leitfaden für Erste Schritte für die](world-building-getting-started.md) Grundlagen.
3. [Installieren Sie Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) und **Unity 2020.3.9.** Der Uploader funktioniert nur, wenn Sie genau mit dieser Version übereinstimmen. Wenn Sie noch kein Unity-Konto haben, benötigen Sie ein kostenloses Unity-Konto, und wählen Sie **Persönlich** aus, da Sie dies zum Spaß machen! Stellen Sie während der Installation sicher, dass Sie die **Option Android Builds** aktivieren und die automatische Aktualisierung deaktivieren.
4. [Herunterladen des neuesten Unity-Uploaders](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. [Erstellen Sie eine Vorlage](https://account.altvr.com/space_templates/new) auf unserer Website. Nennen Sie **ihn Hallo Welt Vorlage**.
6. [Erstellen Sie eine Welt,](https://account.altvr.com/worlds/my) und nennen **Sie sie Hallo Welt.** Wählen **Hallo Welt Vorlage** als Vorlage aus.

![Bildschirm "Welt erstellt"](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Hochladen Ihrer Szene

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Öffnen Sie Unity Hub, und erstellen Sie ein neues Unity 2020.3.9-Projekt.
2. Wenn Ihr Projekt geöffnet ist, importieren Sie den Uploader, indem Sie auf die heruntergeladene Datei doppelklicken (es ist ein Unity-Paket). Nun sollte eine neue Registerkarte mit dem Namen **AltspaceVR angezeigt werden.** Sie müssen das Paket für jedes Unity-Projekt importieren, das Sie mit Altspace verwenden möchten.
3. Menü **öffnen > AltspaceVR > Buildeinstellungen**
4. Melden Sie sich mit ihren Altspace-Kontoanmeldeinformationen an.
5. Wählen **Sie Vorlagen laden** und dann Vorlage Hallo Welt **aus.**
6. Fügen Sie Ihrer Szene einen Würfel hinzu, und speichern Sie ihn.
7. Aktivieren **Sie Build für Windows?** und deaktivieren Sie Build für **Android?**
8. Klicken Sie auf **Hochladen**. In etwa einer Minute sollte Upload **abgeschlossen** sein.
9. Treten **Hallo Welt,** indem Sie Altspace starten und über **Menu > Worlds > My Worlds eingeben.**
10. Reset the World from **Menu > Settings > Moderate > Reset Space**
11. Der Cube sollte angezeigt werden. Wenn Sie dies wie im obigen Video schnell tun, können Sie Änderungen innerhalb von nur 10 Sekunden sehen.

## <a name="whats-supported"></a>Unterstützte Funktionen

* Ja: Modelle, Kollisionen, Animationen, Partikeleffekte, Audio, Skyboxes und so weiter
* Nein: Skripts. Aus Sicherheitsgründen werden Uploads mit Skripts abgelehnt.
* Vielleicht: ausgefallene Dinge wie dynamische globale Beschriftung
* Hochladen von Szenen für verschiedene Plattformen separat oder zusammen
* Weitere Informationen [finden Sie unter Ausgewählte Welten.](https://account.altvr.com/worlds/featured)Viele wurden mit dem Uploader erstellt.

## <a name="tips"></a>Tipps

* Treten Sie der [offiziellen AltspaceVR-Verwesung bei.](https://discordapp.com/invite/altspacevr)
* Auf der Seite Vorlage auf der linken Seite werden die neuesten Uploads nach Plattform angezeigt. Wenn dies erfolgreich war, wird vor **1 bis 2 Minuten die 1-2-Minuten-1000-000-000-000-000-Minute-1-0** Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![Geöffneter Vorlagenbereich mit hervorgehobenen Uploads](images/unity-uploader-img-03.png)

* Sie können sich beim Aktualisieren auf der ganzen Welt befingen. In dem Moment, in dem der Uploader **Upload Complete (Upload abgeschlossen)** sagt, können Sie die Welt zurücksetzen, um die Änderungen zu sehen.
* Das Erstellen für nur PC-Computer mit einer einfachen Szene sollte weniger als 1 Minute dauern, um eine Änderung in Altspace zu sehen.
* Legen Sie Ihre Welt auf Privat und Nicht aufgeführt fest, um Ableitungen zu vermeiden.
* Platzieren Sie einen Cube am Ursprung, damit Sie sehen können, wo benutzer standardmäßig erstellt werden. Blendet den Cube beim Hochladen aus.

## <a name="troubleshooting"></a>Problembehandlung

**Ich stürzt ab oder kann mich nicht auf etwas teleportieren.** Sie müssen Objekten eine Kollision hinzufügen, um sie zu teleportieren.

**Nichts geändert**
    * Haben Sie die Szene in Unity speichern?
    * Haben Sie die Plattform, auf der Sie testen möchten, auswählen?
    * Befinden Sie sich in der richtigen Welt? Haben Sie die richtige Vorlage im Uploader- und im World-Formular verwendet?
    * Haben Sie die Statistiken der Vorlagenseite überprüft?

**Fehler beim Hochladen oder Zeitsendzeit**
    * Der häufigste Uploadfehler ist die falsche Unity-Version. Er muss genau mit der erforderlichen Version übereinstimmen.
    * Ihr Upload ist möglicherweise zu groß. Versuchen Sie, PC-Szenen < 100 MB zu halten. Beginnen Sie klein, und erstellen Sie sich. Optimieren, Optimieren, Optimieren.
    * Versuchen Sie es mit einem neuen Projekt mit einem einfachen Cube.
    * Erzwingen Sie nicht das Beenden während eines Build- es kann Ihre Szene beschädigt. Versuchen Sie, erneut zu laden.

**Dies ist ein langsamer Prozess.**
    * Es wird empfohlen, nur während der Iterierung und später für Android für PC zu erstellen.
    * Versuchen Sie, nicht verwendete Dateien zu entfernen. Aus irgendeinem Grund wird Unity manchmal übereigen.

**Ich kann mich nicht mit meinen Altspace-Anmeldeinformationen anmelden.**
    * Bei E-Mails wird die Kleinschreibung beachtet.
    * Versuchen Sie es mit einem neuen Projekt.
    * Stellen Sie sicher, dass Ihr Altspace-Konto in gutem Zustand ist.

## <a name="see-also"></a>Siehe auch

* [Unity Learn](https://unity3d.com/learn)
* [Unity-Foren](https://forum.unity.com)
