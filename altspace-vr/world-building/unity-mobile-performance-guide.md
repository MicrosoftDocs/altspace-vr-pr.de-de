---
title: AltspaceVR Mobile Performance Guide
description: Erfahren Sie, wie Sie verschiedene Unity-Eigenschaften verwenden, um Ihre Welten auf mobilen Geräten wie Oculus Quest leistungsbringend zu gestalten.
ms.date: 04/20/2021
ms.topic: article
keywords: World Editor, Performance, oculus, quest, unity, textures, lightmaps, stats, profiler, draw calls, altspacevr, uploader
ms.openlocfilehash: d5689e245c10ccb61abdd0aaa2327132d4374bb7e53a2eaec316d991b38378fb
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126981"
---
# <a name="altspacevr-mobile-performance-guide"></a>AltspaceVR Mobile Performance Guide

## <a name="main-points"></a>**Hauptpunkte:**

* **72 FPS** auf Oculus Quest 1 und 2 ist das Ziel.
* **Das Reduzieren von Draw-Aufrufen über statische Batchverarbeitung** ist unerlässlich und ist auf **weniger als 25 Drawcalls** ausgerichtet.
* **Ein Material pro Objekt** zur Unterstützung der statischen Batchverarbeitung (aufteilen von Objekten mit mehreren Materialien in separate Objekte).
* **Objekte** in einer Umgebung sollten in den meisten Fällen auf **"Statisch"** festgelegt werden.
* **Eine Lightmap pro Szene,** ein 2k oder ein 4k für die gesamte Szene, ca. 25 Texel pro Einheit, Lightmapskalierung sollte pro Objekt optimiert werden (Skalierungsdiagramm unten)
* **Verwenden Sie Shader in Mobile-Qualität** (d. h. "Mobil/Diffus" usw.), vermeiden Sie den Unity Standard-Shader/PBR/Reflektionstest/Lichttest, da es sich um umfangreiche Vorgänge handelt, und im Fall der Tests werden Draw-Aufrufe hinzugefügt.
* **Weniger als 100.000 Dreiecke** auf dem Bildschirm
* **Occlusion Culling** kann dazu beitragen, Polygone auf dem Bildschirm zu reduzieren, obwohl es im Voraus Kosten für die Aktivierung der Okklusion gibt. Messen Sie daher die Auswirkungen auf die Framerate in Altspace mithilfe des Diagnosebereichs.
* Verwenden Sie für alle **Texturen** in einer Szene **"Override for Android" (Außerkraftsetzung für Android),** und legen Sie sie auf **RGB(A) Compressed ASTC 6x6 block format fest.**  Belassen Sie ihre Android Build Einstellungen-Komprimierung auf den Standardwert (finden Sie unter: File/Build Einstellungen/Android/Texture Compression: 'Don't override'), damit Lightmaps keine ASTC-Komprimierung erhalten.  Indem wir die obigen Aufgaben ausführen und Materialien objektübergreifend freigeben, versuchen wir, das Unity-Paket unserer Szene für Android auf etwa **10-20 MB** zu halten.

Das allgemeine Ziel besteht darin, eine akzeptable Framerate geräteübergreifend zu erreichen. Auf Oculus Quest 1 und 2 wird die Szene idealerweise bei 72 FPS von allen Vantagepunkten ausgeführt, wenn die Szene aufgefüllt wird, obwohl ein Bereich von 60 bis 72 FPS häufig ein realistischeres Ziel ist.

Die Framerate kann in AltspaceVR auf dem Gerät gemessen werden, das Sie verwenden (in der AltspaceVR-App unter **Einstellungen/Support/Diagnosebereich anzeigen/FPS).**

Eine Rundown der verfügbaren Unity-Standardtools, die Ihnen helfen, Ihre Szenen besser zu optimieren:

## <a name="stats-panelframe-debuggerprofiler"></a>**Statistikbereich/Framedebugger/Profiler**

* Diese Tools sind Ihre besten Freunde bei der Verbesserung der Leistung Ihrer Szene.  Auf sie kann **nur verwiesen werden, während die Szene im Editor wiedergegeben wird,** da sich ihre Werte von denen unterscheiden, wenn die Szene nicht wiedergegeben wird (d. b. automatische statische Batchverarbeitung findet nicht statt, wenn die Szene nicht wiedergegeben wird).

* **Der Statistikbereich** (in der Spielansicht unter "Statistiken" angezeigt) zeigt die Menge der **gespeicherten Batches/Batches, SetPass-Aufrufe und Framerate** an.

    * Batches: Die Anzahl der aktuellen Zeichnen-Aufrufe, die aus Sicht der aktuellen Kamera sichtbar sind.  **Weniger als 25 Batches** für eine Umgebung sind ein gutes Ziel.
    * Gespeicherte Batches (nur sichtbar, wenn die Szene wiedergegeben wird) – die Anzahl der Draw-Aufrufe, die durch **statische Batchverarbeitung oder GPU-Instanziierung** reduziert wurden
    * SetPass-Aufrufe: Die Anzahl der verschiedenen sichtbaren Materialien in einer Szene
    * Framerate: die Menge der Frames pro Sekunde in der Spielansicht (gibt Ihnen eine ungefähre Vorstellung davon, was passiert; Szenen sollten immer in der App und im Headset getestet werden, indem Sie das Oculus Framerate-Panel verwenden, da sich das FPS-Readout immer von dem unterscheidet, was im Editor vorkommt).

* **Framedebugger** (finden Sie unter Fenster/Analyse/Framedebugger).  Im Bereich "Statistiken" können Sie bei Aktivierung sehen, was die GPU zeichnet, um das endgültige Bild zu erstellen, und eine Liste der Drawcalls vom ersten bis zum letzten Mal anzeigen.  Sie erhalten Gründe dafür, warum ein Draw-Aufruf nicht mit einem vorherigen Draw-Aufruf in Batches ausgeführt wurde (d. h. "Dieses Objekt verwendet ein anderes Material" oder "Dieses Objekt verwendet eine andere Lightmap"), und ist eine hervorragende Möglichkeit, um ein Verständnis dafür zu entwickeln, was in Ihrer Szene passiert und wie und warum bestimmte visuelle Optionen rechenintensiv sein können.

* **Profiler** zeigt Ihnen, welche Teile des Computers zu einem beliebigen Zeitpunkt verwendet werden, während das Spiel ausgeführt wird. Hilfreich bei der Ermittlung, wo die Leistung einen Engpass darstellt.  Wenn Sie z. B. eine hohe CPU-Auslastung in Ihrer Szene sehen, kann es sein, dass zu viele Zeichnen-Aufrufe vorhanden sind, oder wenn eine hohe GPU-Auslastung auftritt, kann es zu viele Überzeichnungen geben (d. b. die Anzahl der Renderzeiten eines einzelnen Pixels zum Erzeugen des endgültigen Bilds), was durch mehrere transparente Oberflächen verursacht werden kann.  - oder -Objekte, die nicht angezeigt werden, wenn sie nicht angezeigt werden.

## <a name="draw-calls-shadersmaterialsobjects"></a>**Zeichnen von Aufrufen (Shader/Materialien/Objekte)**

* Jedes Mal, wenn ein Shader, Material oder Objekt gerendert werden muss, muss die CPU die GPU des Schalters anweisen (auch als "Zeichnen-Aufrufe" bezeichnet, üblicherweise **"Drawcalls").**  Das heißt, wenn Sie über 5 Shader, 10 Materialien und 20 Objekte verfügen, mit dem größten; Sie verfügen über ungefähr 20 Drawcalls.  Andere Dinge, die Drawcalls multiplizieren können, sind das Verwenden von Objekten auf verschiedenen Lightmaps oder das Verwenden mehrerer Echtzeitlichts in einer Szene (d. h., ein Punktlicht fügt jedem Objekt, das sich innerhalb seines Bereichs befindet, einen weiteren Drawcall hinzu), sodass im Allgemeinen alles andere als das richtungsbezogene Licht einer Szene vermieden werden sollte.  Reflektions- und Lichtprüfpunkte multiplizieren auch Draw-Aufrufe für die Objekte, die sie treffen, sodass sie vermieden werden sollten.

* Bei der **statischen Batchverarbeitung** werden Objekte, die ähnliche Materialien gemeinsam nutzen, in einem einzelnen Objekt zusammengefasst, wenn sie an die GPU gesendet werden (wobei Occlusion Culling Gitternetze verwirft, die nicht angezeigt werden). Wenn Sie also alle Objekte im obigen Beispiel auf "Statisch" festlegen, würden Sie die Szene auf ungefähr 10 Drawcalls reduzieren, 1 für jedes Material. 

* **Materialbatches** treten auf, wenn ein Objekt über die genauen Materialien als ein anderes Objekt verfügt. Wenn ein Objekt jedoch über mehrere Materialien verfügt, wird es nicht mit einem Objekt, das weniger Materialien enthält, batchweise ausgeführt.  Aus diesem Grund: **Objekte DÜRFEN nur ein Material aufweisen,** und Objekte, die mehrere Materialien verwenden, sollten in separate Objekte pro Material aufgeteilt werden.  **Materialbatches** können durch **Texturat atlasing** reduziert werden (kombiniert die Texturen mehrerer eindeutiger Objekte, um ein einzelnes Texturblatt zu teilen, sodass alle das gleiche Material verwenden).  Versuchen Sie, die Menge von Atlases nach Möglichkeit auf eine einzelne 2k- oder 4k-Textur/material pro Szene zu halten.

## <a name="scene-complexity"></a>**Szenenkomplexität**

* **Geometrie:** Versuchen Sie, Bildschirmdreiecke für Umgebungen unter 100.000 beizubehalten.  Verwenden Sie die Registerkarte "Statistiken" im Spielbereich von Unity, um zu sehen, welche Dreiecksanzahl Sie von verschiedenen Vantagepunkten in der Szene erreichen.  Props als solche sollten sich im Bereich "Hunderte" von Dreiecken mit nur wichtigen "Hero"-Props im Tausenderbereich von Dreiecken befindet. 

* Sie können **LODs** (Detailgitternetzebene) technisch verwenden, obwohl die Standardmäßige Lightmaplösung von Unity keine Lightmapdaten zwischen LODs teilt, sodass Sie möglicherweise Lightmappingartefakte erhalten, wenn die LODs bei dieser Auflösung wechseln.  Alternativ können Sie die LOD-Gruppenkomponente auch dann für einfache Distance Culling-Objekte verwenden, wenn das Objekt keine niedrigeren LOD-Gitternetze besitzt:

![LOD-Gruppenfenster in Unity](images/world-building-lod-Group.png)

* **Occlusion Culling** reduziert die Anzahl der Objekte, die nur auf das gerendert werden, was sich innerhalb des Sicht-Frustums der Kamera befindet, und die sofort sichtbar sind (d.amp;quot;Objekte, die aus der Ansicht verdeckt werden, sind Culled.)  Occlusion culling sollte fast immer für Ihre Szene gebacken werden, und Ebenen sollten so entworfen werden, dass sie diese unterstützen (d. h. wenn Sie über eine große Ebene verfügen, können Wände oder große Objekte verwendet werden, um die Sichtlinie des Spielers aufzubrechen, sodass sie nicht immer bis zum entgegengesetzten Ende der Ebene durchsehen können.  Die Standardeinstellungen für bake sollten funktionieren, obwohl Sie möglicherweise die Werte "Smallest Occluder" oder "Smallest Hole" verkleinern müssen.  Für Objekte wie Zäunen, bei denen Sie möglicherweise Risse im Objekt oder transparente Objekte sehen können, sollten Sie den Occluder-Status des Objekts im Dropdownmenü "Statisch" deaktivieren, damit die darin enthaltenen Objekte nicht fälschlicherweise verdeckt werden. 

## <a name="lightmaps"></a>**Lightmaps**

* Idealerweise nur **eine Lightmap pro Szene** (ein 2k oder ein 4k für alles), falls nicht; Weniger Lightmaps mit höheren Auflösungen sind besser als viele Lightmaps mit niedrigeren Auflösungen.
* Mehrere Lightmaps können sich auch auf die Anzahl der Zeichnen-Aufrufe auswirken, da Objekte, die entweder Lightmaps haben oder nicht, sich in unterschiedlichen Batches befinden und andere Lightmaps sich ebenfalls in unterschiedlichen Batches befinden.
* Im Allgemeinen sollte eine Lightmap-Auflösung von etwa **25 Texel pro Einheit** ausreichen (auflösung in den Einstellungen für Beleuchtung/Szene festlegen).  Wenn Sie zusätzlichen Platz in Ihrer Lightmap haben, können Sie diesen Wert erhöhen.
* Ändern Sie die **Lightmap-Skalierungseinstellung** pro Objekt, sodass die Auflösung für Objekte gespeichert wird, die sie benötigen. 

* **Lightmap-Skalierungsdiagramm** (Faustregel) 
    * **Vordergrund** (geografischer Durchlaufgrad): 1 
    * **Props** (insbesondere Props kleiner als ein Mensch): **2-3** (um Lightmapartefakte und Naht auf Ihren Objekten zu vermeiden) 
    * **Midground** (Geometrie, die sich direkt außerhalb des Durchlaufbereichs und/oder großer Objekte wie Gebäude befindet): **0,5**
    * **Hintergrund** (Vista-/entfernte Objekte): **0,02** 
    * **Transparente Oberflächen** (z.B. Glass): **0** (mit deaktivierter Option "Cast/Receive Shadows") 

Außerdem sind hier einige Einstellungen, die für die Screen Door Effect-Umgebung verwendet wurden, als Baseline:

![Beleuchtungsfenster in Unity](images/world-building-lightmaps.png)

Hinweis: Wenn Sie diese Einstellungen verwenden, können Sie lightmapper auf "GPU Lightmapper" festlegen und die Lightmap-Größe für wesentlich schnellere Vorschau-Bakes auf "2048" festlegen und dann für ihren endgültigen Bake auf CPU und 4k sichern.

## <a name="texture-compressionfile-size"></a>**Texturkomprimierung/Dateigröße**

* Für unseren Android-Build versuchen wir, die Größe der Unity-Paketszene auf insgesamt etwa 10 bis 20 MB zu halten.  Dies geschieht, indem wir generische Materialien für viele Objekte freigeben, die Scheitelpunktfarbe verwenden, um die Objekte zu tönen, und indem wir manuelle Außerkraftsetzungen für Android festlegen, sodass Texturen die **ASTC 6x6-Blockkomprimierung** verwenden, die kleiner als die Standardkomprimierung ist.

* Der Grund dafür, dass wir die Android-Buildeinstellungen nicht für die Verwendung von ASTC festlegen, liegt daran, dass Lightmaps mit dieser Komprimierung nicht gut aussehen (viele Blockartefakte), und wir müssten die Lightmap so festlegen, dass sie ETC nach jedem Bake verwendet. Daher ist es einfacher, die Außerkraftsetzung für alle Szenentexturen einmal einzurichten, als die Komprimierungseinstellungen der Lightmap nach jedem Bake zu aktualisieren.

![Texturfenster in Unity](images/world-building-texutres.png)

* Darüber hinaus kann das Festlegen von Texturen für die Verwendung des trilinearen Filtermodus mit einer Anisotropeebene von 2 dazu beitragen, dass sie in spitzen Winkeln bleiben.

Weitere Tipps und Tricks zur Leistung finden Sie in der Dokumentation Improving world performance (Verbessern der [Weltleistung).](improving-performance.md)
