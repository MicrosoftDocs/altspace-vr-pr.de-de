---
title: Einführung in altspace uploader
description: Erfahren Sie, wie Sie Ihre AltspaceVR-Welten mithilfe von Unity-Szenenvorlagen mit dem Altspace Uploader einrichten und hochladen.
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: Toolkit, Altspace, Uploader
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298803"
---
# <a name="introducing-the-altspace-uploader"></a>Einführung in altspace uploader

> [!NOTE]
> - Wenn Sie daran interessiert sind, treten Sie der offiziellen [AltspaceVR-Diskothek bei,](https://discordapp.com/invite/altspacevr) und besuchen Sie den #world-Building-Kanal.  
> - Wenn Sie versuchen, einen alten Bereich zu beleben, lesen Sie den [Upgradeleitfaden](upgrading-old-unity-projects.md). 

Mit dem Uploader können Sie eine Unity-Szene als Vorlage für Ihre Welten verwenden. Sie können ein eigenes Haus für Oder Ihre bevorzugte Erstellung von einem Minecraft. Wenn Sie sie in Unity importieren können, können Sie sie wahrscheinlich auf diese Weise in Altspace importieren. Hier sind einige Beispiele [für Worlds](https://account.altvr.com/worlds/1046572460192825569).

![Beispielwelten](images/unity-uploader-img-01.png)

## <a name="setup"></a>Einrichten

1. Treten Sie der [offiziellen AltspaceVR-Diskothek bei,](https://discordapp.com/invite/altspacevr) und besuchen Sie den #world-Building-Kanal. Freunde lassen Freunde nicht allein Welten erstellen.
2. Lesen Sie [unseren Leitfaden für Erste Schritte world-building für](world-building-getting-started.md) die Grundlagen.
3. [Installieren Sie Unity Hub](https://unity3d.com/get-unity/download) und **Unity 2020.3.9.** Der Uploader funktioniert nur, wenn Sie genau mit dieser Version übereinstimmen. Wenn Sie noch kein Unity-Konto haben, benötigen Sie ein kostenloses Unity-Konto. Wählen Sie während der Installation die **persönliche Version** aus (da Sie dies aus Spaß machen!) und stellen Sie sicher, dass Sie Folgendes tun:
    * Schließen Sie das **Android Build Support-Modul** ein.
    * Fügen Windows das Modul **Mac Build Support (Mono)** ein.
    * Fügen Sie unter Mac das Modul **Windows BuildUnterstützung (Mono)** ein.
4. [Herunterladen des AltspaceVR-Uploaders](https://aka.ms/AvrUrpUploader)
5. [Erstellen Sie eine Vorlage](https://account.altvr.com/space_templates/new) auf unserer Website. Nennen Sie **ihn Hallo Welt Vorlage**.
6. [Erstellen Sie eine Welt,](https://account.altvr.com/worlds/my) und nennen Sie **sie Hallo Welt.** Wählen **Hallo Welt Vorlage** als Vorlage aus.

![Bildschirm "Welt erstellt"](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>Hochladen Ihrer Szene

> [!NOTE]
> Eine ausführlichere Schritt-für-Schritt-Anleitung finden Sie [hier.](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)

1. Öffnen Sie Unity Hub, und erstellen Sie ein neues Unity 2020.3.9-Projekt. Wählen Sie für Ihre Vorlage Universal **Render Pipeline (Universelle Renderpipeline) aus.**

    ![Auswählen der UNITY-VORLAGE für URP](images/001-unity-templates.png)

1. Navigieren Sie zu dem Ordner, in den Sie den Altspace Uploader heruntergeladen haben, und kopieren oder verschieben Sie ihn dann aus diesem Ordner in den Stammordner Ihres neuen Unity-Projekts.
1. Wählen Sie in Unity auf der Menüleiste **Fenster**  >  **Paket-Manager.**
1. Wählen Sie Paket-Manager Menüleiste die Dropdownliste mit dem Pluszeichen ("+") und dann Paket aus **Tarball hinzufügen aus.**
1. Navigieren Sie zu dem Ordner, der den Altspace Uploader enthält, wählen Sie den Uploader aus, und klicken Sie dann **auf Öffnen.**  Nachdem das Paket geladen wurde, **wird AltspaceVR** auf der Menüleiste angezeigt:

    ![AltspaceVR in der Menüleiste](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Sie müssen das Altspace Uploader-Paket in jedes Unity-Projekt importieren, das Sie mit Altspace verwenden möchten.
1. Wählen Sie in der Menüleiste **AltspaceVR > Vorlagen aus.**
1. Melden Sie **sich im Dialogfeld Altspace VR Templates (ALTSPACE-VR-Vorlagen)** mit ihren Altspace-Kontoanmeldeinformationen an. (Die MSA-Anmeldung ist in Kürze verfügbar. Wenn Sie sich bisher nur mit Ihrem Microsoft-Konto bei Altspace angemeldet haben, müssen Sie mithilfe der Option "Kennwort vergessen" auf der Website ein Kennwort erstellen.)
1. Klicken Sie **auf die Dropdownliste** Vorlage auswählen, und wählen Sie **dann vorlage Hallo Welt aus.**
1. Wählen Sie eine Szene aus: Klicken Sie auf die Schaltfläche Auslassungspunkten für eine **UNITY-Datei** auswählen (drei Punkte), navigieren Sie dann zum Ordner Assets Scenes in Ihrem Projekt, und wählen Sie  >   **SampleScene.unity** aus, und öffnen Sie ihn.
1. Stellen **Sie sicher, dass unter Build** für Plattformen: die **Windows** ausgewählt ist. Derzeit sollten die anderen beiden Optionen, **Android** und **Mac,** **nicht** ausgewählt werden. Sobald Sie möchten, dass Die Benutzer besuchen, sollten Sie für alle Plattformen erstellen und hochladen."
1. Wählen Sie die **Schaltfläche Build & Hochladen** aus. Dieser Vorgang kann ein bis zwei Minuten dauern.
1. Starten Sie ALTSPACE, wählen Sie **hauptmenü** aus, und wählen Sie dann auf der Menüleiste **My Worlds (Meine Welten) aus.**
1. Navigieren Sie **Hallo Welt,** und öffnen Sie es.

    Ihre Szene sollte mit denen im Unity-Editor vergleichbar sein.

## <a name="whats-supported"></a>Unterstützte Funktionen

* Ja: Modelle, Kollisionen, Animationen, Partikeleffekte, Audio, Skyboxes und so weiter.
* Nein: Skripts. Aus Sicherheitsgründen werden Uploads mit Skripts abgelehnt.
* Vielleicht: ausgefallene Dinge wie dynamische globale Füllungen.
* Hochladen szenen für verschiedene Plattformen separat oder zusammen.
* Weitere Informationen [finden Sie unter Ausgewählte Welten.](https://account.altvr.com/worlds/featured) Viele wurden mit dem Uploader erstellt.

## <a name="tips"></a>Tipps

* Treten Sie der [offiziellen AltspaceVR-Verwesung bei.](https://discordapp.com/invite/altspacevr)
* Auf der Seite Vorlage auf der linken Seite werden die neuesten Uploads nach Plattform angezeigt. Wenn dies erfolgreich war, wurde **vor 1 bis 2 Minuten die 1-2-Minuten-1-Minute-1-000-000-Uhr -1-0000-000** 

![Geöffneter Vorlagenbereich mit hervorgehobenen Uploads](images/template-upload-list.png)

* Sie können sich bei der Aktualisierung auf der ganzen Welt befingen. In dem Moment, in dem der Uploader **Hochladen Abgeschlossen ausdrückt,** können Sie die Welt zurücksetzen, um die Änderungen zu sehen.
* Beim Erstellen für nur PC mit einer einfachen Szene sollte es weniger als eine Minute dauern, bis eine Änderung in Altspace zu sehen ist.
* Legen Sie Ihre Welt auf Privat und Nicht aufgeführt fest, um Ableitungen zu vermeiden.
* Platzieren Sie einen Cube am Ursprung, damit Sie sehen können, wo benutzer standardmäßig erstellt werden. Blendet den Cube beim Hochladen aus.

## <a name="troubleshooting"></a>Problembehandlung

**Ich stürzt ab oder kann mich nicht auf etwas teleportieren.** Sie müssen Objekten eine Kollision hinzufügen, um sie zu teleportieren.

**Nichts geändert**
    * Haben Sie die Szene in Unity speichern?
    * Haben Sie die Plattform, auf der Sie testen möchten, auswählen?
    * Befinden Sie sich in der richtigen Welt? Haben Sie die richtige Vorlage im Uploader- und im World-Formular verwendet?
    * Haben Sie die Statistiken der Vorlagenseite überprüft?

**Hochladen schlägt fehl oder es kommt zu einem Zeitsendzeit**
    * Der häufigste Uploadfehler resultiert aus der falschen Unity-Version. Sie müssen genau mit der erforderlichen Version übereinstimmen.
    * Ihr Upload ist möglicherweise zu groß. Versuchen Sie, PC-Szenen < 100 MB zu halten. Beginnen Sie klein, und erstellen Sie es. Optimieren, Optimieren, Optimieren.
    * Versuchen Sie es mit einem neuen Projekt, das einen einfachen Cube enthält.
    * Erzwingen Sie nicht das Beenden während eines Build- es kann Ihre Szene beschädigt. Versuchen Sie, erneut hochzuladen.

**Dies ist ein langsamer Prozess.**
    * Es wird empfohlen, nur während der Iterierung und später für Android für PC zu erstellen.
    * Versuchen Sie, nicht verwendete Dateien zu entfernen. Aus irgendeinem Grund wird Unity manchmal übereigen.

**Ich kann mich nicht mit meinen Altspace-Anmeldeinformationen anmelden.**
    * Bei E-Mails wird die Kleinschreibung beachtet.
    * Versuchen Sie es mit einem neuen Projekt.
    * Stellen Sie sicher, dass Ihr Altspace-Konto in gutem Zustand ist.

## <a name="see-also"></a>Weitere Informationen

* [Unity Learn](https://unity3d.com/learn)
* [Unity-Foren](https://forum.unity.com)  
