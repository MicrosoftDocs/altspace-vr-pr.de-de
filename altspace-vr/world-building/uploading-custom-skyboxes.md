---
title: Hochladen von benutzerdefinierten Skyboxes
description: Hier finden Sie Schritt-für-Schritt-Anleitungen zum Hochladen und behandeln von benutzerdefinierten Skyboxes-Vorgängen in altspacevr.
ms.date: 03/11/2021
ms.topic: article
keywords: Skyboxes, Problembehandlung
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213262"
---
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="6ae72-104">Hochladen von benutzerdefinierten Skyboxes</span><span class="sxs-lookup"><span data-stu-id="6ae72-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="6ae72-105">Eine Skybox ist eine Möglichkeit, einen **Hintergrund** für Ihre Welt zu erstellen, der die Erfahrung verbessert.</span><span class="sxs-lookup"><span data-stu-id="6ae72-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="6ae72-106">Es gibt unterschiedliche Arten von Skyboxes, aber wir unterstützen derzeit **equirecht eckige** Felder.</span><span class="sxs-lookup"><span data-stu-id="6ae72-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="6ae72-107">Hier sehen Sie ein Beispiel mit einer 360-Kamera (Weitere Beispiele [finden Sie hier](http://moments.mankindforward.com/)):</span><span class="sxs-lookup"><span data-stu-id="6ae72-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![360 equirecht eckige Ansicht eines Wohnraums](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="6ae72-109">Sie können auch das [Unity-Uploader](world-building-toolkit-getting-started.md) verwenden, aber dieser Ansatz ist einfacher.</span><span class="sxs-lookup"><span data-stu-id="6ae72-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="6ae72-110">Navigieren Sie zu [Worlds > Skyboxes](https://account.altvr.com/skyboxes) , und klicken Sie auf der rechten Seite auf die Schaltfläche **Erstellen**</span><span class="sxs-lookup"><span data-stu-id="6ae72-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![Die Seite "Website" ist für das Skyboxes-Panel](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="6ae72-112">Geben Sie einen Namen ein, und geben Sie Ihr 360-Image an.</span><span class="sxs-lookup"><span data-stu-id="6ae72-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="6ae72-113">Es muss kein Foto sein, es gibt Programme, mit denen Sie Ihre eigenen erstellen können, oder Sie können nach einigen Online suchen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="6ae72-114">Wählen Sie **Erstellen** aus, wenn Sie fertig sind.</span><span class="sxs-lookup"><span data-stu-id="6ae72-114">When you're ready, select **Create**.</span></span> 

![Erstellungs Formular für Skybox](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="6ae72-116">Optional können Sie ein **Vorschaubild** hochladen, damit Sie diese Skybox problemlos identifizieren können.</span><span class="sxs-lookup"><span data-stu-id="6ae72-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="6ae72-117">Sie können Ambient-Audiodaten auch im WAV-Format hochladen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="6ae72-118">Es wird empfohlen, Vorschau Bilder und Ambient-Audiodaten separat hochzuladen, nachdem Sie das 360-Image hochgeladen haben.</span><span class="sxs-lookup"><span data-stu-id="6ae72-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="6ae72-119">Wenn Sie Sie hochladen, können die Dateigrößen groß genug sein, um den Prozess zu stoppen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="6ae72-120">[Jegsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) ist ein gutes Beispiel für die Verwendung von Skybox mit Ambient-Audiodaten.</span><span class="sxs-lookup"><span data-stu-id="6ae72-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="6ae72-121">Beachten Sie, dass der Welt-Generator das audiovolume niedrig gehalten hat, und Klänge, die Sie hören, sind sporadisch, damit Menschen nicht verärgert werden.</span><span class="sxs-lookup"><span data-stu-id="6ae72-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="6ae72-122">Geben Sie Ihre Welt ein, und öffnen Sie den World-Editor.</span><span class="sxs-lookup"><span data-stu-id="6ae72-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="6ae72-123">Wählen Sie unter Skyboxes die neue Skybox aus.</span><span class="sxs-lookup"><span data-stu-id="6ae72-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="6ae72-124">Innerhalb weniger Sekunden wird der Himmel buchstäblich geändert.</span><span class="sxs-lookup"><span data-stu-id="6ae72-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="6ae72-125">Andere Benutzer in ihrer Welt sehen auch die Änderung am Himmel.</span><span class="sxs-lookup"><span data-stu-id="6ae72-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="6ae72-126">Um zurückzukehren, wählen Sie die **Standard** -Skybox in der gleichen Liste aus.</span><span class="sxs-lookup"><span data-stu-id="6ae72-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="6ae72-127">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="6ae72-127">Troubleshooting</span></span>

<span data-ttu-id="6ae72-128">**Es gibt eine Naht oder eine Linie im Himmel:-(.**</span><span class="sxs-lookup"><span data-stu-id="6ae72-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="6ae72-129">Es handelt sich um einen Fehler, den wir bald beheben werden.</span><span class="sxs-lookup"><span data-stu-id="6ae72-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="6ae72-130">**Fehler beim Hochladen.**</span><span class="sxs-lookup"><span data-stu-id="6ae72-130">**Upload failed**</span></span>
    * <span data-ttu-id="6ae72-131">versuchen Sie, nur das 360-Image eigenständig hochzuladen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="6ae72-132">versuchen Sie es mit einer anderen, kleineren Datei als Test.</span><span class="sxs-lookup"><span data-stu-id="6ae72-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="6ae72-133">**Ich kann ein 360-Foto nicht finden.**</span><span class="sxs-lookup"><span data-stu-id="6ae72-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="6ae72-134">Flickr ist eine gute Quelle (ändern Sie die Filter, um Creative Commons zu finden)</span><span class="sxs-lookup"><span data-stu-id="6ae72-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="6ae72-135">Nehmen Sie Ihre eigenen!</span><span class="sxs-lookup"><span data-stu-id="6ae72-135">Take your own!</span></span> <span data-ttu-id="6ae72-136">Die Kameras von Ricoh waren erfolgreich.</span><span class="sxs-lookup"><span data-stu-id="6ae72-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="6ae72-137">**Der Himmel sieht grau oder grobe aus** . Möglicherweise müssen Sie ein Bild mit höherer Auflösung suchen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="6ae72-138">Üblicherweise ca. 2-5 MB und ~ 5000 px x 2000 px</span><span class="sxs-lookup"><span data-stu-id="6ae72-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="6ae72-139">**Die Framerate meiner Welt!**</span><span class="sxs-lookup"><span data-stu-id="6ae72-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="6ae72-140">Das Image ist wahrscheinlich zu groß.</span><span class="sxs-lookup"><span data-stu-id="6ae72-140">The image is probably too large.</span></span> <span data-ttu-id="6ae72-141">Einige generierte Skyboxes können 8 KB betragen.</span><span class="sxs-lookup"><span data-stu-id="6ae72-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="6ae72-142">Sie sind in der Regel mit Mobil funkfreundlichen 2K-Versionen ausgestattet. verwenden Sie diese Version.</span><span class="sxs-lookup"><span data-stu-id="6ae72-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="6ae72-143">**Hilfe bei der Ambient-Audiodatei**</span><span class="sxs-lookup"><span data-stu-id="6ae72-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="6ae72-144">Verwenden Sie die kostenlose Software, wie z. b. Audacity, um das Volume zu verringern oder eigene Schleifen</span><span class="sxs-lookup"><span data-stu-id="6ae72-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="6ae72-145">Denken Sie daran, dass das Audiomaterial wiederholt wird und in den Ohren der Menschen wiedergegeben wird.</span><span class="sxs-lookup"><span data-stu-id="6ae72-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="6ae72-146">Der [freie Sound](https://freesound.org/) ist eine gute Quelle für kostenlose Sounds.</span><span class="sxs-lookup"><span data-stu-id="6ae72-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
