---
title: Gewähren von World-Rollen
description: Erfahren Sie mehr über das Rollen- und Fähigkeitssystem, und erhalten Sie schritt-für-Schritt-Anweisungen zum Zuweisen von Rollen für Benutzer in Ihren AltspaceVR-Welten.
ms.date: 04/14/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923192"
---
# <a name="granting-world-roles"></a><span data-ttu-id="bd012-104">Gewähren von World-Rollen</span><span class="sxs-lookup"><span data-stu-id="bd012-104">Granting world roles</span></span>

<span data-ttu-id="bd012-105">Altspace verfügt über ein Rollen- und Fähigkeitssystem.</span><span class="sxs-lookup"><span data-stu-id="bd012-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="bd012-106">Jede Person kann über mehrere Rollen verfügen, und ihre Rollen können sich je nach Ihrem Ort unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="bd012-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="bd012-107">Jede Rolle wiederum bietet Ihnen eine oder mehrere Fähigkeiten.</span><span class="sxs-lookup"><span data-stu-id="bd012-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="bd012-108">Wenn Sie sich beispielsweise in Ihrem eigenen Ereignis sind, erhalten Sie automatisch die **Host-** und **Moderatorrollen.**</span><span class="sxs-lookup"><span data-stu-id="bd012-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="bd012-109">Mit diesen beiden Rollen können Sie unbändige Benutzer starten, auf der Stage sein und die Conf conf zu veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="bd012-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="bd012-110">Bearbeiten Sie Ihre Welt, und sehen Sie sich die rechte Spalte für **Kontextrollen** [(Verwalten von Welten) an.](managing-worlds.md)</span><span class="sxs-lookup"><span data-stu-id="bd012-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![Ändern von Rollen im Abschnitt "Kontextrollen" von Welten](images/granting-roles.png)

2. <span data-ttu-id="bd012-112">Klicken **Sie im Feld** **Kontextrollen** auf Benutzer hinzufügen, wenn Sie bestimmten Benutzern nur für diese Welt bestimmte Rollen zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="bd012-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="bd012-113">Wenn Sie mir z. B. host moderator **geben** möchten, fügen Sie  +  den oben genannten hinzu, und wählen Sie **Speichern aus.**</span><span class="sxs-lookup"><span data-stu-id="bd012-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="bd012-114">Das Format ist **Benutzername,** bei Benutzername wird die Groß-/Kleinschreibung nicht beachtet. Wählen Sie die Rolle im Dropdownmenü **Terraformer** aus, klicken Sie mehrmals auf Benutzer hinzufügen, um weitere Benutzer hinzuzufügen, und klicken Sie dann **auf Aktualisieren.**</span><span class="sxs-lookup"><span data-stu-id="bd012-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="bd012-115">Damit die Änderung in Altspace wirksam wird, sollten Sie "Space the world" zurücksetzen, um alle Benutzer zu zwingen, wieder dabei zu sein oder jeden Benutzer mit einer neuen Rolle wieder in die Welt zu nehmen.</span><span class="sxs-lookup"><span data-stu-id="bd012-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="bd012-116">Bearbeiten Sie **das Feld Standardmäßige** kontextbezogene Rollen im Abschnitt **In VR,** wenn Sie jeder Rolle, die Ihrer Welt beitritt, eine Rolle zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="bd012-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="bd012-117">Wenn Sie z. B. personen das Megaphone zum Fliegt und verwenden möchten, damit sie sich im fernen Teil hören können, fügen Sie Folgendes hinzu:</span><span class="sxs-lookup"><span data-stu-id="bd012-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="bd012-118">Nachdem Sie Aktualisieren **ausgewählt haben,** setzen Sie den Speicherplatz in der Welt zurück.</span><span class="sxs-lookup"><span data-stu-id="bd012-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="bd012-119">Dies wirkt sich nur auf diese Welt aus.</span><span class="sxs-lookup"><span data-stu-id="bd012-119">This will only affect this World.</span></span> <span data-ttu-id="bd012-120">Wenn Sie einem gesamten Universe Rollen zuweisen möchten, bearbeiten Sie die gleichen Felder im Universe.</span><span class="sxs-lookup"><span data-stu-id="bd012-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="bd012-121">Dasselbe gilt für Ereignisse. Wenn Sie möchten, dass alle Benutzer in Ihrem Ereignis über diese Rollen verfügen, müssen Sie diese zu den **Standardkontexrollen** des Ereignisses selbst hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="bd012-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="bd012-122">Rollen</span><span class="sxs-lookup"><span data-stu-id="bd012-122">Roles</span></span>

* <span data-ttu-id="bd012-123">**Megaphone_only:** Möglichkeit, überall auf der Welt in die Menschen zu sprechen</span><span class="sxs-lookup"><span data-stu-id="bd012-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="bd012-124">**Moderator:** Fähigkeiten wie **"Kick"** zum Verwalten des Anstands</span><span class="sxs-lookup"><span data-stu-id="bd012-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="bd012-125">**Pilot:** Möglichkeit zum Umschalten des Flymodus und Zum Erstellen des 6DOF-Flugtools</span><span class="sxs-lookup"><span data-stu-id="bd012-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="bd012-126">**Host:** Fähigkeiten wie die Möglichkeit, auf der Stage zu sein, megaphone</span><span class="sxs-lookup"><span data-stu-id="bd012-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="bd012-127">**Terraformer:** Möglichkeit, den World Editor zu verwenden Weitere Informationen zu ( Rollen in Ereignissen, Welten, Gruppen und [in AltspaceVR](../getting-started/roles.md))</span><span class="sxs-lookup"><span data-stu-id="bd012-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="bd012-128">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="bd012-128">Troubleshooting</span></span>

<span data-ttu-id="bd012-129">**Kann ich Rollen löschen?**</span><span class="sxs-lookup"><span data-stu-id="bd012-129">**Can I delete roles?**</span></span>
<span data-ttu-id="bd012-130">Ja, bearbeiten Sie Ihre Welt, klicken Sie **unterhalb** der Rolle, die Sie löschen möchten, auf Entfernen, und klicken Sie auf **Aktualisieren.**</span><span class="sxs-lookup"><span data-stu-id="bd012-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="bd012-131">**Werden Rollen kopiert, wenn eine Welt aus einer anderen importiert wird?**</span><span class="sxs-lookup"><span data-stu-id="bd012-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="bd012-132">Nein, Rollen werden nicht kopiert.</span><span class="sxs-lookup"><span data-stu-id="bd012-132">No, roles aren't copied</span></span>