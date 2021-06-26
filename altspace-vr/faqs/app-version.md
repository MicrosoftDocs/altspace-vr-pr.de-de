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
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="23151-104">Suchen der AltspaceVR-App-Version</span><span class="sxs-lookup"><span data-stu-id="23151-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="23151-105">Im Zuge der Problembehandlung werden Sie möglicherweise gefragt, welche Version der AltspaceVR-App Sie gerade ausführen.</span><span class="sxs-lookup"><span data-stu-id="23151-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="23151-106">In AltspaceVR</span><span class="sxs-lookup"><span data-stu-id="23151-106">In AltspaceVR</span></span>

<span data-ttu-id="23151-107">Um die App-Version in AltspaceVR zu finden, navigieren Sie zum Einstellungsmenü, **und** wählen Sie **in** der linken Navigationsleiste About aus.</span><span class="sxs-lookup"><span data-stu-id="23151-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="23151-108">Die "App-Version" wird hier gemeldet, wie im folgenden Screenshot gezeigt.</span><span class="sxs-lookup"><span data-stu-id="23151-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![Menü "Einstellungen" mit geöffneten "About"-Panel geöffnet](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="23151-110">In den Windows-Systemeinstellungen</span><span class="sxs-lookup"><span data-stu-id="23151-110">In Windows System Settings</span></span>

<span data-ttu-id="23151-111">Wenn Sie AltspaceVR über die Microsoft Store installiert haben, finden Sie zusätzlich die App-Version in den Windows-Systemeinstellungen.</span><span class="sxs-lookup"><span data-stu-id="23151-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="23151-112">Dieses Szenario ist gut geeignet, wenn Sie die App-Version melden, wenn Sie sich nicht erfolgreich beim Client anmelden können.</span><span class="sxs-lookup"><span data-stu-id="23151-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="23151-113">Um die App-Version in den Windows-Systemeinstellungen zu finden, öffnen Sie das **Startmenü,** geben Sie Apps & **Features** ein, und wählen Sie das Ergebnis aus.</span><span class="sxs-lookup"><span data-stu-id="23151-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="23151-114">Navigieren Sie in der Liste der Apps zu **AltspaceVR.**</span><span class="sxs-lookup"><span data-stu-id="23151-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="23151-115">Klicken Sie mit der linken Maustaste auf AltspaceVR, und wählen **Sie im** angezeigten Menü Erweiterte Optionen aus.</span><span class="sxs-lookup"><span data-stu-id="23151-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![Menü "Apps und Features" mit hervorgehobener Option "Erweitert" geöffnet](images/app-version-img-02.png)

<span data-ttu-id="23151-117">In den **erweiterten Optionen** unter dem **Header Spezifikationen** sollte die **App-Version** rechts neben der Bezeichnung **Version aufgeführt** werden.</span><span class="sxs-lookup"><span data-stu-id="23151-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![Erweiterte Optionen mit hervorgehobener App-Version geöffnet](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="23151-119">In Clientprotokollen</span><span class="sxs-lookup"><span data-stu-id="23151-119">In Client Logs</span></span>

<span data-ttu-id="23151-120">AltspaceVR meldet die App-Version in der Clientprotokolldatei während des Anwendungsstarts als "ALTSPACE-Version".</span><span class="sxs-lookup"><span data-stu-id="23151-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="23151-121">Dies wäre eine gute Option, um die App-Version zu erhalten, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber es wurde versucht, vor dem Fehler zu starten.</span><span class="sxs-lookup"><span data-stu-id="23151-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="23151-122">Windows</span><span class="sxs-lookup"><span data-stu-id="23151-122">Windows</span></span>

<span data-ttu-id="23151-123">Unter Windows finden Sie die Clientprotokolldatei über Windows-Explorer:</span><span class="sxs-lookup"><span data-stu-id="23151-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

<span data-ttu-id="23151-124">Diese Datei wird jedes Mal überschrieben, wenn Sie AltspaceVR starten.</span><span class="sxs-lookup"><span data-stu-id="23151-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="23151-125">"Player.log" stellt Ihre neueste Sitzung dar, und "Player-prev.log" stellt die vorherige Sitzung dar.</span><span class="sxs-lookup"><span data-stu-id="23151-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="23151-126">Über PowerShell</span><span class="sxs-lookup"><span data-stu-id="23151-126">Via PowerShell</span></span>

<span data-ttu-id="23151-127">Fortgeschrittene Benutzer können die Clientprotokolle wie folgt über PowerShell nach dieser Zeichenfolge durchsuchen:</span><span class="sxs-lookup"><span data-stu-id="23151-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="23151-128">Eingabe:</span><span class="sxs-lookup"><span data-stu-id="23151-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="23151-129">Ausgabe:</span><span class="sxs-lookup"><span data-stu-id="23151-129">Output:</span></span>

<span data-ttu-id="23151-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span><span class="sxs-lookup"><span data-stu-id="23151-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>