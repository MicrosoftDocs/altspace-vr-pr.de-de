---
title: Verbessern der Leistung in der Welt
description: Erfahren Sie, wie Sie die Leistung Ihrer AltspaceVR-Welten mithilfe von Diagnosetools messen, beheben und verbessern.
ms.date: 03/11/2021
ms.topic: article
keywords: Leistung, Problembehandlung
ms.openlocfilehash: 79d2bc43858c99652439aafa159c23f48eb3aa299c2b183936e40b1794fe444e
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126921"
---
# <a name="improving-world-performance"></a>Verbessern der Leistung in der Welt

Wir möchten, dass Menschen eine gute Erfahrung haben, sodass die Leistung oder die Leistung Ihrer Welt auf VR-Headsets sehr wichtig ist. Unser World Building-System ist für eine hervorragende Leistung für die gängigsten Anwendungsfälle konzipiert. Wenn Sie die Präsenz maximieren möchten, ist dieser Leitfaden für Sie da. ALTSPACE unterstützt jede Hardwareplattform. Wir empfehlen World Builders, die Grenzwerte zu überschreiten. Für öffentliche Welten empfehlen wir Ihnen jedoch, oculus Quest und jede PC-basierte Plattform wie Windows Mixed Reality, Oculus Rift/Rift S oder OC Vive als Ziel zu verwenden. Wenn Ihre Welt gut auf einer Quest ausgeführt wird, ist dies wahrscheinlich für Altspace ideal, um es einfach zu halten.

## <a name="tools-and-measurement"></a>Tools und Messung

