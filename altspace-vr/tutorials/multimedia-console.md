---
title: Verwenden der Multimediakonsole
description: Erfahren Sie, wie Sie mit dem Konfigurieren, Veröffentlichen und Steuern der Multimediakonsole in Ihren AltspaceVR-Funktionen beginnen.
ms.date: 03/11/2021
ms.topic: article
keywords: Konsole, Multimedia
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923007"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="2a2bc-104">Verwenden der Multimediakonsole</span><span class="sxs-lookup"><span data-stu-id="2a2bc-104">Using the multimedia console</span></span>

<span data-ttu-id="2a2bc-105">Die Multimediakonsole ist ein Tool, das die Medienfreigabe in Ereignissen und Welten ermöglicht.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="2a2bc-106">Sie können damit u. a. Bilder, Präsentationsfolien, Livestreams, Videos, Wiedergabelisten und vieles mehr freigeben.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="2a2bc-107">Im Folgenden finden Sie eine schrittweise Anleitung zur Verwendung der Multimedia-Konsole **v0.5.0+**.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="2a2bc-108">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="2a2bc-108">Getting started</span></span>

<span data-ttu-id="2a2bc-109">Die ersten Schritte mit der Multimediakonsole sind ein zweiteiler Prozess.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="2a2bc-110">Zuerst gibt es das Webportal, mit dem Sie eine Konfiguration für die Multimediakonsolensitzung generieren und veröffentlichen, die Sie in Ihrer Umgebung platzieren.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="2a2bc-111">Das zweite ist die Platzierung der eigentlichen Multimediakonsolen-App in Ihrer Umgebung und das Festlegen des Konfigurationscodes, den sie verwenden soll.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="2a2bc-112">Konfigurieren der Multimediakonsole mit dem Webportal</span><span class="sxs-lookup"><span data-stu-id="2a2bc-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="2a2bc-113">Zunächst müssen Sie sicherstellen, dass Ihre Inhalte online gehostet werden, da Sie eine URL benötigen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="2a2bc-114">(Sie können Fotos in altvr.com hochladen, ein Video .mp4 Datei online hosten oder einen Dlive-Livestreamlink verwenden: https://dlive.tv/yourlivestream)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-114">(You can upload photos to altvr.com, host a video .mp4 file online or use a Dlive live stream link: https://dlive.tv/yourlivestream)</span></span> 
2. <span data-ttu-id="2a2bc-115">Navigieren Sie zum Webportal für die Multimediakonsole unter . [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="2a2bc-116">Über das Webportal können Sie eine Konfiguration für die Multimediakonsole generieren und veröffentlichen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="2a2bc-117">(Weitere Informationen zu den verschiedenen Eigenschaften finden Sie unten.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="2a2bc-118">Nachdem Sie die Medien in die Medienliste eingegeben und die allgemeinen Einstellungen konfiguriert haben, wählen Sie oben rechts in der App die Schaltfläche Veröffentlichen aus.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="2a2bc-119">Sobald die Veröffentlichung abgeschlossen ist, wird ein Dialogfeld mit einem Zwei-Wort-Code angezeigt, den Sie in die von Ihnen platzierte Multimediakonsole eingeben können.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="2a2bc-120">Platzieren der Multimediakonsole in Ihrer Umgebung</span><span class="sxs-lookup"><span data-stu-id="2a2bc-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="2a2bc-121">Wählen Sie **> Editor-Bereich > SDK-Apps > Multimedia-Konsole** die Option World Editor aus.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="2a2bc-122">(Wechseln Sie nicht zu **World Editor > Basics > SDK-App**, die für nicht registrierte Apps gilt.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="2a2bc-123">Positionieren Sie die Multimediakonsole so, dass Ihr Raum und Ihre Zielgruppe am besten geeignet sind.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="2a2bc-124">Wechseln Sie aus dem Bearbeitungsmodus, indem Sie auf die orangefarbene Schaltfläche Edit Mode (Bearbeitungsmodus) klicken.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="2a2bc-125">Sie werden **gefragt, sind Sie der Besitzer des Media Player?**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="2a2bc-126">Wenn Sie die Person sind, die der offizielle Besitzer dieser Multimediakonsolensitzung sein soll, bestätigen Sie dies, und fahren Sie fort.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="2a2bc-127">(Weitere rollenberechtigungen sind ebenfalls verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="2a2bc-128">Eine ausführliche Liste finden Sie unten.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="2a2bc-129">Wählen Sie Ja aus, um zu bestätigen, dass Sie der primäre Host sind.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="2a2bc-130">Es sollte ein Dialogfeld angezeigt werden, in dem Sie aufgefordert werden, einen Code aus dem Webportal oder gültigen JSON-Code einzugeben.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="2a2bc-131">Geben Sie den Zwei-Wort-Code aus dem Webportal ein, einschließlich des Bindestrichs, und drücken Sie OK.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="2a2bc-132">(JSON ist eine weiter unten beschriebene erweiterte Konfiguration.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="2a2bc-133">Die Multimediakonsole sollte nach einigen Sekunden mit der Konfiguration geladen werden, die Sie im Webportal erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="2a2bc-134">Steuern der Multimediakonsole</span><span class="sxs-lookup"><span data-stu-id="2a2bc-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="2a2bc-135">Nachdem Sie Ihren Code eingegeben und den Konfigurationsprozess abgeschlossen haben, werden Steuerelementschaltflächen unterhalb einer Medienanzeige angezeigt.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="2a2bc-136">**Wiedergabe** startet den Medien-Viewer (oder startet beim aktuellen Eintrag neu, falls er zuvor beendet wurde)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="2a2bc-137">**Beenden** beendet die Medienanzeige und blendet aktuelle Medien aus.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="2a2bc-138">**Next/Prev** überspringt das nächste oder vorherige Medium.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="2a2bc-139">**x/x**   zeigt den aktuellen Index in der Medienliste an und ermöglicht es Ihnen, zu einem beliebigen Punkt in der Liste zu springen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="2a2bc-140">**Die Konfiguration** ermöglicht das erneute Eingeben eines neuen Codes aus dem Webportal, um eine neue Konfiguration in der Konsole festzulegen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="2a2bc-141">Jetzt können Sie mit der Freigabe über die Multimediakonsole beginnen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="2a2bc-142">Arbeiten mit dem Webportal</span><span class="sxs-lookup"><span data-stu-id="2a2bc-142">Working with the web portal</span></span>

<span data-ttu-id="2a2bc-143">Das Webportal ist eine Web-App, mit der die verschiedenen Funktionen der Multimediakonsole konfiguriert werden können.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="2a2bc-144">Diese Features lassen sich in zwei Kategorien unterteilen: Allgemeine Medienkonsoleneinstellungen und die Medienwiedergabeliste.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="2a2bc-145">Allgemeine Einstellungen der Multimediakonsole</span><span class="sxs-lookup"><span data-stu-id="2a2bc-145">Multimedia console general settings</span></span>

<span data-ttu-id="2a2bc-146">**Wiedergabeeinstellungen**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-146">**Playback Settings**</span></span>

<span data-ttu-id="2a2bc-147">Allgemeine Wiedergabeeinstellungen für die Medienliste</span><span class="sxs-lookup"><span data-stu-id="2a2bc-147">General playback settings for the media list</span></span>

* <span data-ttu-id="2a2bc-148">**Schleifenmedienliste:** Bestimmt, ob die Medienliste eine Schleife durchlaufen soll, sobald Sie das Ende der Liste erreicht haben.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="2a2bc-149">**Methode starten:** Wählt die Methode aus, mit der die Multimediakonsole gestartet werden soll.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="2a2bc-150">Manuell: Wartet, bis die Wiedergabeschaltfläche gedrückt wird, bevor das Medium gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="2a2bc-151">Automatisch von Anfang starten: Starten Sie die Medienliste automatisch am Anfang der Liste.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="2a2bc-152">Auto Start Random : Startet die Medien automatisch von einem zufälligen Startpunkt in der Liste</span><span class="sxs-lookup"><span data-stu-id="2a2bc-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="2a2bc-153">**Rollen**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-153">**Roles**</span></span>

<span data-ttu-id="2a2bc-154">Rollenzuweisungen zum Steuern und Konfigurieren der Multimediakonsole.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="2a2bc-155">Diese Rollen sind in folgende Gruppe unterteilt:</span><span class="sxs-lookup"><span data-stu-id="2a2bc-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="2a2bc-156">**Nur Besitzer:** Der Benutzer, der Besitzer der Multimediakonsolensitzung ist</span><span class="sxs-lookup"><span data-stu-id="2a2bc-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="2a2bc-157">Benutzer mit **erhöhten Rechten:** Benutzer mit Moderator- oder Hostrollen in dem Bereich, in dem die Multimediakonsole ursprünglich konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="2a2bc-157">**Elevated Users** - Users that have moderator or host roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="2a2bc-158">**Alle Benutzer** – Alle Benutzer</span><span class="sxs-lookup"><span data-stu-id="2a2bc-158">**All Users** - All users</span></span>

<span data-ttu-id="2a2bc-159">Diese Rollen stapeln sich in dem Sinne, dass allen Rollen, die über der in dieser Liste ausgewählten Rolle liegen, auch die Berechtigung zum Verwenden dieses Features erteilt wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="2a2bc-160">Beispiel: Benutzer mit **erhöhten Rechten** enthalten den **Besitzer,** auch wenn sie kein Moderator oder Host\*\* in AltspaceVR sind.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator or host\*\* in AltspaceVR.</span></span> <span data-ttu-id="2a2bc-161">Funktionen, die durch Rollenzuweisungen gesteuert werden, sind wie folgt:</span><span class="sxs-lookup"><span data-stu-id="2a2bc-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="2a2bc-162">**Kann den Medienplayer steuern:** Bestimmt, welche Rollen die Medienwiedergabeschaltflächen für die Multimediakonsole steuern können.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="2a2bc-163">**Kann den Media Player konfigurieren:** Bestimmt, welche Rollen die Multimediakonsole konfigurieren können, indem Zugriff auf die Schaltfläche **"Konfiguration"** gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="2a2bc-164">Hinzufügen von Fotos und Videos zur Medienliste</span><span class="sxs-lookup"><span data-stu-id="2a2bc-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="2a2bc-165">Medien sind das Kernstück der Multimediakonsole.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="2a2bc-166">Bilder und Videolinks werden in der Multimediakonsole als Medientypen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="2a2bc-167">Um neue Medien hinzuzufügen, wählen Sie entweder das Symbol **Bild hinzufügen** oder **Video hinzufügen** aus, damit ein Dialogfeld angezeigt wird, in dem die Medieninformationen und -einstellungen eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="2a2bc-168">Im Folgenden finden Sie eine Aufschlüsselung der Medientypen und der zugehörigen Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="2a2bc-169">**Image**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-169">**Image**</span></span>

<span data-ttu-id="2a2bc-170">Bilder sollten ein Standardbildtyp wie jpeg, png und son on sein.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="2a2bc-171">Sie müssen an einem Ort mit einem öffentlichen Link gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="2a2bc-172">**Name:** (Erforderlich) Der Name, mit dem Sie das Bild identifizieren möchten.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="2a2bc-173">**Bild-URL** – (erforderlich) Die öffentliche URL des Bilds</span><span class="sxs-lookup"><span data-stu-id="2a2bc-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="2a2bc-174">**Überspringen nach:** Die Anzahl von Sekunden, nach der das Bild übersprungen werden soll</span><span class="sxs-lookup"><span data-stu-id="2a2bc-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="2a2bc-175">**Video**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-175">**Video**</span></span>

<span data-ttu-id="2a2bc-176">Videos können über Twitch und DLive gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="2a2bc-177">(Andere Unterstützung kann mit zusätzlichem Aufwand funktionieren, um die richtige Stream-URL abzurufen, wird jedoch nicht vollständig in der Multimediakonsole unterstützt.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="2a2bc-178">**Name:** (Erforderlich) Der Name, mit dem Sie das Video identifizieren möchten.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="2a2bc-179">**Video-URL** : (Erforderlich) Die öffentliche URL, unter der das Video gehostet wird oder von der aus der Livestream bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="2a2bc-180">**Überspringen nach** : Die Anzahl von Sekunden, nach der das Video übersprungen werden soll</span><span class="sxs-lookup"><span data-stu-id="2a2bc-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>

> [!NOTE]
> <span data-ttu-id="2a2bc-181">ERFORDERLICH: Geben Sie die Zeit ein, die der Länge des Videos entspricht, damit Videos ordnungsgemäß weitergeleitet werden können.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-181">REQUIRED: Put in the time that matches the length of the video to enable videos to properly forward.</span></span> <span data-ttu-id="2a2bc-182">Wenn Ihr Video beispielsweise 5 Minuten lang ist, legen Sie 300 Sekunden ein, andernfalls wird Ihr Video nicht mit dem nächsten Inhaltsteil übersprungen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-182">For example, if your video is 5 minutes long put 300 seconds, otherwise your video won't skip to the next piece of content.</span></span>

* <span data-ttu-id="2a2bc-183">**Volume:** Das Videovolumen von 0 (min) bis 1 (max) Werten.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-183">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="2a2bc-184">**Startzeit:** Die Anzahl von Sekunden ab dem Anfang des Videos.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-184">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="2a2bc-185">**Roll Off Start Distance** :Die Entfernung in Metern auf der Welt, bei der das Volumen abfällt, wenn Sie sich von der Multimediakonsole wegbewegt haben.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-185">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="2a2bc-186">**Videoendeaktion:** Die Aktion, die nach Erreichen des Videoendes erfolgen soll.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-186">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="2a2bc-187">Beenden: Die Medienliste wird beendet, nachdem das Video beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-187">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="2a2bc-188">Schleife: Das Video führt eine Schleife durch, bis es manuell übersprungen wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-188">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="2a2bc-189">Weiter wiedergeben: Die nächsten Medien in der Medienliste werden gestartet, nachdem das aktuelle Video beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-189">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="2a2bc-190">Direktes Arbeiten mit JSON (erweitert/optional)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-190">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="2a2bc-191">Die Multimediakonsole unterstützt das direkte Eingeben von JSON in die Eingabeaufforderung der Konsole in AltspaceVR.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-191">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="2a2bc-192">JSON ist der interne Mechanismus, mit dem Media Player-Konfigurationen aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-192">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="2a2bc-193">Die Möglichkeit, JSON direkt festzulegen, ermöglicht es erweiterten Benutzern, ihre eigenen Workflows zu erstellen, die ihre Anforderungen erfüllen und mit JSON vertraut sind.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-193">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="2a2bc-194">Es folgt eine kurze Beschreibung der JSON-Struktur und des Schemas, nach dem der JSON-Code überprüft wird.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-194">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="2a2bc-195">Ausführlichere Beschreibungen der folgenden Eigenschaften finden Sie in den obigen Abschnitten zum Konfigurieren der Multimediakonsole.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-195">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="2a2bc-196">Dieser Abschnitt konzentriert sich hauptsächlich auf die Schemabeispiele und die Strukturierung für die JSON-Daten.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-196">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="2a2bc-197">Globale Medieneinstellungen</span><span class="sxs-lookup"><span data-stu-id="2a2bc-197">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="2a2bc-198">Medienliste</span><span class="sxs-lookup"><span data-stu-id="2a2bc-198">Media list</span></span>

<span data-ttu-id="2a2bc-199">Die Medienliste ist eine Eigenschaft, die im Stammverzeichnis der JSON-Struktur festgelegt ist, z. B. Rollen und Wiedergabeeinstellungen.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-199">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="2a2bc-200">Es ist ein einfaches Array, das eine der folgenden Medienkonfigurationsstrukturen enthalten kann.</span><span class="sxs-lookup"><span data-stu-id="2a2bc-200">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="2a2bc-201">(Ausführliche Informationen zu den einzelnen Eigenschaften finden Sie oben in den Eigenschaftenbeschreibungen.)</span><span class="sxs-lookup"><span data-stu-id="2a2bc-201">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="2a2bc-202">**Bildbeispiel**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-202">**Image example**</span></span>

<span data-ttu-id="2a2bc-203">*Erforderliche Felder: "name" und "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="2a2bc-203">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="2a2bc-204">**Videobeispiel**</span><span class="sxs-lookup"><span data-stu-id="2a2bc-204">**Video example**</span></span>

<span data-ttu-id="2a2bc-205">*Erforderliche Felder: "name" und "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="2a2bc-205">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="2a2bc-206">JSON-Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a2bc-206">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="2a2bc-207">Schema</span><span class="sxs-lookup"><span data-stu-id="2a2bc-207">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="2a2bc-208">Aktuelle Version von Multimedia Console v0.5.0</span><span class="sxs-lookup"><span data-stu-id="2a2bc-208">Up to date with Multimedia Console v0.5.0</span></span>