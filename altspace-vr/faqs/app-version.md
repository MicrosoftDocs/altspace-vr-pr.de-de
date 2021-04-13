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
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="2e0e0-104">Ermitteln der Version der altspacevr-App</span><span class="sxs-lookup"><span data-stu-id="2e0e0-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="2e0e0-105">Im Verlauf der Behebung eines Problems werden Sie möglicherweise gefragt, welche Version der altspacevr-App derzeit ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="2e0e0-106">In altspacevr</span><span class="sxs-lookup"><span data-stu-id="2e0e0-106">In AltspaceVR</span></span>

<span data-ttu-id="2e0e0-107">Navigieren Sie zum Suchen der App-Version in altspacevr zum **Menü "Einstellungen** ", **und wählen Sie** in der linken Navigationsleiste Info aus.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="2e0e0-108">Die "App-Version" wird hier angezeigt, wie im folgenden Screenshot gezeigt.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![Menü "Einstellungen" mit Infobereich geöffnet](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="2e0e0-110">In den Windows-System Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2e0e0-110">In Windows System Settings</span></span>

<span data-ttu-id="2e0e0-111">Wenn Sie altspacevr über das Microsoft Store installiert haben, können Sie die App-Version zusätzlich in den Windows-Systemeinstellungen finden.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="2e0e0-112">Dieses Szenario eignet sich gut zum Melden der App-Version, wenn Sie sich nicht erfolgreich beim Client anmelden können.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="2e0e0-113">Um die App-Version in den Windows-Systemeinstellungen zu finden, öffnen Sie das **Startmenü**, geben Sie **apps & Features** ein, und wählen Sie das Ergebnis aus.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="2e0e0-114">Navigieren Sie in der Liste der apps zu **altspacevr** .</span><span class="sxs-lookup"><span data-stu-id="2e0e0-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="2e0e0-115">Klicken Sie mit der linken Maustaste auf altspacevr, und wählen Sie im angezeigten Menü **Erweiterte Optionen** aus.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![Menü "Apps und Features" mit hervorgehobener erweiterte Option Öffnen](images/app-version-img-02.png)

<span data-ttu-id="2e0e0-117">In den **erweiterten Optionen** muss die **App-Version** unter dem **Spezifikationen** -Header rechts neben der **Versions** Bezeichnung aufgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![Erweiterte Optionen geöffnet mit hervorgehobener App-Version](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="2e0e0-119">In Client Protokollen</span><span class="sxs-lookup"><span data-stu-id="2e0e0-119">In Client Logs</span></span>

<span data-ttu-id="2e0e0-120">Altspacevr meldet die App-Version in der Client Protokolldatei beim Starten der Anwendung als "altspace-Version".</span><span class="sxs-lookup"><span data-stu-id="2e0e0-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="2e0e0-121">Dies wäre eine gute Option, um die App-Version zu erhalten, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber es wurde versucht, zu starten, bevor ein Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="2e0e0-122">Windows</span><span class="sxs-lookup"><span data-stu-id="2e0e0-122">Windows</span></span>

<span data-ttu-id="2e0e0-123">Unter Windows befindet sich die Client Protokolldatei über den Windows-Explorer unter:</span><span class="sxs-lookup"><span data-stu-id="2e0e0-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

<span data-ttu-id="2e0e0-124">Diese Datei wird jedes Mal überschrieben, wenn Sie "altspacevr" starten.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="2e0e0-125">"Player. log" stellt die neueste Sitzung dar, und "Player-Prev. log" stellt die vorherige Sitzung dar.</span><span class="sxs-lookup"><span data-stu-id="2e0e0-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="2e0e0-126">Über PowerShell</span><span class="sxs-lookup"><span data-stu-id="2e0e0-126">Via PowerShell</span></span>

<span data-ttu-id="2e0e0-127">Erweiterte Benutzer können die Client Protokolle für diese Zeichenfolge mithilfe von PowerShell wie folgt durchsuchen:</span><span class="sxs-lookup"><span data-stu-id="2e0e0-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="2e0e0-128">Eingabe:</span><span class="sxs-lookup"><span data-stu-id="2e0e0-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="2e0e0-129">Ausgabe:</span><span class="sxs-lookup"><span data-stu-id="2e0e0-129">Output:</span></span>

<span data-ttu-id="2e0e0-130">[2,047] altspacevr-Version: 3.2.23. e66c2</span><span class="sxs-lookup"><span data-stu-id="2e0e0-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>