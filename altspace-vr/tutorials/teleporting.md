---
title: Verwenden des Teleporter
description: Erfahren Sie, wie Sie mithilfe eines Teleporter in altspacevr von einem Ereignis oder einer Welt zu einem anderen Reisen können.
ms.date: 03/11/2021
ms.topic: article
keywords: Teleporter
ms.openlocfilehash: afc199e958824bb5f0a9ff6d74865cbcd3f16868
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213419"
---
# <a name="using-the-teleporter"></a>Verwenden des Teleporter

Das Reisen von einem Ereignis oder einer Welt zu einem anderen ist eine hervorragend für Sie und die Community, um alles zu untersuchen, was von altspacevr angeboten werden muss.

## <a name="the-short-version"></a>Die Kurzversion

![Teleportierungs Schritte aus dem Editor-Panel zum Festlegen eines Teleportations-Ziels](images/teleporter.png)

## <a name="the-slightly-longer-version"></a>Die etwas längere Version

Stellen Sie zunächst sicher, dass Sie sich in Ihrem Homespace befinden, in einem Ereignis oder einer Welt, das Sie erstellt haben oder in dem Sie die terraex-Rolle erhalten haben. Wenn Sie sich im 2D-Modus befinden und die Schaltfläche "World Editor" nicht in der unteren rechten Ecke der Benutzeroberfläche angezeigt wird, klicken Sie mit der rechten Maustaste auf die Maustaste, um diese ein-bzw. auszuschalten. Wenn die Schaltfläche "World Editor" immer noch nicht angezeigt wird, befinden Sie sich möglicherweise in einer anderen Person. Wenn dies der Fall ist, bitten Sie den Host, Ihnen die terraex-Rolle zu übergeben.

Außerdem wird Folgendes unterstützt: 
1. Erstellen Sie zuerst die Ereignisse oder die Welt.
2. Wechseln Sie zu der Stelle, an der Sie den Teleporter erzeugen möchten, damit Ihre Ereignisse/Welten im Bereich "Teleporter-Ziel" aufgefüllt werden und die Verbindung mit dem Teleporter schneller und einfacher gestalten.

Ein weiterer Trick, mit dem Sie im 2D-Modus mit Teleportern navigieren können, ist die Verwendung von STRG + LEERTASTE. Die Eingabeaufforderung wird angezeigt, und Sie können Folgendes eingeben: "zurück", damit Sie wieder zum letzten Bereich gelangen, in dem Sie sich befinden. 

Wechseln Sie nun zu dem Speicherort, an dem Sie einen Teleporter erzeugen möchten, und wählen Sie im Bereich "World Editor/Editor Panel/Basics/Teleporter" aus.

Dadurch wird der Bereich "Teleporter-Ziel" angezeigt. Es werden drei Kategorien angezeigt, aus denen Sie auswählen können:

* **Meine Leerzeichen** : Liste der von Ihnen erstellten Welten.
* **Zuletzt** verwendete Liste der zuletzt verwendeten Ereignisse. Verwenden Sie diese Option, wenn Sie zu einem Ereignis wechseln möchten. Dies ist die einzige Option, die Sie zu einem Ereignis führt, das andere 2 ermöglicht nur die Übertragung zwischen den Welten. Hinweis: siehe weiter unten, wenn Sie Front Row-Ereignisse mit importierten Welten verbinden, müssen Sie die teleportoren in der importierten Welt und nicht im eigentlichen Ereignis einrichten und einrichten.
* **Vorgestellt** : Liste der vorgestellten Welten Sie können den Teleporter auf Reisen festlegen.

Wählen Sie das Ereignis oder die Welt aus, das Sie verwenden möchten. Dadurch wird der Teleporter erzeugt und eine Text Bezeichnung für das Ereignis oder den Namen der Welt etwas zurückgesetzt. Sie können also das Zahnrad Symbol im Abschnitt "vorhandene Objekte" auswählen, um den Namen der Bezeichnung zu ändern.

Sie können entweder für den Teleporter mit dem Cursor auswählen (Sie werden gefragt, ob es in Ordnung ist, wenn es sich um einen Fehlschlag handelt) oder den Avatar direkt in den Teleporter verschieben, und Presto, dass Sie zu Ihrem Ziel gelangen. Sagen Sie, dass wir Hallo!

## <a name="advanced-features"></a>Erweiterte Funktionen

Wenn Sie eine Konferenz, einen Summit oder ein größeres Ereignis mithilfe von Front Row mit einer benutzerdefinierten Welt erstellen (z. b. eine Foundation World-, Unity-Uploader-Raum Vorlage, Re-Import Welt), müssen Sie den Teleporter in ihrer Foundation-Welt einrichten und nicht im eigentlichen Ereignis. Stellen Sie sicher, dass Sie den Teleporter so einrichten, dass er zum richtigen Ereignis (muss aus der Liste "zuletzt aufgeführt") in ihrer Foundation-Welt wechseln, und Re-Import Welt im Ereignis, um die teleportoren in allen Front-Row-Ereignis Räumen anzuzeigen.

## <a name="faqs"></a>Häufig gestellte Fragen

**Fehler: "Wir möchten uns leider nicht erlauben, aber wir können Sie nur dort"**

An das Ereignis ist möglicherweise eine Gruppe angefügt, sodass nur Benutzernamen in der Gruppe in den Teleporter gelangen können, um das Ereignis für die private Gruppe zu erhalten.

**Wie viele teleportoren kann ich in einem Bereich verwenden?**

Teleportierer verwenden transparente Texturen mit animierten Partikel Effekten. es ist also am besten, dass sich nicht zu viele alle in derselben Stelle/überlappenden überlappenden, da dies die Leistung beeinträchtigen könnte. Versuchen Sie nicht, mehr als 4 im gleichen Bereich oder mehr als 10 zu verwenden, wenn Sie alle in Ihrem Raum verteilt sind.