---
title: Suchen der AltspaceVR-App-Version
description: Erfahren Sie, wie Sie die AltspaceVR-App, Einstellungen und Clientprotokolle verwenden, um die aktuell ausgeführte Version von AltspaceVR zu finden.
ms.date: 02/10/2021
ms.topic: article
keywords: App-Version
ms.openlocfilehash: 6b710e1724b890fa7ba0eecfcd774ef63128d5b7
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923177"
---
# <a name="finding-the-altspacevr-app-version"></a>Suchen der AltspaceVR-App-Version

Im Zuge der Problembehandlung werden Sie möglicherweise gefragt, welche Version der AltspaceVR-App Sie gerade ausführen.

## <a name="in-altspacevr"></a>In AltspaceVR

Um die App-Version in AltspaceVR zu finden, navigieren Sie zum Einstellungsmenü, **und** wählen Sie **in** der linken Navigationsleiste About aus. Die "App-Version" wird hier gemeldet, wie im folgenden Screenshot gezeigt.

![Menü "Einstellungen" mit geöffneten "About"-Panel geöffnet](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>In den Windows-Systemeinstellungen

Wenn Sie AltspaceVR über die Microsoft Store installiert haben, finden Sie zusätzlich die App-Version in den Windows-Systemeinstellungen.  Dieses Szenario ist gut geeignet, wenn Sie die App-Version melden, wenn Sie sich nicht erfolgreich beim Client anmelden können.

Um die App-Version in den Windows-Systemeinstellungen zu finden, öffnen Sie das **Startmenü,** geben Sie Apps & **Features** ein, und wählen Sie das Ergebnis aus. Navigieren Sie in der Liste der Apps zu **AltspaceVR.** Klicken Sie mit der linken Maustaste auf AltspaceVR, und wählen **Sie im** angezeigten Menü Erweiterte Optionen aus.

![Menü "Apps und Features" mit hervorgehobener Option "Erweitert" geöffnet](images/app-version-img-02.png)

In den **erweiterten Optionen** unter dem **Header Spezifikationen** sollte die **App-Version** rechts neben der Bezeichnung **Version aufgeführt** werden.

![Erweiterte Optionen mit hervorgehobener App-Version geöffnet](images/app-version-img-03.png)

## <a name="in-client-logs"></a>In Clientprotokollen

AltspaceVR meldet die App-Version in der Clientprotokolldatei während des Anwendungsstarts als "ALTSPACE-Version". Dies wäre eine gute Option, um die App-Version zu erhalten, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber es wurde versucht, vor dem Fehler zu starten.

## <a name="windows"></a>Windows

Unter Windows finden Sie die Clientprotokolldatei über Windows-Explorer:

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