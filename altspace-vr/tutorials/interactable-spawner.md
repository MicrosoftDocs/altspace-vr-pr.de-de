---
title: Verwenden des-interactables-spawners
description: Erfahren Sie, wie Sie den interactables-Spawner erstellen, verwenden und anpassen, um Elemente in Ihrem altspacevr-Raum zu platzieren.
ms.date: 02/10/2021
ms.topic: article
keywords: Spawner, Interaktionen, Anpassungen
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213550"
---
# <a name="using-the-interactables-spawner"></a>Verwenden des-interactables-spawners

Der interactables Spawner ermöglicht Ihnen das Platzieren von Objekten, die sich in Ihrem Ereignis, in der Welt oder in der privatfläche befinden. Diese Funktion ist zurzeit Teil des [frühen Zugriffs Programms](../world-building/early-access.md) und ist nur verfügbar, wenn Sie sich über Ihr Hauptmenü angemeldet haben.

> [!NOTE]
> Obwohl wir dieses Feature weiter testen, beachten Sie, dass das Erzeugen von zu vielen interactables möglicherweise die Leistung Ihrer Umgebung oder Ihres Ereignisses beeinträchtigt. 

## <a name="creating-an-interactable"></a>Erstellen einer Interaktionen

So schalten Sie das Objekt in ein Objekt mit Interaktionen um:

1. Platzieren Sie das-Objekt in Ihrem Bereich.
2. Suchen Sie anschließend den Eintrag in der Objektliste, und wählen Sie das **Zahnrad Symbol** neben dem Eintrag aus, um die Einstellungen zu öffnen:

![World Editor geöffnet mit hervorgehobener Objektliste](images/interactables-spawner-img-01.png)

Auf der Seite "Einstellungen" finden Sie das neue Kontrollkästchen **"Objekt Spawner"**, das verwendet wird, um es zu einem Objekt zu machen, das interacbar ist.

1. Aktivieren Sie das Kontrollkästchen, und klicken Sie auf **bestätigen**.
2. Im Bearbeitungsmodus können Sie den Speicherort des Objekts im Bereich verschieben.
3. **Beenden des Bearbeitungsmodus** zum Aktivieren der Element Interaktion.

![Artefaktfenster in der altspacevr-APP öffnen](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>Weitere Anpassungen

Nachdem Sie **"Object Spawner"** aktiviert haben, wenn Sie zu den Eigenschaften für dieses Objekt zurückkehren, gibt es eine zusätzliche Einstellung, die Sie auf die Art und Weise des erzeugten Objekts anwenden können.

> [!NOTE]
> Objekt Skala mit interactable: Hiermit wird die Skalierung des Objekts festgelegt, wenn es abgerufen wird, im Vergleich zu "Skalieren", bei der es sich um die Skalierung des Objekts in der Welt handelt, bevor es zum ersten mal abgerufen wird.

Die Kit-Ersteller bemerken möglicherweise, dass Änderungen an Ihrem Kit, während altspacevr ausgeführt wird, erst nach einem Neustart von altspacevr wirksam werden.

Vor kurzem haben wir auf der Registerkarte " **moderate Einstellungen** " eine Schaltfläche mit dem Namen " **Upload Worlds Kits**" Wenn Sie auf diese Schaltfläche klicken, wird der Bereich erneut eingegeben, und alle Kits werden erneut geladen, sodass nur neue Versionen der Kits heruntergeladen werden, die während der Ausführung von altspacevr aktualisiert wurden.

![Mittlerer Einstellungsbereich in der altspacevr-app geöffnet](images/interactables-spawner-img-03.png)