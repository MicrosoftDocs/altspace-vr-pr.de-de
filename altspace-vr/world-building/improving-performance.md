---
title: Verbessern der Welt Leistung
description: Erfahren Sie, wie Sie die Leistung Ihrer altspacevr-Welten mithilfe von Diagnosetools Messen, beheben und verbessern.
ms.date: 03/11/2021
ms.topic: article
keywords: Leistung, Problembehandlung
ms.openlocfilehash: 558ce2e089aecc206445c6b7bf99423f2d5c45cc
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212118"
---
# <a name="improving-world-performance"></a>Verbessern der Welt Leistung

Wir möchten, dass die Benutzer eine gute Leistung haben, oder wie gut Ihre Welt auf VR-Headsets läuft. Unser Welt eigenes Gebäudesystem ist für die meisten gängigen Anwendungsfälle konzipiert. Wenn Sie die Anwesenheit maximieren möchten, finden Sie diese Anleitung für Sie. In altspace wird die Unterstützung jeder Hardwareplattform angestrebt. Wir empfehlen Welt-Generatoren, die Grenzwerte zu übersetzen. für öffentliche Umgebungen empfiehlt es sich, die Oculus Quest und eine beliebige PC-basierte Plattform wie Windows Mixed Reality, oculus Rift/Rift S oder HTC Vive als Ziel zu setzen. Wenn Ihre Welt bei einer Quest gut funktioniert, ist es wahrscheinlich großartig für "altspace".

## <a name="tools-and-measurement"></a>Tools und Messungen

