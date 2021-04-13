---
title: Ermitteln der Version der altspacevr-App
description: Erfahren Sie, wie Sie die altspacevr-APP, Einstellungen und Client Protokolle verwenden, um die Version von altspacevr zu ermitteln, die Sie gerade ausführen.
ms.date: 02/10/2021
ms.topic: article
keywords: App-Version
ms.openlocfilehash: 5d503d3b89cd213696dd53616c5c7e3013aeef01
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213182"
---
# <a name="finding-the-altspacevr-app-version"></a>Ermitteln der Version der altspacevr-App

Im Verlauf der Behebung eines Problems werden Sie möglicherweise gefragt, welche Version der altspacevr-App derzeit ausgeführt wird.

## <a name="in-altspacevr"></a>In altspacevr

Navigieren Sie zum Suchen der App-Version in altspacevr zum **Menü "Einstellungen** ", **und wählen Sie** in der linken Navigationsleiste Info aus. Die "App-Version" wird hier angezeigt, wie im folgenden Screenshot gezeigt.

![Menü "Einstellungen" mit Infobereich geöffnet](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>In den Windows-System Einstellungen

Wenn Sie altspacevr über das Microsoft Store installiert haben, können Sie die App-Version zusätzlich in den Windows-Systemeinstellungen finden.  Dieses Szenario eignet sich gut zum Melden der App-Version, wenn Sie sich nicht erfolgreich beim Client anmelden können.

Um die App-Version in den Windows-Systemeinstellungen zu finden, öffnen Sie das **Startmenü**, geben Sie **apps & Features** ein, und wählen Sie das Ergebnis aus. Navigieren Sie in der Liste der apps zu **altspacevr** . Klicken Sie mit der linken Maustaste auf altspacevr, und wählen Sie im angezeigten Menü **Erweiterte Optionen** aus.

![Menü "Apps und Features" mit hervorgehobener erweiterte Option Öffnen](images/app-version-img-02.png)

In den **erweiterten Optionen** muss die **App-Version** unter dem **Spezifikationen** -Header rechts neben der **Versions** Bezeichnung aufgeführt werden.

![Erweiterte Optionen geöffnet mit hervorgehobener App-Version](images/app-version-img-03.png)

## <a name="in-client-logs"></a>In Client Protokollen

Altspacevr meldet die App-Version in der Client Protokolldatei beim Starten der Anwendung als "altspace-Version". Dies wäre eine gute Option, um die App-Version zu erhalten, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber es wurde versucht, zu starten, bevor ein Fehler aufgetreten ist.

## <a name="windows"></a>Windows

Unter Windows befindet sich die Client Protokolldatei über den Windows-Explorer unter:

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

Diese Datei wird jedes Mal überschrieben, wenn Sie "altspacevr" starten. "Player. log" stellt die neueste Sitzung dar, und "Player-Prev. log" stellt die vorherige Sitzung dar.

## <a name="via-powershell"></a>Über PowerShell

Erweiterte Benutzer können die Client Protokolle für diese Zeichenfolge mithilfe von PowerShell wie folgt durchsuchen:

Eingabe:

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

Ausgabe:

[2,047] altspacevr-Version: 3.2.23. e66c2