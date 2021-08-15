---
title: Hinzufügen von benutzerdefinierten Spawnpunkten
description: Erfahren Sie, wie Sie Ihre benutzerdefinierten Spawnpunkte in AltspaceVR erstellen, hinzufügen und Probleme beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Spawnpoint, Problembehandlung
ms.openlocfilehash: 53ff2e60d929aed9be5650b132da6d1dab8e6f1c5a78425dc5f17c10f2c4dfdb
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127260"
---
# <a name="adding-custom-spawn-points"></a>Hinzufügen von benutzerdefinierten Spawnpunkten

Personen, die in Ihre Welt eintreten, werden am Ursprung und an der Position (0,0,0) **angezeigt,** wenn sie in Ihre Welt eintreten. Sie können jedoch einen oder mehrere Spawn Points hinzufügen, wenn Sie z. B. personen am Eingang ihrer Stadt beginnen möchten. Wenn Sie mehrere Spawn Points angeben, wird nach dem Zufallsprinzip einer ausgewählt, wenn jemand eingeht und der Ursprung nicht eingeschlossen wird. Sie können Spawn Points to any World oder Event (Spawn Points to any World oder Event) verwalten, bei dem Ihr World Editor aktiviert ist. Sie steuern, wo Personen entstehen (Position) und welche Richtung sie haben (Drehung). Spawn Points sind nur im Bearbeitungsmodus sichtbar. 

1. Wechseln Sie in die Nähe der Stelle, an der Die Menschen erstellen sollen. Öffnen Sie **den Editor für die Welt > Grundlagen,** und stellen Sie sicher, dass die **Sperrrotation** aktiviert ist. Wählen Sie **Spawn Point (Spawn Point)** aus, um einen zu erstellen. Verschieben Sie sie an die gewünschte Position:

![Fenster "Grundlagen" des World-Editors geöffnet](images/spawn-points-img-01.png)

2. Wählen Sie das Einstellungssymbol für den Spawn Point aus, und stellen Sie sicher, dass **Rotation > X** und Rotation > **Z** beide **0** sind. Wenn es sich um kleine Zahlen wie **8,537777745E-07** handelt, ist dies ebenfalls in Ordnung. Dies ist ein Quirk der Behandlung von Gleitkommazahlen:

![Aktualisieren von Spawnpunkten in den Einstellungen des World-Editors](images/spawn-points-img-02.png)

3. Reenter Your World via **Menu > Einstellungen > General > Reenter Space > Re-Enter**
4. Sie sollten am neuen Spawn Point erstellen!
5. Wenn Sie möchten, dass Personen in eine andere Richtung wechseln, wählen Sie die Einstellungen für den Spawn Point (Spawn Point) aus, und legen Sie Rotation > Y only (Nur **Drehung > Y)** fest. Versuchen Sie, Y auf 180 und sowohl X als auch Z auf 0 festzulegen (Warnung: X und Z sind erweitert, kann dies dazu führen, dass Die Menschen untätig werden). Wählen Sie dann **Bestätigen** aus, und geben Sie die Welt erneut ein. Dadurch sollten Sie die entgegengesetzte Richtung sehen. 

## <a name="troubleshooting"></a>Problembehandlung

**Personen, die noch am Ursprung entstehen?**
    * Stellen Sie sicher, dass sich Die Spawn Points leicht über dem Boden oder der Oberfläche befinden. Wenn sich der Spawn-Punkt mit anderen Objekten überschneidet, werden die Personen am Standardspeicherort, dem Ursprung, angezeigt. Dies kann passieren, wenn der Spawn Point innerhalb eines Objekts und die Höhe der Person variieren. 
    * Versuchen Sie, Ihre Welt über **menü > Einstellungen > Moderieren > Zurücksetzen des Speicherplatzes zurückzusetzen.**

**Haben Sie mehrere Spawn Points, aber werden immer noch an derselben Stelle spawning?**
Möglicherweise sind Sie unaufdinglich– es ist schließlich zufällig. Versuchen Sie es mindestens fünfmal erneut, bevor Sie davon ausgehen, dass ein Fehler vorliegt. 

**Menschen sind ungute, oder ihr Kopf ist geneigt** Möglicherweise haben Sie vergessen, die **Sperrrotation** zu überprüfen oder den X- und Z-Wert für Rotation festzulegen. Diese sollten in der Regel auf 0 festgelegt werden, es sei denn, Sie erstellen eine "World World". 

**Fallen Menschen, wenn sie entstehen?**
Legen Sie die Spawn Point-Position nicht zu hoch über einem Objekt fest. Wenn sie zu weit fallen, werden sie am Ursprung angezeigt.