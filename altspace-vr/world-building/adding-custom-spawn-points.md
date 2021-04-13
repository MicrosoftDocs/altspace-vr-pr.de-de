---
title: Hinzufügen von benutzerdefinierten punktpunkten
description: Erfahren Sie, wie Sie Ihre benutzerdefinierten Erstellungs Punkte in altspacevr erstellen, hinzufügen und beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Spawnpoint, Problembehandlung
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212223"
---
# <a name="adding-custom-spawn-points"></a>Hinzufügen von benutzerdefinierten punktpunkten

Personen, die ihre Welt betreten **, werden am** Ursprung, an der Position (0, 0, 0) angezeigt, wenn Sie in Ihre Welt gelangen. Sie können jedoch einen oder mehrere Ausgangspunkte hinzufügen, wenn Sie sagen möchten, dass die Benutzer am Eingang Ihres Schlosses beginnen. Wenn Sie mehrere Ausgangspunkte angeben, wird eine nach dem Zufallsprinzip ausgewählt, und der Ursprung wird nicht eingeschlossen. Sie können die-erlerpunkte auf jede Welt oder jedes Ereignis verwalten, in dem der World Editor aktiviert ist. Sie steuern, wo Menschen (Position) und in welcher Richtung Sie stehen (Drehung). Erfügebpunkte sind nur im Bearbeitungsmodus sichtbar. 

1. Wechseln Sie in der Nähe der Stelle, an der Sie die Leute erzeugen möchten. Öffnen Sie den **World Editor > Grundlagen** , und stellen Sie sicher, dass die **Sperr Drehung** aktiviert Wählen Sie einen **Punkt** für die Erstellung aus. Verschieben Sie es an die genaue Position, die Sie wünschen:

![Grundlagen des World Editor-Fensters geöffnet](images/spawn-points-img-01.png)

2. Wählen Sie auf dem Symbol "Einstellungen" für den pullpunkt aus, und stellen Sie sicher, dass **Drehung > X** und **Drehung > Z** beide **0** sind. Wenn Sie kleine Zahlen wie **8.537777745 e-07** sind, ist das auch in Ordnung. Dabei handelt es sich um eine Voreinstellung, wie Gleit Komma Zahlen behandelt werden:

![Aktualisieren von erstellungspunkten in den World Editor-Einstellungen](images/spawn-points-img-02.png)

3. Geben Sie Ihre Welt über das **Menü > Einstellungen erneut ein > Allgemein > > erneut** eingeben.
4. Sie sollten am neuen Punkt für das erzeugen!
5. Wenn Sie möchten, dass Personen einer anderen Richtung begegnen, wählen Sie die Einstellungen für den ausstellungspunkt aus, und legen Sie **Drehung > Y** fest. Versuchen Sie, Y auf 180 und sowohl x als auch z auf 0 festzulegen (Warnung: "x" und "z" werden möglicherweise krank gemacht). Wählen Sie dann **bestätigen** aus, und geben Sie die Welt wieder ein. Das sollte Ihnen die entgegengesetzte Richtung begegnen. 

## <a name="troubleshooting"></a>Problembehandlung

**Personen, die noch am Ursprung sind?**
    * Stellen Sie sicher, dass sich die-erwurgpunkte leicht über dem Grund-oder Oberflächen Wenn sich der Ausgangspunkt auf andere Objekte überschneidet, werden die Benutzer am Standard Speicherort, dem Ursprung, verschwinden. Dies kann vorkommen, wenn der Erstellungspunkt innerhalb eines Objekts und die Höhe der Person variiert. 
    * Versuchen Sie, ihre Welt über das **Menü > Einstellungen zurückzusetzen > > den Bereich zurücksetzen** .

**Haben Sie mehrere Ausgangspunkte, werden aber immer noch am gleichen Speicherort ausgeführt?**
Sie sind möglicherweise nicht glücklich, Sie sind nach allen zufällig. Versuchen Sie mindestens fünfmal, ein paar wieder einzugeben, und gehen Sie davon aus, dass ein Fehler vorliegt. 

**Menschen sind unbequem, oder ihre Kopfzeile ist gekippt** Möglicherweise haben Sie vergessen, die **Sperr Drehung** zu überprüfen oder den X-und Z-Wert für die Drehung festzulegen Diese sollten normalerweise auf 0 festgelegt werden, es sei denn, Sie entwickeln eine exotische Welt. 

**Menschen fallen, wenn Sie verschwinden?**
Legen Sie die Position des Punkt Punkts nicht zu hoch oberhalb eines Objekts fest. Wenn Sie zu weit gehen, werden Sie am Ursprung neu festgeschrieben.