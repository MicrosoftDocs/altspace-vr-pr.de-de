---
title: AltspaceVR Mobile Performance Guide
description: Erfahren Sie, wie Sie verschiedene Unity-Eigenschaften verwenden, um Ihre Welten auf mobilen Geräten wie Oculus Quest leistunglich zu machen.
ms.date: 04/20/2021
ms.topic: article
keywords: World Editor, Performance, Oculus, Quest, Unity, Texturen, Lightmaps, Statistiken, Profiler, Zeichnen-Aufrufe, altspacevr, uploader
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
* **Das Reduzieren von Zeichnen-Aufrufen** über statische Batchverarbeitung ist von entscheidender Bedeutung und zielt auf **weniger als 25 Drawcalls ab.**
* **Ein Material pro Objekt, um** die statische Batchverarbeitung zu fördern (mehrere Materialobjekte in separate Objekte aufteilen).
* **Objekte** in einer Umgebung sollten in den meisten Fällen **auf "Statisch"** festgelegt werden.
* **Ein Lightmap** pro Szene, ein 2.000 oder ein 4.000 für die gesamte Szene, ca. 25 Texel pro Einheit. Die Lightmapskalierung sollte pro Objekt optimiert werden (Skalierungsdiagramm unten).
* Verwenden Sie Shader in mobiler Qualität (d. h. "Mobil/Diffus" usw.), vermeiden Sie die Unity-Standard-Shader-/PBR-/Reflektions-/Licht-Tests, da es sich um hohe Vorgänge handelt und im Fall der Tests **Zeichnen-Aufrufe** hinzugefügt werden.
* **Weniger als 100.000 Dreiecke** auf dem Bildschirm
* **Occlusion Culling** kann dazu beitragen, Polygone auf dem Bildschirm zu reduzieren, obwohl die Aktivierung von Okklusions-Culling im Vorweg kosten muss. Messen Sie daher die Auswirkungen auf die Framerate im Altspace mithilfe des Diagnosebereichs.
* Verwenden Sie **für alle Texturen** in einer Szene **"Override for Android",** und legen Sie sie auf **RGB(A) Compressed ASTC 6x6 block format (RGB(A)-komprimiertes ASTC 6x6-Blockformat fest.**  Lassen Sie ihre Android Build Einstellungen-Komprimierung auf den Standardwert festgelegt (siehe Datei/Build Einstellungen/Android/Texturkomprimierung: 'Nicht überschreiben'), damit Lightmaps keine ASTC-Komprimierung erhalten.  Indem wir die oben genannten Und-Materialien objektübergreifend freigeben, versuchen wir, das Unity-Paket unserer Szene für Android auf ca. **10-20 MB zu halten.**

Das allgemeine Ziel besteht im Erreichen einer akzeptablen Framerate auf allen Geräten– bei Oculus Quest 1 und 2 wird die Szene idealerweise bei 72 FPS von allen Vantagepunkten aus ausgeführt, wenn die Szene aufgefüllt ist, obwohl ein Bereich von 60-72 FPS häufig ein realistischeres Ziel ist.

Die Framerate kann in AltspaceVR auf dem gerät gemessen werden, das Sie verwenden (in der AltspaceVR-App unter **Einstellungen/Support/Diagnosebereich anzeigen/FPS**).

Ein Rundown der verfügbaren Unity-Standardtools, mit deren Hilfe Sie Ihre Szenen besser optimieren können:

## <a name="stats-panelframe-debuggerprofiler"></a>**Statistikbereich/Framedebugger/Profiler**

* Diese Tools sind Ihre besten Freunde bei der Verbesserung der Leistung Ihrer Szene.  Auf sie kann nur verwiesen werden, während die Szene Im Editor **spielt,** da sich ihre Werte von denen unterscheiden, wenn die Szene nicht abspielt (d. h., die automatische statische Batchverarbeitung findet nicht statt, wenn die Szene nicht abspielt).

* **Im Statistikbereich** (in der Spielansicht unter "Statistiken") wird die Menge der gespeicherten **Batches/Batches, SetPass-Aufrufe und Framerate angezeigt.**

    * Batches: Die Menge der aktuellen Zeichnen-Aufrufe, die aus sicht der aktuellen Kamera sichtbar sind.  **Weniger als 25 Batches für** eine Umgebung sind ein gutes Ziel.
    * Gespeicherte Batches (nur sichtbar, wenn die Szene abspielt) – die Menge der Zeichnen-Aufrufe, die durch statische Batchverarbeitung oder **GPU-Instancing reduziert wurden**
    * SetPass-Aufrufe– die Anzahl der verschiedenen sichtbaren Materialien in einer Szene
    * Framerate: Die Menge der Frames pro Sekunde in der Spielansicht (bietet Ihnen eine ungefähre Vorstellung davon, was passiert. Szenen sollten immer in der App und im Headset getestet werden, indem sie den Oculus Framerate-Bereich verwenden, da sich die Fps-Leseauslese immer von dem im Editor unterscheiden wird)

* **FrameDebugger** (unter Fenster-/Analyse-/Framedebugger)  Der Statistikbereich für Tafeln, mit dem Sie nach der Aktivierung sehen können, welche GPU gezeichnungt wird, um das endgültige Bild zu erstellen. Es wird eine Liste mit Drawcalls vom ersten bis zum letzten Bild angezeigt.  Es gibt Ihnen Gründe dafür, warum ein Zeichnen-Aufruf nicht mit einem vorherigen Zeichnen-Aufruf (d. h. "Dieses Objekt verwendet ein anderes Material" oder "Dieses Objekt verwendet eine andere Lightmap") als Batch verwendet wurde, und ist eine hervorragende Möglichkeit, um ein Verständnis dafür zu entwickeln, was in Ihrer Szene passiert und wie und warum bestimmte visuelle Optionen rechenintensiv sein können.

* **Profiler** zeigt Ihnen, welche Teile des Computers zu einem beliebigen Zeitpunkt verwendet werden, während das Spiel ausgeführt wird. Hilfreich bei der Ermittlung, wo die Leistung Engpässe verursacht.  Wenn Sie beispielsweise eine hohe CPU-Auslastung in Ihrer Szene sehen, kann es sein, dass zu viele Zeichnen-Aufrufe ausgeführt werden, oder wenn sie eine hohe GPU-Auslastung sehen, kann es zu viel Überzeichnung (d. h. die Anzahl der Renderung eines einzelnen Pixels zum Erzeugen des endgültigen Bilds) kommen, was durch mehrere transparente Oberflächen verursacht werden kann.  - oder -Objekte, die nicht gecullt werden, wenn sie nicht angezeigt werden.

## <a name="draw-calls-shadersmaterialsobjects"></a>**Zeichnen von Aufrufen (Shader/Materialien/Objekte)**

* Jedes Mal, wenn ein Shader, Material oder Objekt gerendert werden muss, muss die CPU die GPU des Switches anweisen (auch als "Zeichnen-Aufrufe" bezeichnet, **umgangssprachlich "Drawcalls").**  Das heißt, wenn Sie über 5 Shader, 10 Materialien und 20 Objekte verfügen, mit welchem am besten ist. Sie verfügen über ungefähr 20 Drawcalls.  Andere Dinge, die Drawcalls multiplizieren können, sind das Verwenden von Objekten auf unterschiedlichen Lightmaps oder das Verwenden von mehr als einem Echtzeitlicht in einer Szene (d.h. ein Punktlicht fügt jedem Objekt, das sich innerhalb seines Bereichs befindet, einen weiteren Zeichnencall hinzu). Daher sollte im Allgemeinen alles, was nicht das direktionale Licht einer Szene ist, vermieden werden.  Reflektions- und Licht-Tests multiplizieren auch Zeichnen-Aufrufe für die Objekte, auf die sie treffen, sodass sie vermieden werden sollten.

* Bei der **statischen Batchverarbeitung** werden Objekte, die Like-Materials gemeinsam nutzen, in ein einzelnes Objekt gebatcht, wenn sie an die GPU gesendet werden (mit verwirften Verschlussgittern, die Gitternetze verwerfen, die nicht angezeigt werden). Wenn Sie also alle Objekte im obigen Beispiel auf "Statisch" festlegen, würden Sie die Szene auf ungefähr 10 Drawcalls reduzieren, 1 für jedes Material. 

* **Materialbatches** treten auf, wenn ein Objekt über die genauen Materialien als ein anderes Objekt verfügt. Wenn ein Objekt jedoch über mehrere Materialien verfügt, wird es nicht mit einem Objekt batchen, das weniger Materialien enthält.  Aus diesem Grund: **Objekte DÜRFEN nur ein Material** enthalten, und Objekte, die mehrere Materialien verwenden, sollten in separate Objekte pro Material aufgeteilt werden.  **Materialbatches können** durch **Texture Atlasing** reduziert werden (indem die Texturen mehrerer eindeutiger Objekte kombiniert werden, um ein einzelnes Texturblatt gemeinsam zu verwenden, sodass alle das gleiche Material verwenden).  Versuchen Sie, die Menge an Atlases nach Möglichkeit auf eine einzelne 2k- oder 4k-Textur/ein einzelnes Material pro Szene zu halten.

## <a name="scene-complexity"></a>**Komplexität der Szene**

* **Geometrie:** Versuchen Sie, die Dreiecke auf dem Bildschirm für Umgebungen unter 100.000 zu halten.  Verwenden Sie die Registerkarte "Statistiken" im Unity-Spielbereich, um zu sehen, welche Dreiecksanzahl Sie von verschiedenen Vantagepunkten in der Szene aus treffen.  "Props" als solche sollten im Bereich "Hunderte" von Dreiecken liegen, mit nur wichtigen "Hero"-Props im Tausenden von Dreieckenbereich. 

* Technisch gesehen können Sie **LODs** (Level of Detail Meshes) verwenden, obwohl die Standardmäßige Lightmap-Lösung von Unity keine Lightmapdaten zwischen LODs gemeinsam nutzt, sodass Sie möglicherweise lightmapping-Artefakte erhalten, wenn die LODs bei dieser Auflösung wechseln.  Alternativ können Sie die LOD-Gruppenkomponente für einfache Distance Culling-Objekte verwenden, auch wenn das Objekt keine niedrigeren LOD-Gitternetze hat:

![Fenster "LOD-Gruppe" in Unity](images/world-building-lod-Group.png)

* **Occlusion Culling** reduziert die Anzahl der Objekte, die nur auf das gerendert werden, was sich innerhalb des Ansichtsfrustums der Kamera befindet und sofort sichtbar sind (d. h. Objekte, die aus der Ansicht verdecken, werden gecullt).  Occlusion culling sollte fast immer für Ihre Szene gebacken werden, und Ebenen sollten so entworfen werden, dass sie unterstützt werden (d. h., wenn Sie über eine große Ebene verfügen, können Wände oder große Objekte verwendet werden, um die Sichtlinie des Spielers zu unterbrechen, damit sie nicht immer bis zum gegenüberliegenden Ende der Ebene durchgeblickt werden können.  Die standardmäßigen Bake-Einstellungen sollten funktionieren, obwohl Sie möglicherweise die Werte "Kleinstes Occluder" oder "Smallest Hole" verkleinern müssen.  Für Objekte wie Zäunen, bei denen Sie möglicherweise durch Risse im Objekt oder transparente Objekte sehen können, sollten Sie den Occluder-Status des Objekts im Dropdownmenü "Statisch" deaktivieren, damit objekte hinter ihm nicht fälschlicherweise verblendet werden. 

## <a name="lightmaps"></a>**Lightmaps**

* Idealerweise nur **ein Lightmap pro Szene** (ein 2.000 oder ein 4.000 für alles), falls nicht; weniger Lightmaps mit höheren Auflösungen sind besser als viele Lightmaps mit niedrigeren Auflösungen.
* Mehrere Lightmaps können sich auch auf die Anzahl der Zeichnen-Aufrufe auswirken, da Objekte, die entweder Über- oder Keine Lightmaps haben, sich in verschiedenen Batches und andere Lightmaps ebenfalls in verschiedenen Batches finden.
* Im Allgemeinen sollte eine Lightmap-Auflösung von **ca. 25 Texeln** pro Einheit ausreichen (legen Sie die Auflösung in den Einstellungen für Beleuchtung/Szene fest).  Wenn Sie zusätzlichen Platz in Ihrer Lightmap haben, können Sie diesen Wert erhöhen.
* Ändern Sie die **Einstellung Lightmap-Skalierung** pro Objekt, sodass die Auflösung für Objekte gespeichert wird, die sie benötigen. 

* **Lightmap-Skalierungsdiagramm** (Faustregel) 
    * **Foreground** (Traversable Level Geo): 1 
    * **Props** (insbesondere Props kleiner als ein Mensch): **2-3** (um Lightmapartefakte und Nahtungen an Ihren Objekten zu vermeiden) 
    * **Mittelgrund** (Geometrie, die sich direkt außerhalb des durchlaufbaren Bereichs und/oder großer Objekte wie Gebäude befindet): **0,5**
    * **Hintergrund** (Vista-Objekte/entfernte Objekte): **0,02** 
    * **Transparente Oberflächen** (z. B. Glass): **0** (mit deaktivierter "Cast/Receive Shadows" ( Cast/Receive Shadows) 

Als Baseline sind hier einige Einstellungen, die für die Screen Door Effect-Umgebung verwendet wurden:

![Beleuchtungsfenster in Unity](images/world-building-lightmaps.png)

Hinweis: Wenn Sie diese Einstellungen verwenden, können Sie den Lightmapper auf "GPU Lightmapper" und die Lightmap-Größe auf "2048" festlegen, um das Baking in der Vorschau deutlich zu beschleunigen, und dann auf CPU und 4k für den endgültigen Bake-Abschluss sichern.

## <a name="texture-compressionfile-size"></a>**Texturkomprimierung/Dateigröße**

* Für unseren Android-Build versuchen wir, die Größe unserer Unity-Paketszene auf etwa 10 bis 20 MB zu halten.  Hierzu geben wir generische Materialien für viele Objekte weiter, verwenden Scheitelpunktfarbe, um die Objekte zu tönen, und setzen manuelle Überschreibungen für Android so ein, dass Texturen die **ASTC 6x6-Blockkomprimierung** verwenden, die kleiner als die Standardkomprimierung ist.

* Der Grund dafür, dass wir die Android-Buildeinstellungen nicht für die Verwendung von ASTC festlegen, ist, dass Lightmaps mit dieser Komprimierung nicht gut aussehen (viele Blockierungsartefakte), und wir müssen die Lightmap so festlegen, dass nach jedem Baking etc verwendet wird, sodass es einfacher ist, stattdessen die Außerkraftsetzung für alle Szenentexturen einmal einrichten zu können, als die Komprimierungseinstellungen der Lightmap nach jedem Bake zu aktualisieren.

![Texturfenster in Unity](images/world-building-texutres.png)

* Außerdem kann das Festlegen von Texturen für die Verwendung des trilinearen Filtermodus mit einer anisotropen Ebene von 2 dazu beitragen, dass sie beim Abblenden von Winkeln stark bleiben.

Weitere Tipps und Tricks zur Leistung finden Sie in der Dokumentation Improving world performance (Verbessern [der Leistung in der Welt).](improving-performance.md)
