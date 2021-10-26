---
title: Aktualisieren alter Unity-Projekte
description: Erfahren Sie, wie Sie Ihre Inhalte auf die neueste Version von Unity aktualisieren.
ms.date: 10/19/2021
ms.topic: article
keywords: Kits, Welten, Unity, Aktualisieren, Shader, Uploader, Problembehandlung
ms.openlocfilehash: 06af70164e5bf870a10bf1ee9e949e09dfa69fd2
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2021
ms.locfileid: "130302389"
---
<a name="upgrading-old-unity-projects"></a>Aktualisieren alter Unity-Projekte
=============================

Im Laufe der Jahre hat AltspaceVR mehrere seltene Upgrades durchlaufen, bei denen Benutzer ihre Inhalte ändern mussten. Wenn Sie feststellen, dass auf eine Vorlage oder ein Kit, die Sie in der Vergangenheit hochgeladen haben, in der neuesten Version von AltspaceVR nicht zugegriffen werden kann, befolgen Sie diese Anleitung, um Ihre Inhalte wieder in Betrieb zu nehmen.

> [!NOTE]
> Bevor Sie die Schritte in diesem Leitfaden ausführen, sollten Sie eine vollständige Sicherung Ihres Projekts erstellen, falls das Upgrade nicht reibungslos verläuft. Die einfachste Möglichkeit besteht darin, eine zweite Kopie des gesamten Projektordners zu erstellen. Erwägen Sie für eine erweiterte Lösung die Verwendung eines Versionskontrollsystems wie Git und GitHub.

<a name="overview"></a>Übersicht
---------

In diesem Artikel wird für die aktuelle Version von AltspaceVR die folgende Konfiguration verwendet:

* Spiel-Engine: Unity 2020.3.18f1 (auch akzeptabel: Unity 2020.3.9f1)
* Hochladen Tool: Uploader 2.2
* Rendering: Universal Render Pipeline (URP)
* Stereomodus: Single-Pass Instanziierung (SPI) oder Multiview auf Quest

Wenn Ihre Unity-Projektversion älter als 2020.3 ist, müssen Sie wahrscheinlich alle diese Updates gleichzeitig übernehmen. Befolgen Sie daher diese Anleitung von Anfang an. Wenn Sie unity 2020.3 bereits, aber mit Uploader 0.9, bereits haben, beginnen Sie mit Schritt 6.

1. **SICHERN IHRES PROJEKTS:** Erstellen Sie eine Kopie Ihres gesamten Projektverzeichnisses, und legen Sie sie an einem sicheren Ort ab. Dieses Upgrade ist ein destruktives Upgrade, sodass Sie ihre ursprünglichen Projektdateien verlieren, nachdem Sie es abgeschlossen haben.
    Wenn während dieses Upgrades Probleme auftreten, benötigen Sie eine bereinigte Kopie Ihres Projekts, auf die Sie zurückgreifen können.

2. **REMOVE OLD UPLOADER:** Gehen Sie wie in diesem Schritt vor, wenn Ihr Projekt altspaceVR Uploader 0.8 oder früher verwendet. Wenn Unity geschlossen ist, löschen Sie die folgenden Dateien/Ordner, und es sind die entsprechenden META-Dateien. Wenn die Datei/der Ordner nicht vorhanden ist, überspringen Sie sie einfach.

    * Assets/Altspace
    * Objekte/Plug-Ins
    * Assets/Prefabs/test-folder
    * Assets/Prefabs/Readme.txt
    * Assets/Resources/bg.jpeg
    * Assets/Resources/bg2.jpeg
    * Assets/Resources/logo.png
    * Assets/Resources/UserPreferences.asset
    * Assets/DFloor_v004.fbx

3. **REMOVE PROCESSED ASSETS (VERARBEITETE OBJEKTE ENTFERNEN)** – Gehen Sie wie in diesem Schritt vor, wenn Sie ein Upgrade auf eine neue Unity-Version durchführen. Wenn Unity geschlossen ist, löschen Sie den Ordner Bibliothek aus dem Projekt. Dies ist ein Unity-Systemordner, der enginespezifische Objekte und Dateien enthält, die (unter anderem) automatisch aus dem Inhalt des Ordners Assets generiert werden.