Die Administrator Diagnose ist ein Offline Tool, das auf unserer Website altvr.com verfügbar ist. Wenn Sie zu den [Welten > meine Welten](https://account.altvr.com/users/sign_in)navigieren, ihre Welt suchen und "Diagnose" auswählen, sehen Sie Folgendes:

![Fenster "Administrator Diagnose"](images/performance.png)

Dabei handelt es sich um mehr Richtlinien als Anforderungen. Die Leistung hängt davon ab, wie viele Objekte Sie haben und wie Sie angeordnet werden. Wenn Sie z. b. 500 Objekte haben, die sich über zwei Kilometer verteilen, ist die Leistung wahrscheinlich gut. Wenn Sie jedoch die gleichen 500-Objekte in einem stark gepackten Bereich platzieren, werden Sie wahrscheinlich Probleme erkennen. Das liegt daran, dass die Leistung von dem Bereich einer Person abhängig ist. Die beste Methode zum Testen ist das Springen in altspace und Teleport auf der ganzen Welt. Wenn Sie feststellen, dass ein Problem auftritt, können Sie die Problempunkte untersuchen.

Wenn Sie sich an diese Empfehlungen halten, haben Sie sich für einen Erfolg festgelegt. Im folgenden wird das Beispiel für die Diagnose aus einer realen hervor zeigte Welt behandelt: 

* **Objekte** -Gesamtzahl der Objekte weltweit. Alles ist ein Objekt,-Artefakte, Fotos, Punkt Punkte usw. Wir empfehlen, dass Sie eine bestimmte Anzahl behalten, aber dies ist flexibel. Wenn Sie fortfahren, geben wir das Problem mit einem gelben Ausrufezeichen an, wie hier gezeigt. In diesem Fall gibt es jedoch zwei separate Bereiche in dieser Welt, sodass die Dichte nicht hoch ist.
* **Kits** -Gesamtzahl der einmaligen, verwendeten Kits für die Welt Bausteine. Dies wirkt sich auf die anfängliche Downloadzeit beim Laden der Welt aus. Kits enthalten Artefakte, das Menü von Objekten, die Sie in der Welt erzeugen können. 

> [!NOTE] 
> Wenn ein einzelnes artefaktelement von einem Kit verwendet wird, müssen die Assets dieses Kits heruntergeladen werden. Es ist also awvoll aufwendig, nur einige Artefakte aus einem einzelnen Kit zu verwenden. 

* **Kits--Mobile** : Gesamtgröße aller Kit-Ressourcen, die eine Person auf einer Quest herunterladen muss, bevor Sie in die Welt wechselt. Versuchen Sie nicht, alle fünf Minuten zu warten, damit alles heruntergeladen wird, was Sie für Ihre Welt benötigen.
* **Fotos** -Gesamtzahl der verwendeten Fotos, die tendenziell höhere Auswirkungen auf die Leistung als Artefakte haben. Verwenden Sie sparsam.
Vorlage--Mobile: Wenn Sie das Unity-Uploader verwenden, sollten Sie die Downloadgröße gering halten.
* **Skybox--Mobile** : Wenn Sie benutzerdefinierte Skyboxes verwenden, sollten Sie die Dateigröße gering halten, sodass die Benutzer nicht "schwarzer Bildschirm" erhalten (nicht genügend Videospeicher).
* **Fehlende/ungültige Kits/Artefakte** -Verweise auf problematische Kits oder Artefakte... Haben Sie eine Idee für eine Metrik? Informieren Sie uns!
Auch hier sind dies keine Anforderungen, daher zeigen wir grüne, gelbe, rote Statussymbole an. Sogar eine Welt mit einer Reihe von roten Indikatoren ist möglicherweise weiterhin zu sehen. Wir testen in altspace, damit Sie es auch tun sollten. [Wenden Sie sich an uns, wenn Sie Hilfe benötigen](getting-help.md). 

## <a name="load-time"></a>Ladezeit

Wenn eine Person mit der Reise zu ihrer Welt beginnt (versucht, einzugeben), lädt Sie zuerst die Vorlage. Die Vorlagen Objekte (Dateien) werden für Ihre Plattform heruntergeladen, und Sie sehen, dass die Umgebung geladen wird. Anschließend werden die Skybox-und Kit-Assets heruntergeladen. Schließlich laden Sie alle Objekte, während Sie "Objekte laden" sehen. Das Herunterladen aller Assets kann je nach Internetbandbreite einige Minuten dauern – das Laden von Objekten ist recht schnell. Während die Assets von schnellen Servern auf der ganzen Welt heruntergeladen werden, verwendet altspace zwischen Speicherungs Techniken, um zu vermeiden, dass dieselben Dateien wiederholt heruntergeladen werden. Technisch gesehen wirkt sich die anfängliche Ladezeit nicht auf die Leistung einer Person aus, nachdem Sie in die Welt gelangt ist, Sie ist jedoch Teil der gesamten Umgebung. versuchen Sie also nicht, dass die Benutzer zu lange warten, wenn Sie zu ihrer Welt reisen. Wir empfehlen Ihnen, sorgfältig zu überlegen, welche Kits verwendet werden und wie Sie sich mit weniger Möglichkeiten beschäftigen.

## <a name="troubleshooting-and-tips"></a>Problembehandlung und Tipps

**Menschen sehen einen "schwarzen Bildschirm"** . Dies liegt in der Regel daran, dass das Gerät nicht mehr über Videospeicher verfügt. Versuchen Sie, die Anzahl der Objekte im Bereich "Problem" der Welt zu reduzieren, und reduzieren Sie die Größe der Dinge wie Ihre Skybox oder Vorlage oder die Anzahl der Fotos. Diese Typen haben tendenziell die größte Auswirkung auf die Videospeicher Auslastung.

**Menschen abstürzen**
    * Manchmal kann ein fehlerhaftes Kit oder artefaktelement dies verursachen.
    * Diese können auch von verrückten Shadern oder Animationen verursacht werden.
    * Achten Sie auf benutzerdefinierte Vorlagen und Kits.
    * Sichern Sie Ihre Welt häufig, insbesondere während der frühen Entwicklung. Verwenden Sie diese Sicherungen, um sich darüber zu vertiefen, was Sie vor kurzem hinzugefügt haben, was dazu führt, dass Menschen abstürzen.

**"Headroom" verlassen**
    * Denken Sie daran, dass Sie gleichzeitig 20-30 Personen auf der Welt haben können. Was geschieht, wenn alle diese Personen um ein Lager herum herum waren. Möchten Sie trotzdem 200 Pebbles durch den Brand platzieren? Wahrscheinlich keine gute Idee. Überlassen Sie Raum für Avatare und interactables (wie z. b. Basketbälle).
    * Weniger ist mehr.

**Planen Sie voraus** Stellen Sie sich vor, was Sie erstellen möchten. Es ist einfach, in altspace zu umgehen.

**Verwenden Sie das Diagnose Tool frühzeitig und häufig** Markieren Sie Sie, und aktualisieren Sie Sie in einer Weile. Schließlich sind ähnliche Tools in VR vorhanden, auf die zugegriffen werden kann.

**Treffen von Benutzern mit Oculus Quest-Benutzern** Laden Sie Sie in Ihre Welt ein, um Sie beim Testen zu unterstützen. Gründlich und häufig testen! Testen Sie alle anderen Welten! Es gibt keine Auswirkungen auf das Testen der tatsächlichen Dinge.

**Fügen Sie Freunde als "Administratoren" für Ihre Welt hinzu** . Bearbeiten Sie Ihre Welt, und fügen Sie Ihr Freunde zur Administrator Liste hinzu. Auf diese Weise können Sie das Diagnosetool für Ihre Welt sehen. Seien Sie jedoch vorsichtig, da Sie auch andere Aspekte der Welt bearbeiten können. 

**Die Leistungsoptimierung ist schwierig, damit unsere Community Hilfe** Treten Sie der [offiziellen altspacevr-Uneinigkeit](https://discordapp.com/invite/altspacevr) * besuchen Sie den #World bauchannel, um allgemeine Unterstützung bei den Welten zu erhalten.
    * In den MRE SDK-Kanälen finden Sie besondere Unterstützung bei technischen und Unity-Uploader-Hilfe (Vorlagen und benutzerdefinierte Kits).