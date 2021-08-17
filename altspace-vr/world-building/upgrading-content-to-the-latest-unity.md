---
title: Aktualisieren von Inhalten auf die neueste Unity-Version
description: Erfahren Sie, wie Sie Ihre Inhalte auf die neueste Version von Unity aktualisieren.
ms.date: 06/4/2021
ms.topic: article
keywords: Kits, Welten, Unity, Aktualisieren, Shader, Uploader, Problembehandlung
ms.openlocfilehash: a10e64b4dc19e256dcae9d61620de0140db60ccc0bf2a10dc864313f139bbd10
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126760"
---
# <a name="updating-content-to-the-latest-unity-version"></a>Aktualisieren von Inhalten auf die neueste Unity-Version

## <a name="moving-to-unity-202039"></a>Wechsel zu Unity 2020.3.9

Ab heute hat AltspaceVR ein Upgrade auf eine aktuelle Version von Unity (2020.3.9) durchgeführt. Zusätzlich zu einigen Leistungsverbesserungen ist dieses Update für zukünftige Features, die wir gerne integrieren möchten, für die Zukunft sicher. Diese Änderung sollte mit allen vorhandenen Inhalten kompatibel sein. Falls nicht, wenden Sie sich an den Support: altvr.com/support

Obwohl sich diese Umstellung auf 2020.3.9 nicht auf vom Benutzer generierte Inhalte ausdingt, nehmen wir in einigen Wochen eine Änderung am Stereorenderingmodus von AltspaceVR vor, der erfordert, dass Benutzer ihren Inhalt [aktualisieren.]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html) Dieses Upgrade auf [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) ermöglicht erhebliche Leistungsverbesserungen in Ihrer Welt. Beachten Sie, dass dieser neue Build die Abwärtskompatibilität mit Inhalten aus 2019.4 und älteren Versionen nicht mehr unterstützt. Es ist dringend erforderlich, dass alle Inhalte im Besitz des Erstellers so bald wie möglich aktualisiert werden, um Breaking Changes zu vermeiden. Befolgen Sie die anleitung unten, um Ihre Inhalte zu aktualisieren und einen reibungslosen Übergang zu Single Pass Instancing in Unity 2020.3.9 sicherzustellen.

> [!NOTE]
> Wenn Sie regelmäßig Inhalte verwenden, die sich im Besitz einer anderen Person befinden und für Sie freigegeben wurden, wenden Sie sich an den Besitzer des World Kits, und stellen Sie sicher, dass er plant, seine Inhalte zu aktualisieren.

> Wenn Sie Inhaltsersteller sind und Fragen haben oder Unterstützung benötigen, wenden Sie sich an unser Supportteam, um Hilfe zu erhalten: altvr.com/support

## <a name="testing-your-spi-content"></a>Testen von SPI-Inhalten

Verwenden Sie die folgenden Vorschauversionen von AltspaceVR, um Ihre neu aktualisierten Inhalte in VR zu testen. Die Vorschauversionen dienen nur zu Testzwecken und sollten nicht für eine allgemeine Nutzung der Plattform verwendet werden.

