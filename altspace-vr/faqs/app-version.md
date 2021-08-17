---
title: Suchen der AltspaceVR-App-Version
description: Erfahren Sie, wie Sie die AltspaceVR-App, -Einstellungen und -Clientprotokolle verwenden, um die aktuell ausgeführte AltspaceVR-Version zu ermitteln.
ms.date: 02/10/2021
ms.topic: article
keywords: App-Version
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128251"
---
# <a name="finding-the-altspacevr-app-version"></a>Suchen der AltspaceVR-App-Version

Im Zuge der Problembehandlung werden Sie möglicherweise gefragt, welche Version der AltspaceVR-App Sie gerade ausführen.

## <a name="in-altspacevr"></a>In AltspaceVR

Navigieren Sie zum Menü **"Einstellungen",** und wählen Sie in der linken Navigationsleiste **Die** App-Version in AltspaceVR aus. Die "App-Version" wird hier gemeldet, wie im folgenden Screenshot gezeigt.

![Einstellungen menü open with about panel open](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>In Windows System Einstellungen

Wenn Sie AltspaceVR über die Microsoft Store installiert haben, finden Sie die App-Version zusätzlich in den Windows Systemeinstellungen.  Dieses Szenario eignet sich gut, wenn Sie die App-Version melden, wenn Sie sich nicht erfolgreich beim Client anmelden können.

Um die App-Version in Windows Systemeinstellungen zu finden, öffnen Sie das **Startmenü,** geben **Sie Apps & Features** ein, und wählen Sie das Ergebnis aus. Navigieren Sie in der Liste der Apps zu **AltspaceVR.** Klicken Sie mit der linken Maustaste auf ALTSPACEVR, und wählen Sie **erweiterte Optionen** aus dem angezeigten Menü aus.

![Menü "Apps und Features" mit hervorgehobener Option "Erweitert" geöffnet](images/app-version-img-02.png)

In den **erweiterten Optionen** sollte unter dem **Header Spezifikationen** rechts neben der Bezeichnung **Version** die **App-Version** aufgeführt werden.

![Erweiterte Optionen mit hervorgehobener App-Version geöffnet](images/app-version-img-03.png)

## <a name="in-client-logs"></a>In Clientprotokollen

AltspaceVR meldet die App-Version in der Clientprotokolldatei während des Anwendungsstarts als "Altspace-Version". Dies wäre eine gute Option zum Abrufen der App-Version, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber versucht haben, vor dem Fehlschlagen zu starten.

## <a name="windows"></a>Windows

Auf Windows befindet sich die Clientprotokolldatei über Windows Explorer unter:

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

Diese Datei wird jedes Mal überschrieben, wenn Sie AltspaceVR starten. "Player.log" stellt Ihre neueste Sitzung dar, und "Player-prev.log" stellt die vorherige Sitzung dar.

## <a name="via-powershell"></a>Über PowerShell

Fortgeschrittene Benutzer können die Clientprotokolle wie folgt über PowerShell nach dieser Zeichenfolge durchsuchen:

Eingabe:

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

Ausgabe:

[2.047] AltspaceVR Version: 3.2.23.e66c2