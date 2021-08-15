---
title: Verbessern der Weltleistung
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
# <a name="improving-world-performance"></a>Verbessern der Weltleistung

Wir möchten, dass Menschen eine gute Erfahrung haben, sodass leistung oder wie gut Ihre Welt auf VR-Headsets ausgeführt wird, sehr wichtig ist. Unser World Building-System ist für eine hervorragende Leistung für die meisten gängigen Anwendungsfälle konzipiert. Wenn Sie die Präsenz maximieren möchten, ist dieser Leitfaden für Sie geeignet. Altspace unterstützt alle Hardwareplattformen. World Builders wird zwar empfohlen, die Grenzwerte zu pushen, aber für öffentliche Welten empfehlen wir, oculus Quest und alle PC-basierten Plattformen wie Windows Mixed Reality, Oculus Rift/Rift S oder QUEST Vive als Ziel zu verwenden. Um dies einfach zu halten, ist es wahrscheinlich ideal für Altspace, wenn Ihre Welt gut auf einer Quest ausgeführt wird.

## <a name="tools-and-measurement"></a>Tools und Messungen

Die Administratordiagnose ist ein Offlinetool, das auf unserer Website altvr.com verfügbar ist. Wenn Sie zu [Worlds > My Worlds](https://account.altvr.com/users/sign_in)navigieren, Ihre Welt suchen und "Diagnose" auswählen, sehen Sie in etwa Wie folgt:

![Fenster "Administratordiagnose"](images/performance.png)

Dies sind mehr Richtlinien als Anforderungen. Die Leistung hängt davon ab, wie viele Objekte Sie haben und wie sie angeordnet sind. Wenn Sie beispielsweise über 500 Objekte verfügen, die auf zwei Kilometer verteilt sind, ist die Leistung wahrscheinlich in Ordnung. Wenn Sie jedoch die gleichen 500 Objekte in einen eng gepackten Bereich legen, treten wahrscheinlich Probleme auf. Dies liegt daran, dass die Leistung davon abhängt, was im Sichtfeld einer Person vorkommt. Die beste Möglichkeit zum Testen besteht darin, in Altspace zu springen und um Ihre Welt zu teleportieren. Wenn Sie eine Störung bemerken oder sich unzumutig fühlen, handelt es sich um Problempunkte, die Sie untersuchen möchten.

Indem Sie sich an diese Empfehlungen halten, richten Sie sich für den Erfolg ein. Sehen wir uns diese Beispieldiagnose an, die aus einer tatsächlichen Ausgewählten Welt entnommen wurde: 

* **Objekte:** Gesamtanzahl der Objekte in der Welt. Alles ist ein Objekt– Artifacts, Fotos, Spawn Points usw. Es wird empfohlen, unter einer bestimmten Zahl zu bleiben, aber dies ist flexibel. Wenn Sie darüber hinaus gehen, geben wir unsere Bedenken mit einem gelben Ausrufezeichen an, wie hier gezeigt. In diesem Fall gibt es jedoch zwei separate Bereiche in dieser Welt, sodass die Dichte nicht hoch ist.
* **Kits:** Gesamtanzahl der verwendeten eindeutigen World Building Kits. Dies wirkt sich auf die anfängliche Downloadzeit beim Laden der Welt aus. Kits enthalten Artifacts, das Menü der Objekte, die Sie in der Welt erstellen können. 

> [!NOTE] 
> Wenn ein einzelnes Artefakt aus einem Kit verwendet wird, müssen die Ressourcen dieses Kits heruntergeladen werden. Daher ist es sehr teuer, nur ein paar Artifacts aus einem einzelnen Kit zu verwenden. 

* **Kits– Mobil:** Gesamtgröße aller Kit-Ressourcen, die eine Person auf einer Quest herunterladen muss, bevor sie in die Welt eintritt. Versuchen Sie nicht, dass Benutzer fünf Minuten warten, um alles herunterzuladen, was sie für Ihre Welt benötigen.
* **Fotos:** Gesamtzahl der verwendeten Fotos, die tendenziell eine höhere Leistungsbeeinträchtigung als Artifacts haben. Verwenden Sie sparingly.
Vorlage – Mobil: Wenn Sie den Unity-Uploader verwenden, halten Sie die Downloadgröße niedrig.
* **Skybox- Mobile:** Wenn Sie benutzerdefinierte Skyboxes verwenden, halten Sie die Dateigröße klein, damit die Benutzer keinen "schwarzen Bildschirm" erhalten (nicht genügend Videospeicher).
* **Fehlende/ungültige Kits/Artifacts:** Verweise auf problematische Kits oder Artifacts ... Haben Sie eine Idee für eine Metrik? Informieren Sie uns!
Auch hier sind dies keine Anforderungen, sodass wir grüne, gelbe und rote Statussymbole anzeigen. Sogar eine Welt mit einer Reihe roter Indikatoren kann weiterhin angezeigt werden. Wir testen in Altspace, daher sollten Sie es auch tun. [Wenn Sie Hilfe benötigen, können Sie sich an uns äusseren.](getting-help.md) 

## <a name="load-time"></a>Ladezeit

Wenn eine Person beginnt, in Ihre Welt zu reisen (versucht, sie einzugeben), lädt sie zuerst die Vorlage. Sie laden die Vorlagenressourcen (Dateien) für ihre Plattform herunter und sehen sich "Ladeumgebung" an. Anschließend laden sie die Skybox- und Kit-Ressourcen herunter. Schließlich laden sie alle Objekte, während sie "Loading Objects" (Objekte laden) sehen. Das Herunterladen aller Ressourcen kann je nach Internetbandbreite bis zu einigen Minuten dauern. Das Laden von Objekten ist relativ schnell. Während die Ressourcen von schnellen Servern auf der ganzen Welt heruntergeladen werden, verwendet Altspace Cachingtechniken, um zu vermeiden, dass dieselben Dateien wiederholt erneut heruntergeladen werden. Technisch gesehen wirkt sich die anfängliche Ladezeit nicht auf die Leistung einer Person aus, nachdem sie in die Welt gelangt ist, aber sie ist Teil der Gesamterfahrung. Versuchen Sie also nicht, die Wartezeit für Personen zu lange zu gestalten, wenn sie in Ihre Welt reisen. Wir empfehlen Ihnen, sorgfältig darüber nachzudenken, welche Kits verwendet werden sollten, und sind einfallsreich, indem Sie mehr mit weniger tun.

## <a name="troubleshooting-and-tips"></a>Problembehandlung und Tipps

**Personen sehen einen "schwarzen Bildschirm"** In der Regel liegt dies daran, dass auf dem Gerät nicht genügend Videospeicher vorhanden ist. Versuchen Sie, die Anzahl der Objekte im Problembereich der Welt zu reduzieren und die Größe von Objekten wie Skybox oder Vorlage oder die Anzahl der Fotos zu reduzieren. Diese Typen haben in der Regel die höchsten Auswirkungen auf die Videospeicherauslastung.

**Abstürze von Personen**
    * Manchmal kann dies durch ein fehlerhaftes Kit oder Artefakt verursacht werden.
    * Dies kann auch durch Shader oder Animationen verursacht werden.
    * Achten Sie auf Dinge in benutzerdefinierten Vorlagen und Kits.
    * Sichern Sie Ihre Welt häufig, insbesondere während der frühen Entwicklung. Verwenden Sie diese Sicherungen, um das zu verbessern, was Sie kürzlich hinzugefügt haben, das zum Absturz von Personen führt.

**Belassen Sie "Headroom".**
    * Denken Sie daran, dass Sie 20 bis 30 Personen gleichzeitig auf der Welt haben können. Was wäre, wenn sich all diese Personen um ein Lagerbrand gezwurscht hätten. Möchten Sie trotzdem 200 Steine nach dem Brand setzen? Wahrscheinlich keine gute Idee. Lassen Sie Platz für Avatare und Interaktivables (z. B. Swerte).
    * Weniger ist mehr.

**Planen im Voraus** Überlegen Sie sich, was Sie erstellen möchten, und legen Sie den Platz frei. Es ist einfach, sich in Altspace zu bewegen.

**Frühzeitiges und häufiges Verwenden des Diagnosetools** Setzen Sie ein Lesezeichen, und aktualisieren Sie es ab und zu. Irgendwann werden ähnliche Tools in VR vorhanden sein, die leichter zugänglich sind.

**Treffen von Freunden mit Oculus Quest-Benutzern** Laden Sie sie ein, in Ihre Welt zu kommen, um Sie beim Testen zu unterstützen. Testen Sie gründlich und häufig! Testen Sie die Welten der anderen! Nichts übertrifft tests auf die reale Sache.

**Hinzufügen von Freunden als "Administratoren" für Ihre Welt** Bearbeiten Sie Ihre Welt, und fügen Sie Ihre Freunde der Administratorliste hinzu. Dadurch wird das Diagnosetool für Ihre Welt angezeigt. Seien Sie jedoch vorsichtig, da sie auch andere Aspekte Ihrer Welt bearbeiten können. 

**Die Leistungsoptimierung ist schwierig, sodass unsere Community gerne helfen möchte.** Treten Sie dem [offiziellen AltspaceVR Discord](https://discordapp.com/invite/altspacevr) bei * Besuchen Sie den kanal für #world, um allgemeine Unterstützung bei Welten zu erhalten.
    * Besuchen Sie die MRE SDK-Kanäle, um spezifische Hilfe zu technischen und Unity Uploader-bezogenen Hilfe (Vorlagen und benutzerdefinierte Kits) zu erhalten.