Die Administratordiagnose ist ein Offlinetool, das auf unserer Website verfügbar altvr.com. Wenn Sie zu [Worlds > My Worlds](https://account.altvr.com/users/sign_in)navigieren, Ihre Welt suchen und "Diagnose" auswählen, sehen Sie etwas wie das:

![Fenster "Administratordiagnose"](images/performance.png)

Dies sind mehr Richtlinien als Anforderungen. Die Leistung hängt davon ab, wie viele Objekte Sie haben und wie sie angeordnet sind. Wenn Sie beispielsweise 500 Objekte auf 2 Kilometer verteilen, ist die Leistung wahrscheinlich in Ordnung. Wenn Sie jedoch die gleichen 500 Objekte in einen eng gepackten Bereich legen, werden Wahrscheinlich probleme auftreten. Das liegt daran, dass die Leistung davon abhängt, was sich im Sichtfeld einer Person abspielt. Die beste Möglichkeit zum Testen besteht im Springen in Altspace und dem Teleport um Ihre Welt. Wenn Sie problemebehebungen oder Unannehmlichkeiten bemerken, sind dies Problempunkte, die Sie untersuchen möchten.

Indem Sie sich an diese Empfehlungen halten, richten Sie sich für den Erfolg ein. Sehen wir uns diese Beispieldiagnose an, die aus einer tatsächlichen featured World entnommen wurde: 

* **Objekte:** Gesamtanzahl der Objekte auf der Welt. Alles ist ein Objekt– Artifacts, Fotos, Spawn Points und so weiter. Es wird empfohlen, unter einer bestimmten Anzahl zu bleiben, aber dies ist flexibel. Wenn Sie weiterlesen, geben wir unser Problem mit einem gelben Ausrufezeichen an, wie hier gezeigt. In diesem Fall gibt es jedoch zwei separate Bereiche in dieser Welt, sodass die Dichte nicht hoch ist.
* **Kits:** Gesamtzahl der verwendeten eindeutigen World-Building Kits. Dies wirkt sich auf die anfängliche Downloadzeit beim Laden der Welt aus. Kits enthalten Artifacts, das Menü mit Objekten, die Sie in der Welt erstellen können. 

> [!NOTE] 
> Wenn ein einzelnes Artefakt aus einem Kit verwendet wird, müssen die Objekte dieses Kits heruntergeladen werden. Daher ist es sehr teuer, nur einige wenige Artifacts aus einem einzelnen Kit zu verwenden. 

* **Kits– Mobil:** Gesamtgröße aller Kit-Ressourcen, die eine Person auf einer Quest herunterladen muss, bevor sie in die Welt eintritt. Versuchen Sie nicht, die Menschen 5 Minuten warten zu lassen, um alles herunterzuladen, was sie für Ihre Welt benötigen.
* **Fotos:** Gesamtanzahl der verwendeten Fotos, die tendenziell eine höhere Auswirkung auf die Leistung haben als Artifacts. Verwenden Sie sparingly.
Vorlage– Mobil: Wenn Sie den Unity-Uploader verwenden, halten Sie die Downloadgröße niedrig.
* **Skybox--Mobile:** Wenn Sie benutzerdefinierte Skyboxes verwenden, sollten Sie die Dateigröße klein halten, damit die Benutzer keinen "schwarzen Bildschirm" erhalten (der Videospeicher ist nicht mehr verfügbar).
* **Fehlende/ungültige Kits/Artifacts:** Verweise auf problematische Kits oder Artifacts ... Haben Sie eine Idee für eine Metrik? Informieren Sie uns!
Auch hier sind dies keine Anforderungen, daher werden grüne, gelbe und rote Statussymbole angezeigt. Auch eine Welt mit einer Reihe roter Indikatoren wird möglicherweise weiterhin vorgestellt. Wir testen in Altspace, daher sollten Sie dies auch tun. [Wenn Sie Hilfe benötigen, kontaktieren Sie uns.](getting-help.md) 

## <a name="load-time"></a>Ladezeit

Wenn eine Person anfängt, zu Ihrer Welt zu reisen (versucht, zu gelangen), wird sie zuerst die Vorlage laden. Sie laden die Vorlagenressourcen (Dateien) für ihre Plattform herunter und sehen sich "Laden der Umgebung" an. Anschließend laden sie die Skybox- und Kit-Ressourcen herunter. Schließlich laden sie alle Objekte, während "Loading Objects" (Objekte laden) wird. Das Herunterladen aller Ressourcen kann je nach Internetbandbreite einige Minuten dauern. Das Laden von Objekten ist relativ schnell. Während die Ressourcen von schnellen Servern auf der ganzen Welt heruntergeladen werden, verwendet Altspace Cachetechniken, um zu vermeiden, dass dieselben Dateien wiederholt erneut heruntergeladen werden. Technisch gesehen wirkt sich die anfängliche Ladezeit nicht auf die Leistung einer Person aus, nachdem sie die Welt betritt, aber sie ist Teil der gesamter Erfahrung, also versuchen Sie nicht, zu lange zu warten, wenn sie in Ihre Welt reisen. Wir empfehlen Ihnen, sorgfältig zu überlegen, welche Kits verwendet werden sollen, und einfallsreich zu sein, indem Sie mehr mit weniger machen.

## <a name="troubleshooting-and-tips"></a>Problembehandlung und Tipps

**Personen sehen einen "schwarzen Bildschirm".** In der Regel liegt dies daran, dass dem Gerät nicht genügend Videospeicher zur Verfügung steht. Versuchen Sie, die Anzahl der Objekte im Problembereich der Welt zu reduzieren und die Größe von Objekten wie Skybox oder Vorlage oder die Anzahl der Fotos. Diese Typen haben in der Regel die größten Auswirkungen auf die Videospeicherauslastung.

**Personen stürzt ab**
    * Manchmal kann dies durch ein fehlerhaftes Kit oder Artefakt verursacht werden.
    * Dies kann auch durch Shader oder Animationen verursacht werden.
    * Achten Sie auf Dinge in benutzerdefinierten Vorlagen und Kits.
    * Sichern Sie Ihre Welt häufig, insbesondere während der frühen Entwicklung. Verwenden Sie diese Sicherungen, um das zu verbessern, was Sie kürzlich hinzugefügt haben, was zum Absturz von Personen führt.

**"Headroom" verlassen**
    * Denken Sie daran, dass sie möglicherweise 20 bis 30 Personen gleichzeitig auf der Welt haben. Was wäre, wenn all diese Personen um ein Feuer gestürzt sind. Möchten Sie trotzdem 200 Kieselsteine nach dem Brand setzen? Wahrscheinlich keine gute Idee. Lassen Sie Platz für Avatare und Interaktionsfähige (z. B. 300000000000).
    * Weniger ist mehr.

**Vorausplanen** Denken Sie darüber nach, was Sie erstellen möchten, und stellen Sie die Dinge in den Raum. Es ist einfach, in Altspace umher zu kommen.

**Frühzeitiges und häufiges Verwenden des Diagnosetools** Markieren Sie es als Lesezeichen, und aktualisieren Sie es nach und nach. Schließlich werden ähnliche Tools in VR vorhanden sein, die besser zugänglich sein werden.

**Freunde mit Oculus Quest-Benutzern** Laden Sie sie ein, in Ihre Welt zu kommen, um Sie beim Testen zu unterstützen. Testen Sie gründlich und häufig! Testen Sie die Welten der anderen! Nichts ist das Testen der realen Sache.

**Hinzufügen von Freunden als "Administratoren" für Ihre Welt** Bearbeiten Sie Ihre Welt, und fügen Sie Ihre Freunde der Administratorliste hinzu. Dadurch wird das Diagnosetool für Ihre Welt angezeigt. Seien Sie jedoch vorsichtig, da sie auch andere Aspekte Ihrer Welt bearbeiten können. 

**Die Leistungsoptimierung ist schwierig, daher ist unsere Community bestrebt, Ihnen zu helfen.** Treten Sie der [offiziellen AltspaceVR-Verunsprache](https://discordapp.com/invite/altspacevr) bei * Besuchen Sie den #world-Building-Kanal, um allgemeine Unterstützung bei Welten zu erhalten.
    * Besuchen Sie die MRE SDK-Kanäle, um spezifische Hilfe zu technischen und Unity Uploader-bezogenen Hilfe (Vorlagen und benutzerdefinierte Kits) zu erhalten.