4. **ENGINE-VERSION HERUNTERLADEN:** Gehen Sie wie in diesem Schritt vor, wenn Sie ein Upgrade auf eine neue Unity-Version durchführen. Öffnen Sie den Unity Hub, und installieren Sie Unity 2020.3.18f1 aus dem Downloadarchiv ([Link zur Engine-Installation](unityhub://2020.3.18f1/a7d1c678663c)).
    * Wenn Sie auf einem Windows PC erstellen, aktivieren Sie die Kontrollkästchen für Android- und Mac-Buildunterstützung.
    * Wenn Sie auf einem Mac erstellen, aktivieren Sie die Kontrollkästchen für Android und Windows Buildunterstützung.

5. **UPGRADE PROJECT** : Öffnen Sie Ihr bereinigtes Projekt in Unity 2020.3.18f1, und lassen Sie Unity das Upgrade Ihres Projekts zu.
    Dieser Vorgang nimmt einige Zeit in Anspruch.

6. **DOWNLOAD THE UPLOADER** : Laden Sie die neueste Version des Uploaders [hier](https://aka.ms/AvrUrpUploader)herunter, und speichern Sie sie im Ordner Pakete Ihres Projekts. Diese Datei sollte die Dateierweiterung ".tgz" aufweisen.
    > [!NOTE]
    > Wenn Sie den Safari-Browser zum Herunterladen verwenden, wird er automatisch in eine TAR-Datei extrahiert, die Unity nicht verwenden kann. Sie können entweder einen anderen Browser zum Herunterladen oder das Systemhilfsprogramm "gzip" zum erneuten Komprimieren verwenden.
    
7. **INSTALLIEREN DES UPLOADERS:** Installieren Sie den Uploader aus dem Paket-Manager des Unity-Editors:
    1. Öffnen Sie das Fenster Unity Paket-Manager: Windows > Paket-Manager
    2. Klicken Sie oben links im Fenster auf das Symbol "+", und wählen Sie "Paket aus Tarball hinzufügen" aus.
    3. Wählen Sie die TGZ-Datei aus, die Sie im letzten Schritt heruntergeladen haben.
    4. Warten Sie, bis Unity das Paket entpackt hat.

8. **ÖFFNEN DES UPLOADERS:** Wenn die Installation erfolgreich war, steht in der oberen Leiste das Menü "AltspaceVR" zur Verfügung.
    Dieses Menü enthält separate Fenster für Kits und Vorlagen. Öffnen Sie den für Ihr Projekt am besten geeigneten.
    Wenn das Fenster zum ersten Mal geöffnet wird, werden Ihre Projekteinstellungen so konfiguriert, dass sie mit dem Altspace-Spielclient übereinstimmen: Aktivieren der universellen Renderpipeline und Single-Pass Instanziierung

9. **FIX SHADERS** : Während dieses erstmaligen Setups wird möglicherweise vorübergehend ein PowerShell-Fenster angezeigt.
    Möglicherweise werden Sie aufgefordert, einige Ihrer benutzerdefinierten/heruntergeladenen Shader zu aktualisieren. Wenn Sie die Eingabeaufforderung genehmigen, versucht das PowerShell-Skript automatisch, Ihre Shader zu aktualisieren, aber die Erfolgswahrscheinlichkeiten sind gering. Sie müssen manuell überprüfen, ob der Shader in URP weiterhin ordnungsgemäß funktioniert.

10. **FIX MATERIALS** : Einige/alle Ihre Materialien werden während des Upgradevorgangs möglicherweise rosa/magenta. Dies weist auf einen Fehler im Shader hin, der von diesem Material verwendet wird. Wenn Sie die integrierten Unity-Shader verwendet haben, können Sie diese in der Regel automatisch über das Menü zu URP-kompatiblen Shadern migrieren: Edit > Render Pipeline > Universal Render Pipeline > Upgrade Project Materials to UniversalRP Materials(Bearbeiten > Renderpipeline > Universelle Renderpipeline > Upgrade Project Materials to UniversalRP Materials( Materialien auf UniversalRP-Materialien aktualisieren).

11. **BUILD UND UPLOAD:** An diesem Punkt sollte das Projekt vollständig aktualisiert werden. Befolgen Sie die Anweisungen im [Erste Schritte](world-building-toolkit-getting-started.md) Handbuch, um Ihr Kit/Ihre Vorlage zu erstellen und hochzuladen.

<a name="troubleshooting-tips"></a>Hinweise zur Fehlerbehebung
---------------------

1. Wenn Sie feststellen, dass Ihre Inhalte im VR-Modus nur auf ein Auge angezeigt werden, unterstützen die von Ihnen verwendeten benutzerdefinierten Shader wahrscheinlich kein SPI-Rendering. Sie müssen einen anderen Shader auswählen oder die Anleitung zum Upgrade von [SPI von Unity](https://docs.unity3d.com/Manual/SinglePassInstancing.html) befolgen, um den Shader manuell zu bearbeiten und Unterstützung hinzuzufügen.

2. Wenn Sie feststellen, dass ein Teil Ihrer Inhalte im Spiel rosa/magenta ist oder vollständig unsichtbar ist, kann dies darauf zurückzuführen sein, dass ein Shader nicht mit URP kompatibel ist. Sie müssen entweder den Shader ersetzen oder ihn selbst aktualisieren.