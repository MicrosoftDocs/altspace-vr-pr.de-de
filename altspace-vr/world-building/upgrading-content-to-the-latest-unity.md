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

Ab heute wurde altspaceVR auf eine aktuelle Version von Unity (2020.3.9) aktualisiert. Zusätzlich zu einigen Leistungsverbesserungen ist dieses Update für zukünftige Features geeignet, die wir gerne integrieren werden. Diese Änderung sollte mit allen vorhandenen Inhalten kompatibel sein. Wenn nicht, wenden Sie sich an den Support: altvr.com/support

Obwohl sich dieser Wechsel zu 2020.3.9 nicht auf vom Benutzer generierte Inhalte auswirkt, ändern wir in einigen Wochen den [Stereorenderingmodus]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)von AltspaceVR, in dem Benutzer ihre Inhalte aktualisieren müssen. Dieses Upgrade auf [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) ermöglicht erhebliche Leistungsverbesserungen in Ihrer Welt. Beachten Sie, dass dieser neue Build die Abwärtskompatibilität mit Inhalten ab Version 2019.4 nicht mehr unterstützt. Es ist dringend erforderlich, dass alle Inhalte im Besitz des Erstellers so schnell wie möglich aktualisiert werden, um Breaking Changes zu vermeiden. Befolgen Sie die anleitung unten, um Ihre Inhalte zu aktualisieren und einen reibungslosen Übergang zu Single Pass Instancing in Unity 2020.3.9 sicherzustellen.

> [!NOTE]
> Wenn Sie regelmäßig Inhalte verwenden, die sich im Besitz einer anderen Person befinden und für Sie freigegeben wurden, wenden Sie sich an den Besitzer der Welt/des Kits, und stellen Sie sicher, dass er plant, seine Inhalte zu aktualisieren.

> Wenn Sie Inhaltsersteller sind und Fragen haben oder Hilfe benötigen, wenden Sie sich an unser Supportteam, um Hilfe zu erhalten: altvr.com/support

## <a name="testing-your-spi-content"></a>Testen des SPI-Inhalts

Verwenden Sie die folgenden Vorschauversionen von AltspaceVR, um Ihre neu aktualisierten Inhalte in VR zu testen. Die Vorschauversionen dienen nur zu Testzwecken und sollten nicht für eine allgemeine Verwendung der Plattform verwendet werden.

