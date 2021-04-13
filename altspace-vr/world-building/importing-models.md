---
title: Importieren von gltf-Modellen
description: Erfahren Sie, wie Sie 3D-gltf-Modelle ordnungsgemäß in Ihre altspacevr-Erfahrungen importieren und Probleme beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Modelle, gltf, Import, schräl, Problembehandlung
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213259"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="cd633-104">Importieren von gltf-Modellen</span><span class="sxs-lookup"><span data-stu-id="cd633-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="cd633-105">Diese Funktion ist zurzeit für ausgewählte Benutzer im frühzeitigen Zugriffs Programm verfügbar.</span><span class="sxs-lookup"><span data-stu-id="cd633-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="cd633-106">Eine Möglichkeit zum bringen von 3D-Modellen und-Szenen in altspace ist die Verwendung des [gltf-Standards](https://en.wikipedia.org/wiki/GlTF).</span><span class="sxs-lookup"><span data-stu-id="cd633-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="cd633-107">Sie können eine GLB-Datei (gepacktes gltf) hochladen, um ein Modell zu erstellen, das Sie später im World-Editor erzeugen können.</span><span class="sxs-lookup"><span data-stu-id="cd633-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="cd633-108">Es ist eine Alternative zum [Hochladen Ihrer eigenen Kits](uploading-custom-kits.md).</span><span class="sxs-lookup"><span data-stu-id="cd633-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="cd633-109">Wir empfehlen die Erstellung von Modellen für schnelle Demos, da Sie Unity nicht verwenden müssen, und Kits, wenn Sie die Leistung und Wiederverwendbarkeit maximieren möchten.</span><span class="sxs-lookup"><span data-stu-id="cd633-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="cd633-110">Suchen Sie nach einigen gltf 3D-Assets.</span><span class="sxs-lookup"><span data-stu-id="cd633-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="cd633-111">Ein Ort für die Suche ist "schrätchfab" (Filtern Sie nach **herunterladbaren** Modellen wie [diesem](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span><span class="sxs-lookup"><span data-stu-id="cd633-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="cd633-112">Wenn Sie ihn gefunden haben, wählen Sie **3D-Modell herunterladen** aus:</span><span class="sxs-lookup"><span data-stu-id="cd633-112">Once you find it, select **Download 3D Model**:</span></span>

![3D-Hunde Modell aus "schrätchfab"](images/importing-models-img-01.png)

2. <span data-ttu-id="cd633-114">Kopieren Sie den Link in das Modell, und lesen Sie die Lizenzanforderungen.</span><span class="sxs-lookup"><span data-stu-id="cd633-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="cd633-115">Herunterladen der Version des **Auto konvertierten Formats (gltf)**</span><span class="sxs-lookup"><span data-stu-id="cd633-115">Download the **Autoconverted Format (glTF)** version</span></span>

![Optionen zum Herunterladen von "schrätchfab" mit hervorgehobenem Format](images/importing-models-img-02.png)

4. <span data-ttu-id="cd633-117">Öffnen Sie die [GLB Packer](https://glb-packer.glitch.me) -Website, und aktivieren Sie das Kontrollkästchen **PNG in JPEG konvertieren (Beta)** .</span><span class="sxs-lookup"><span data-stu-id="cd633-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="cd633-118">Deinstalkomprimieren Sie die heruntergeladenen gltf-Dateien, und ziehen Sie Sie nacheinander auf die Browser Registerkarte GLB Packer.</span><span class="sxs-lookup"><span data-stu-id="cd633-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![Fenster mit unkomprimierung des Modells](images/importing-models-img-03.png)

6. <span data-ttu-id="cd633-120&quot;>Abhängig von der Anzahl und Größe der Dateien kann es eine Weile dauern, bis Sie verarbeitet wird.</span><span class=&quot;sxs-lookup&quot;><span data-stu-id=&quot;cd633-120&quot;>Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id=&quot;cd633-121&quot;>Wenn die Verarbeitung abgeschlossen ist, wird eine **out. GLB** -Datei heruntergeladen.</span><span class=&quot;sxs-lookup&quot;><span data-stu-id=&quot;cd633-121&quot;>When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id=&quot;cd633-122&quot;>Benennen Sie diese Datei in eine informative Datei um. Dies ist der Name des Objekts auf der Welt (z **. b. &quot;Low Poly. GLB**").</span><span class="sxs-lookup"><span data-stu-id="cd633-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="cd633-123">Navigieren Sie zu [altvr.com > weitere > Modelle](https://account.altvr.com/users/sign_in) , und wählen Sie **Erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="cd633-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="cd633-124">Geben Sie den Speicherort der GLB-Datei an, und stellen Sie sicher, dass Sie den Link "schrätchfab" in die Beschreibung für die Zuordnung kopieren.</span><span class="sxs-lookup"><span data-stu-id="cd633-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="cd633-125">Wenn Sie möchten, können Sie ein Vorschaubild angeben und dann **Modell erstellen** auswählen:</span><span class="sxs-lookup"><span data-stu-id="cd633-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![Modell Vorschau in altspacevr](images/importing-models-img-04.png)

9. <span data-ttu-id="cd633-127">**In Zwischenablage kopieren** auswählen</span><span class="sxs-lookup"><span data-stu-id="cd633-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="cd633-128">Öffnen des **World Editors > altspace > Grundlagen > gltf**</span><span class="sxs-lookup"><span data-stu-id="cd633-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="cd633-129">Fügen Sie die URL ein, und wählen Sie **bestätigen** aus.</span><span class="sxs-lookup"><span data-stu-id="cd633-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="cd633-130">Herzlichen Glückwunsch!</span><span class="sxs-lookup"><span data-stu-id="cd633-130">Congrats!</span></span> <span data-ttu-id="cd633-131">Sie haben soeben das erste Modell erzeugt.</span><span class="sxs-lookup"><span data-stu-id="cd633-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="cd633-132">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="cd633-132">Troubleshooting</span></span>

<span data-ttu-id="cd633-133">**Beim Anklicken **bestätigen** , dass nichts passiert ist**</span><span class="sxs-lookup"><span data-stu-id="cd633-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="cd633-134">Wir haben derzeit ein Polygon Limit von 100 KB.</span><span class="sxs-lookup"><span data-stu-id="cd633-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="cd633-135">Wenn dies nicht möglich ist, löschen Sie das Objekt, um potenzielle Probleme mit Benutzern zu vermeiden, die ihrer Welt beitreten</span><span class="sxs-lookup"><span data-stu-id="cd633-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="cd633-136">Möglicherweise gibt es andere Probleme mit dem Asset.</span><span class="sxs-lookup"><span data-stu-id="cd633-136">There may be other problems with the asset.</span></span> <span data-ttu-id="cd633-137">Versuchen Sie, Ressourcen mit möglichst wenigen Polygonen zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="cd633-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="cd633-138">Das Modell, das Sie einbinden, kann klein oder groß sein.</span><span class="sxs-lookup"><span data-stu-id="cd633-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="cd633-139">Versuchen Sie, die Skalierung zu vergrößern oder zu verringern oder den Avatar zu verschieben. möglicherweise sind Sie im Modell.</span><span class="sxs-lookup"><span data-stu-id="cd633-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="cd633-140">**Die Auslastung ist langsam** . Wie schnell andere Benutzer weltweit laden, hängt von der Verbindungsgeschwindigkeit ab.</span><span class="sxs-lookup"><span data-stu-id="cd633-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="cd633-141">Sie wird auch nicht wie Kit-Assets zwischengespeichert.</span><span class="sxs-lookup"><span data-stu-id="cd633-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="cd633-142">Wenn Sie einen in Ihrem Zuhause platzieren, können Sie das gleiche Modell jedes Mal erneut herunterladen, wenn Sie beitreten, was nicht gut ist.</span><span class="sxs-lookup"><span data-stu-id="cd633-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="cd633-143">**Es gibt keine Kollision** . Standardmäßig gibt es keine Konflikte mit den Objekten, die auf diese Weise eingeführt werden.</span><span class="sxs-lookup"><span data-stu-id="cd633-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="cd633-144">**Wenn ich Sie verwende, verliere ich meine Steuerelemente auf sechs DOF-Daten, oder ich bin darin, dass es schwierig ist, Sie zu bearbeiten** . Ja, wir kennen diese Probleme und hoffen, Sie bald zu beheben.</span><span class="sxs-lookup"><span data-stu-id="cd633-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  