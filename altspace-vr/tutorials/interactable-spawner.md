---
title: Verwenden des Spawners "Interactables"
description: Erfahren Sie, wie Sie die interaktionsfähige Spawner-Datei erstellen, verwenden und anpassen, um Elemente in Ihren AltspaceVR-Räumen zu platzieren.
ms.date: 02/10/2021
ms.topic: article
keywords: Spawner, Interaktionen, Anpassungen
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127399"
---
# <a name="using-the-interactables-spawner"></a>Verwenden des Spawners "Interactables"

Mit interactables Spawner können Sie interagierbare Elemente in Ihrem Ereignis, ihrer Welt oder Ihrem Heimbereich platzieren. Dieses Feature ist derzeit Teil unseres Early [Access-Programms](../world-building/early-access.md) und steht nur zur Verfügung, wenn Sie sich über Ihr Hauptmenü angemeldet haben.

> [!NOTE]
> Während wir dieses Feature weiterhin als Pilot verwenden, beachten Sie, dass sich zu viele interaktionsfähige Funktionen auf die Leistung Ihrer Umgebung oder Ihres Ereignisses auswirken können. 

## <a name="creating-an-interactable"></a>Erstellen eines interagierbaren

So machen Sie Ihr Objekt in ein interaktionsfähiges Objekt:

1. Platzieren Sie das -Objekt in Ihrem Raum.
2. Suchen Sie dann den Eintrag in der  Objektliste, und wählen Sie das Zahnradsymbol daneben aus, um die Einstellungen zu öffnen:

![Geöffneter World-Editor mit hervorgehobener Objektliste](images/interactables-spawner-img-01.png)

Auf der Einstellungsseite finden Sie ein neues Kontrollkästchen **"Objekt-Spawner",** das verwendet wird, um es zu einem interagierbaren Objekt zu machen.

1. Aktivieren Sie das Kontrollkästchen, und wählen Sie **bestätigen aus.**
2. Im Bearbeitungsmodus können Sie die Spawn-Position des Objekts im Raum bewegen.
3. **Beenden Sie den Bearbeitungsmodus,** um die Elementinteraktion zu aktivieren.

![Öffnen des Artefaktfensters in der AltspaceVR-App](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>Weitere Anpassungen

Nach dem Aktivieren **von "Object spawner" (Objekt-Spawner),** wenn Sie zurück zu den Eigenschaften für dieses Objekt wechseln, gibt es eine zusätzliche Einstellung, die Sie auf das Verhalten des erstellten Objekts anwenden können.

> [!NOTE]
> Interaktionsfähige Objektskala: Hier wird die Skalierung des Objekts bei der Aufnahme im Vergleich zu "Scale" (Skalieren) im Vergleich zur Skalierung der Art und Weise, wie das Objekt in der Welt vor der erstmaligen Aufnahme angezeigt wird, bestimmt.

Kit-Erhersteller bemerken möglicherweise, dass Änderungen an Ihrem Kit, während AltspaceVR ausgeführt wird, erst wirksam werden, wenn Sie AltspaceVR neu starten.

Vor Kurzem haben wir auf der Registerkarte Moderate Einstellungen eine Schaltfläche **namens** **Reload Worlds Kits hinzugefügt.** Wenn Sie auf diese Schaltfläche klicken, werden (nur Sie) erneut in den Bereich geladen, und alle Kits werden erneut geladen. Dadurch werden nur neue Versionen der Kits heruntergeladen, die aktualisiert wurden, während Sie sich in AltspaceVR waren.

![Moderater Einstellungsbereich in der AltspaceVR-App geöffnet](images/interactables-spawner-img-03.png)