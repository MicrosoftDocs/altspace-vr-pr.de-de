---
title: Gewähren von Welt Rollen
description: Erfahren Sie mehr über das System "Rollen und Fähigkeiten" und erhalten Sie Schritt-für-Schritt-Anleitungen für die Bereitstellung von Benutzern in ihren altspacevr-Welten.
ms.date: 03/11/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212200"
---
# <a name="granting-world-roles"></a><span data-ttu-id="0d49f-104">Gewähren von Welt Rollen</span><span class="sxs-lookup"><span data-stu-id="0d49f-104">Granting world roles</span></span>

<span data-ttu-id="0d49f-105">In "altspace" ist ein System für Rollen und Fähigkeiten fest.</span><span class="sxs-lookup"><span data-stu-id="0d49f-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="0d49f-106">Jede Person kann über mehrere Rollen verfügen, und ihre Rollen können abhängig davon, wo Sie sich befinden, unterschiedlich sein.</span><span class="sxs-lookup"><span data-stu-id="0d49f-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="0d49f-107">Jede Rolle bietet Ihnen wiederum eine oder mehrere Funktionen.</span><span class="sxs-lookup"><span data-stu-id="0d49f-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="0d49f-108">Wenn Sie sich z. b. in Ihrem eigenen Ereignis befinden, erhalten Sie automatisch die **Presenter** -und **Moderator** -Rollen.</span><span class="sxs-lookup"><span data-stu-id="0d49f-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="0d49f-109">Mit diesen beiden Rollen können Sie unruly-Benutzer starten, sich in der Phase befinden und das-Programm möglicherweise freigeben.</span><span class="sxs-lookup"><span data-stu-id="0d49f-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="0d49f-110">Bearbeiten Sie Ihre Welt, und Scrollen Sie nach unten zum Abschnitt **in VR** ([Verwalten von Welten](managing-worlds.md)).</span><span class="sxs-lookup"><span data-stu-id="0d49f-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![Ändern von Rollen im VR-Abschnitt der Welten](images/granting-roles.png)

2. <span data-ttu-id="0d49f-112">Bearbeiten Sie das Feld " **Rollen** ", wenn Sie bestimmten Benutzern bestimmte Rollen nur für diese Welt gewähren möchten.</span><span class="sxs-lookup"><span data-stu-id="0d49f-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="0d49f-113">Wenn Sie z. b. **Presenter**  +  **Moderator** und Calen **Moderator** geben möchten, fügen Sie Folgendes hinzu, und wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="0d49f-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="0d49f-114">Das Format ist in jeder Zeile " **{Role}", "{username" oder "Email}** ".</span><span class="sxs-lookup"><span data-stu-id="0d49f-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="0d49f-115">Beim Benutzernamen wird die Groß-/Kleinschreibung</span><span class="sxs-lookup"><span data-stu-id="0d49f-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="0d49f-116">Wenn Sie erneut **Bearbeiten** auswählen, sollte Folgendes über dem Feld Rollen angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0d49f-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="0d49f-117">So haben Sie in der Datenbank aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0d49f-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="0d49f-118">Damit die Änderungen in altspace wirksam werden, sollten Sie die Welt zurücksetzen und alle wiederherstellen.</span><span class="sxs-lookup"><span data-stu-id="0d49f-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="0d49f-119">Unten finden Sie eine vollständige Liste der Rollen.</span><span class="sxs-lookup"><span data-stu-id="0d49f-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="0d49f-120">Bearbeiten Sie das Feld " **Kontext Rollen** ", wenn Sie jeder Rolle, die der Welt Beitritt, eine Rolle erteilen möchten.</span><span class="sxs-lookup"><span data-stu-id="0d49f-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="0d49f-121">Wenn Sie z. b. möchten, dass die Benutzer das Megafon ausführen und das Megafon verwenden können</span><span class="sxs-lookup"><span data-stu-id="0d49f-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="0d49f-122">Nachdem Sie **Aktualisieren** ausgewählt haben, setzen Sie die Welt zurück.</span><span class="sxs-lookup"><span data-stu-id="0d49f-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="0d49f-123">Dies wirkt sich nur auf diese Welt aus.</span><span class="sxs-lookup"><span data-stu-id="0d49f-123">This will only affect this World.</span></span> <span data-ttu-id="0d49f-124">Wenn Sie Rollen einem gesamten Universum zuweisen möchten, bearbeiten Sie die gleichen Felder im Universum.</span><span class="sxs-lookup"><span data-stu-id="0d49f-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="0d49f-125">Rollen</span><span class="sxs-lookup"><span data-stu-id="0d49f-125">Roles</span></span> 

* <span data-ttu-id="0d49f-126">**Presenter** -Funktionen wie die Bereitstellung auf der Stufe</span><span class="sxs-lookup"><span data-stu-id="0d49f-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="0d49f-127">**Moderator** : Funktionen wie " **Kick** " zur Wartung von Decorum</span><span class="sxs-lookup"><span data-stu-id="0d49f-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="0d49f-128">**Terraex** -Möglichkeit zur Verwendung des World-Editors</span><span class="sxs-lookup"><span data-stu-id="0d49f-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="0d49f-129">**Pilot Projekt** : Möglichkeit zum Umschalten des laufenden Modus und zum Erzeugen des 6DOF-Flight-Tools</span><span class="sxs-lookup"><span data-stu-id="0d49f-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="0d49f-130">**Megaphone_only** die Möglichkeit, in den Ohren von Benutzern zu sprechen, wo Sie sich auf der Welt befinden</span><span class="sxs-lookup"><span data-stu-id="0d49f-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="0d49f-131">**Showcase_new_sdk** Fähigkeit, MRE SDK-apps zu erzeugen</span><span class="sxs-lookup"><span data-stu-id="0d49f-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0d49f-132">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="0d49f-132">Troubleshooting</span></span>

<span data-ttu-id="0d49f-133">**Kann ich Rollen löschen?**</span><span class="sxs-lookup"><span data-stu-id="0d49f-133">**Can I delete roles?**</span></span>
<span data-ttu-id="0d49f-134">Nicht aus dem Formular zurzeit können Sie eine Supportanfrage unter Help.altvr.com, und wir kümmern uns um die Datei.</span><span class="sxs-lookup"><span data-stu-id="0d49f-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="0d49f-135">**Werden die Rollen kopiert, wenn eine Welt aus einer anderen importiert wird?**</span><span class="sxs-lookup"><span data-stu-id="0d49f-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="0d49f-136">Nein, Rollen werden nicht kopiert.</span><span class="sxs-lookup"><span data-stu-id="0d49f-136">No, roles aren't copied</span></span>