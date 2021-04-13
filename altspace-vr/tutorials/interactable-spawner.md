---
title: Verwenden des-interactables-spawners
description: Erfahren Sie, wie Sie den interactables-Spawner erstellen, verwenden und anpassen, um Elemente in Ihrem altspacevr-Raum zu platzieren.
ms.date: 02/10/2021
ms.topic: article
keywords: Spawner, Interaktionen, Anpassungen
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213550"
---
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="ac519-104">Verwenden des-interactables-spawners</span><span class="sxs-lookup"><span data-stu-id="ac519-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="ac519-105">Der interactables Spawner ermöglicht Ihnen das Platzieren von Objekten, die sich in Ihrem Ereignis, in der Welt oder in der privatfläche befinden.</span><span class="sxs-lookup"><span data-stu-id="ac519-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="ac519-106">Diese Funktion ist zurzeit Teil des [frühen Zugriffs Programms](../world-building/early-access.md) und ist nur verfügbar, wenn Sie sich über Ihr Hauptmenü angemeldet haben.</span><span class="sxs-lookup"><span data-stu-id="ac519-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="ac519-107">Obwohl wir dieses Feature weiter testen, beachten Sie, dass das Erzeugen von zu vielen interactables möglicherweise die Leistung Ihrer Umgebung oder Ihres Ereignisses beeinträchtigt.</span><span class="sxs-lookup"><span data-stu-id="ac519-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="ac519-108">Erstellen einer Interaktionen</span><span class="sxs-lookup"><span data-stu-id="ac519-108">Creating an interactable</span></span>

<span data-ttu-id="ac519-109">So schalten Sie das Objekt in ein Objekt mit Interaktionen um:</span><span class="sxs-lookup"><span data-stu-id="ac519-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="ac519-110">Platzieren Sie das-Objekt in Ihrem Bereich.</span><span class="sxs-lookup"><span data-stu-id="ac519-110">Place the object in your space.</span></span>
2. <span data-ttu-id="ac519-111">Suchen Sie anschließend den Eintrag in der Objektliste, und wählen Sie das **Zahnrad Symbol** neben dem Eintrag aus, um die Einstellungen zu öffnen:</span><span class="sxs-lookup"><span data-stu-id="ac519-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![World Editor geöffnet mit hervorgehobener Objektliste](images/interactables-spawner-img-01.png)

<span data-ttu-id="ac519-113">Auf der Seite "Einstellungen" finden Sie das neue Kontrollkästchen **"Objekt Spawner"**, das verwendet wird, um es zu einem Objekt zu machen, das interacbar ist.</span><span class="sxs-lookup"><span data-stu-id="ac519-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="ac519-114">Aktivieren Sie das Kontrollkästchen, und klicken Sie auf **bestätigen**.</span><span class="sxs-lookup"><span data-stu-id="ac519-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="ac519-115">Im Bearbeitungsmodus können Sie den Speicherort des Objekts im Bereich verschieben.</span><span class="sxs-lookup"><span data-stu-id="ac519-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="ac519-116">**Beenden des Bearbeitungsmodus** zum Aktivieren der Element Interaktion.</span><span class="sxs-lookup"><span data-stu-id="ac519-116">**Exit edit mode** to enable item interaction.</span></span>

![Artefaktfenster in der altspacevr-APP öffnen](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="ac519-118">Weitere Anpassungen</span><span class="sxs-lookup"><span data-stu-id="ac519-118">Other customizations</span></span>

<span data-ttu-id="ac519-119">Nachdem Sie **"Object Spawner"** aktiviert haben, wenn Sie zu den Eigenschaften für dieses Objekt zurückkehren, gibt es eine zusätzliche Einstellung, die Sie auf die Art und Weise des erzeugten Objekts anwenden können.</span><span class="sxs-lookup"><span data-stu-id="ac519-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="ac519-120">Objekt Skala mit interactable: Hiermit wird die Skalierung des Objekts festgelegt, wenn es abgerufen wird, im Vergleich zu "Skalieren", bei der es sich um die Skalierung des Objekts in der Welt handelt, bevor es zum ersten mal abgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="ac519-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="ac519-121">Die Kit-Ersteller bemerken möglicherweise, dass Änderungen an Ihrem Kit, während altspacevr ausgeführt wird, erst nach einem Neustart von altspacevr wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="ac519-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="ac519-122">Vor kurzem haben wir auf der Registerkarte " **moderate Einstellungen** " eine Schaltfläche mit dem Namen " **Upload Worlds Kits**"</span><span class="sxs-lookup"><span data-stu-id="ac519-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="ac519-123">Wenn Sie auf diese Schaltfläche klicken, wird der Bereich erneut eingegeben, und alle Kits werden erneut geladen, sodass nur neue Versionen der Kits heruntergeladen werden, die während der Ausführung von altspacevr aktualisiert wurden.</span><span class="sxs-lookup"><span data-stu-id="ac519-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![Mittlerer Einstellungsbereich in der altspacevr-app geöffnet](images/interactables-spawner-img-03.png)