* [AltspaceVR SPI Preview für Windows Mixed Reality](https://aka.ms/AvrSpiMr)
* [AltspaceVR SPI Preview für SteamVR](https://aka.ms/AvrSpiSteam)
* [AltspaceVR SPI Preview für Oculus Rift](https://aka.ms/AvrSpiRift)

> Hinweis: Es wurden nur PC-VR-Vorschauversionen bereitgestellt. Single-Pass-Instanzrendering ist unter Android nicht verfügbar und auf Nicht-VR-Plattformen wie Mac nicht erforderlich. Daher können Sie die allgemeine Releaseversion verwenden, um diese Geräte zu testen.


## <a name="storecompatibilitycheck"></a>Store Kompatibilitätsprüfung

Das Upgrade auf Unity 2020.3.9 wirkt sich auch auf headset- und store-build-Kompatibilität aus. Sie müssen altspaceVR jetzt aus dem Store herunterladen, der mit Ihrem Headset kompatibel ist. Beispiel: Laden Sie altspaceVR für ein WinMR- oder Oculus-Headset von der Windows Store oder oculus Store herunter. Windows Mixed Reality Benutzer sollten AltspaceVR aus dem Windows Store herunterladen, Die Benutzer von Steam und Oculus Rift über die Oculus Store.

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>Upgradehandbuch für AltspaceVR Uploader v0.9.0 

Uploader 0.9 ist anders gepackt als frühere Versionen des Uploaders. Gleichzeitig mit dieser Paketänderung erfordert der neue Uploader eine neue Version von Unity. Dieser Leitfaden soll diesen Upgradeprozess für alle Beteiligten reibungsloser und sicherer gestalten.

1. **SICHERN IHRES PROJEKTS:** Erstellen Sie eine Kopie Ihres gesamten Projektverzeichnisses, und legen Sie sie an einem sicheren Ort ab. Dieses Upgrade ist ein destruktiver Upgrade, sodass Sie nach Abschluss des Upgrades keine Bundles für Unity 2019.4 erstellen oder hochladen können. Wenn während dieses Upgrades Probleme auftreten, benötigen Sie eine bereinigte Kopie Ihres Projekts, auf die Sie zurückgreifen können. Sie benötigen sie auch, um alle Live Kits oder Vorlagen zu aktualisieren, bevor AltspaceVR offiziell ein Upgrade auf Unity 2020.3.9 durchführen kann.

2. **REMOVE OLD UPLOADER:** Löschen Sie nach dem Schließen von Unity die folgenden Dateien/Ordner, und es sind die entsprechenden META-Dateien:

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **ENGINE-VERSION HERUNTERLADEN:** Öffnen Sie den Unity-Hub, und installieren Sie Unity 2020.3.9 (oder [klicken Sie hier,](https://unity3d.com/ru/unity/whats-new/2020.3.9) um die Installation direkt zu installieren).

4. **UPGRADE PROJECT** : Öffnen Sie Ihr bereinigtes Projekt in Unity 2020.3.9, und lassen Sie Unity das Upgrade Ihres Projekts zu.

5. (Nur PC) **MIXED REALITY FEATURE TOOL HERUNTERLADEN:** Befolgen Sie die Anweisungen zum Herunterladen des [Mixed Reality Feature Tools,](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)das Sie zum Verwalten der Installation des Uploaderpakets verwenden.

6. **INSTALLIEREN DES UPLOADERS:** Verwenden Sie das MR-Featuretool, um Ihr Unity-Projekt auszuwählen, und fügen Sie das Feature AltspaceVR Uploader (unter der Überschrift AltspaceVR) hinzu. Befolgen Sie die Anweisungen im Tool.

Laden Sie unter macOS manuell die neueste Version aus der [Registrierung](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)herunter, und installieren Sie sie im Paket-Manager des Unity-Editors (Windows > Paket-Manager > + > Paket aus Tarball hinzufügen).

Sobald der Import des Pakets abgeschlossen ist, sollte das vertraute Uploaderfenster im Menüelement AltspaceVR verfügbar sein.

## <a name="troubleshooting-tips"></a>Hinweise zur Fehlerbehebung

1. Wenn Sie Controller- oder Eingabeprobleme an Ihrem WinMR-Headset haben, stellen Sie sicher, dass es auf dem Kopf positioniert ist, um den Anwesenheitssensor ordnungsgemäß einzubinden. Dies ist ein bekanntes Problem, und Microsoft arbeitet aktiv daran, es zu beheben.

2. Überprüfen Sie ihre Headset- und Storebuildkompatibilität. Wenn Sie beispielsweise ein WinMR-Headset verwenden, stellen Sie sicher, dass Ihr AltspaceVR-Build über die Windows Store abgerufen wurde.

3. Wenn Sie während der Tests feststellen, dass Ihre Inhalte nur im VR-Modus auf ein Auge angezeigt werden, unterstützen die von Ihnen verwendeten benutzerdefinierten Shader wahrscheinlich kein SPI-Rendering. Sie müssen einen anderen Shader auswählen oder die Anleitung zum Upgrade von [SPI von Unity](https://docs.unity3d.com/Manual/SinglePassInstancing.html) befolgen, um den Shader manuell zu bearbeiten und Unterstützung hinzuzufügen.

4. Beachten Sie für WinMR-Personen, dass Sie vor dem Zugriff auf den VR-Modus in AltspaceVR: 
    1. Laden Sie OpenXR für Windows Mixed Reality aus dem Microsoft Store herunter, und installieren Sie es.
        1. Öffnen der Mixed Reality-Portal-App
        2. Wählen Sie in der unteren linken Ecke der App "Mehr anzeigen" aus.
        3. Wählen Sie im daraufhin angezeigten Menü OpenXR einrichten aus. Dies führt dazu, dass die Windows Store gestartet wird, von wo aus Sie die Runtime installieren können. Wenn dieses Menüelement nicht angezeigt wird, ist OpenXR möglicherweise bereits auf Ihrem PC installiert.