* [AltspaceVR SPI Preview for Windows Mixed Reality](https://aka.ms/AvrSpiMr)
* [AltspaceVR SPI Preview für SteamVR](https://aka.ms/AvrSpiSteam)
* [AltspaceVR SPI Preview for Oculus Rift](https://aka.ms/AvrSpiRift)

> Hinweis: Es wurden nur PC-VR-Vorschauen bereitgestellt. Single-Pass-Instanzrendering ist unter Android nicht verfügbar und wird auf Nicht-VR-Plattformen wie Mac nicht benötigt. Daher können Sie die allgemeine Releaseversion verwenden, um diese Geräte zu testen.


## <a name="storecompatibilitycheck"></a>Store Kompatibilitätsprüfung

Das Upgrade auf Unity 2020.3.9 wirkt sich auch auf die Kompatibilität von Headsets und Store-Build aus. Es ist jetzt erforderlich, AltspaceVR aus dem Store herunterzuladen, der mit Ihrem Headset kompatibel ist. Beispiel: Laden Sie altspaceVR für ein WinMR- oder Oculus-Headset aus der Windows Store- bzw. Oculus-Store herunter. Windows Mixed Reality Benutzer sollten AltspaceVR aus der Windows Store, Die Benutzer von Steam und Oculus Rift aus dem Oculus-Store.

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR Uploader v0.9.0 Upgrade Guide 

Uploader 0.9 ist anders gepackt als frühere Versionen des Uploaders. Gleichzeitig mit dieser Paketänderung erfordert der neue Uploader eine neue Version von Unity. Dieser Leitfaden soll diesen Upgradeprozess für alle Beteiligten reibungsloser und sicherer gestalten.

1. **SICHERN IHRES PROJEKTS:** Erstellen Sie eine Kopie Des gesamten Projektverzeichnisses, und legen Sie es an einem sicheren Ort ab. Dieses Upgrade ist ein destruktives Upgrade, sodass Sie keine Bundles für Unity 2019.4 erstellen oder hochladen können, nachdem Sie es abgeschlossen haben. Wenn während dieses Upgrades Probleme auftreten, benötigen Sie eine bereinigte Kopie Ihres Projekts, auf die Sie zurückfallen können. Sie benötigen sie auch, um Alle Live Kits oder Vorlagen zu aktualisieren, bevor AltspaceVR offiziell ein Upgrade auf Unity 2020.3.9 vorträgt.

2. **REMOVE OLD UPLOADER:** Wenn Unity geschlossen ist, löschen Sie die folgenden Dateien/Ordner und die entsprechenden META-Dateien:

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **ENGINE-VERSION HERUNTERLADEN:** Öffnen Sie den Unity-Hub, und installieren Sie Unity 2020.3.9 [(oder](https://unity3d.com/ru/unity/whats-new/2020.3.9) klicken Sie hier, um die Installation direkt zu installieren).

4. **UPGRADE PROJECT** : Öffnen Sie Ihr bereinigtes Projekt in Unity 2020.3.9, und lassen Sie Unity das Upgrade Ihres Projekts zu.

5. (nur PC) **DOWNLOAD MIXED REALITY FEATURE TOOL** : Befolgen Sie die Anweisungen zum Herunterladen des Mixed Reality Feature [Tools,](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)das Sie zum Verwalten der Installation des Uploader-Pakets verwenden.

6. **INSTALLIEREN DES UPLOADERS:** Verwenden Sie das MR-Featuretool, um Ihr Unity-Projekt auszuwählen, und fügen Sie das Feature AltspaceVR Uploader (unter der Überschrift AltspaceVR) hinzu. Befolgen Sie die Anweisungen im Tool.

Laden Sie unter macOS manuell [](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)die neueste Version aus der Registrierung herunter, und installieren Sie sie im Paket-Manager des Unity-Editors (Windows > Paket-Manager > + > Paket aus Tarball hinzufügen).

Sobald der Import des Pakets abgeschlossen ist, sollte das vertraute Uploaderfenster im AltspaceVR-Menüelement verfügbar sein.

## <a name="troubleshooting-tips"></a>Hinweise zur Fehlerbehebung

1. Wenn bei Ihrem WinMR-Headset Controller- oder Eingabeprobleme auftreten, stellen Sie sicher, dass es auf dem Kopf positioniert ist, um den Anwesenheitssensor ordnungsgemäß zu verwenden. Dies ist ein bekanntes Problem, und Microsoft arbeitet aktiv daran, dieses Problem zu beheben.

2. Überprüfen Sie Ihre Headset- und Store-Build-Kompatibilität. Wenn Sie beispielsweise ein WinMR-Headset verwenden, stellen Sie sicher, dass Ihr AltspaceVR-Build über die Windows Store.

3. Wenn Sie während der Tests feststellen, dass Ihre Inhalte nur mit einem Auge im VR-Modus angezeigt werden, wird das SPI-Rendering von den von Ihnen verwendeten benutzerdefinierten Shadern wahrscheinlich nicht unterstützt. Sie müssen einen anderen Shader auswählen oder die Anleitung für SPI-Upgrades von Unity befolgen, um den [Shader](https://docs.unity3d.com/Manual/SinglePassInstancing.html) manuell zu bearbeiten und Unterstützung hinzuzufügen.

4. Beachten Sie bei WinMR-Anwendungen, dass Sie vor dem Zugriff auf den VR-Modus in AltspaceVR: 
    1. Laden Sie OpenXR für die Windows Mixed Reality aus dem Microsoft Store.
        1. Öffnen der Mixed Reality-Portal-App
        2. Wählen Sie in der linken unteren Ecke der App "Mehr sehen" aus.
        3. Wählen Sie im angezeigten Menü OpenXR einrichten aus. Dies führt dazu, dass die Windows Store gestartet wird, von wo aus Sie die Runtime installieren können. Wenn dieses Menüelement nicht angezeigt wird, ist OpenXR möglicherweise bereits auf Ihrem PC installiert.