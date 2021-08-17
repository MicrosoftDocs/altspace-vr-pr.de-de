---
title: Verwenden des Interactables-Spawners
description: Erfahren Sie, wie Sie den Spawner für interaktionsfähige Elemente erstellen, verwenden und anpassen, um Elemente in Ihren AltspaceVR-Bereichen zu platzieren.
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
# <a name="using-the-interactables-spawner"></a>Verwenden des Interactables-Spawners

Interactables Spawner ermöglicht es Ihnen, interaktive Elemente in Ihrem Ereignis-, Welt- oder Heimraum zu platzieren. Dieses Feature ist derzeit Teil unseres [Early Access-Programms](../world-building/early-access.md) und ist nur verfügbar, wenn Sie sich über Ihr Hauptmenü angemeldet haben.

> [!NOTE]
> Beachten Sie, dass zu viele interaktionsfähige Ereignisse die Leistung Ihrer Umgebung oder Ihres Ereignisses beeinträchtigen können, während wir mit der Pilotphase dieses Features fortfahren. 

## <a name="creating-an-interactable"></a>Erstellen eines interaktivierbaren

So wandeln Sie Ihr Objekt in ein interaktives Objekt um:

1. Platzieren Sie das Objekt in Ihrem Raum.
2. Suchen Sie dann den Eintrag in der Objektliste, und wählen Sie das **Zahnradsymbol** daneben aus, um dessen Einstellungen zu öffnen:

![Welt-Editor mit hervorgehobener Objektliste geöffnet](images/interactables-spawner-img-01.png)

Auf der Einstellungsseite finden Sie ein neues Kontrollkästchen **"Objekts spawner",** das verwendet wird, um es zu einem interaktionsfähigen Objekt zu machen.

1. Aktivieren Sie das Kontrollkästchen, und wählen Sie **bestätigen** aus.
2. Im Bearbeitungsmodus können Sie sich um die Spawn-Position des Objekts im Raum bewegen.
3. **Beenden Sie den Bearbeitungsmodus,** um die Elementinteraktion zu aktivieren.

![Fenster "Artefakt aktualisieren" in der AltspaceVR-App geöffnet](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>Weitere Anpassungen

Nachdem Sie **"Objekt-Spawner"** aktiviert haben, wenn Sie zu den Eigenschaften für dieses Objekt zurückkehren, gibt es eine zusätzliche Einstellung, die Sie auf das Verhalten des ausgelösten Objekts anwenden können.

> [!NOTE]
> Interaktive Objektskala: Dadurch wird die Skalierung des Objekts festgelegt, wenn es übernommen wird, im Vergleich zu "Scale", der Skalierung der Darstellung des Objekts auf der Welt, bevor es zum ersten Mal ausgewählt wird.

Kit-Entwickler bemerken möglicherweise, dass Änderungen am Kit während der Ausführung von ALTSPACEVR erst wirksam werden, wenn Sie ALTSPACEVR neu starten.

Vor Kurzem haben wir eine Schaltfläche unter der Registerkarte **Moderate Einstellungen** namens **Reload Worlds Kits** hinzugefügt. Wenn Sie auf diese Schaltfläche klicken, werden (nur Sie) den Speicherplatz erneut öffnen und alle Kits erneut laden. Dadurch werden nur neue Versionen der Kits heruntergeladen, die aktualisiert wurden, während Sie sich in AltspaceVR befanden.

![Moderater Einstellungsbereich in der AltspaceVR-App geöffnet](images/interactables-spawner-img-03.png)