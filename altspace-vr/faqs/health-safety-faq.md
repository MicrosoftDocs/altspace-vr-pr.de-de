---
title: Häufig gestellte Fragen zu Integrität und Sicherheit
description: Problembehandlung und Support für Probleme im Zusammenhang mit Integrität und Sicherheit.
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr, AlspaceVR, Problembehandlung, Support, Integrität, Sicherheit, Reduzierung der Minderung der Drosselung in VR
ms.openlocfilehash: fb4a6c020857bc393ea7367b6b5c71b94bd4f948
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311874"
---
# <a name="frequently-asked-questions-on-health-and-safety"></a>Häufig gestellte Fragen zu Integrität und Sicherheit

## <a name="why-do-some-people-feel-ill-in-vr"></a>Warum fühlen sich einige Menschen in VR nicht wohl?

Es ist ein beliebtes Ding, dass alle VR-Vertigo- und -Spots verursachen. Das Problem basiert auf einer Diskrepanz zwischen dem, was Ihre Augen sehen, und dem, was Ihr inneres Gehör an Ihr Gehirn überträgt. Wenn Ihre Augen Bewegungsbewegungen erkennen und Ihr Gesicht mitteilt, dass Sie still stehen, kann das Gehirn einiger Personen reagieren, indem es Müh und Unzufriedenheit auslöst. Einige Personen, die anfälliger für Bewegungsbewegungen sind, sind möglicherweise anfälliger für dieses Übel, während andere möglicherweise kein Problem damit haben. 

Es gibt mehrere Dinge, die auf Hardwareebene ausgeführt werden, und einige in der AltspaceVR-Software, die die in vr-Umgebungen verursachende Bewegung erheblich reduziert oder vollständig beseitigt.

## <a name="hardware-based-nausea-reduction"></a>Hardwarebasierte Reduzierung der Minderung

Durch die moderne VR-Hardware wie Oculus Rift und DEN Vive wird die Bewegung reduziert, indem Videoframes mit einer Rate dargestellt werden, mit der die Latenz beseitigt wird, die zu Einerschleusung führen kann. Wenn die Software optimiert ist, wie altspaceVR ist, gibt es keine erkannte Verzögerung, wenn Sie den Kopf in VR drehen. Die Beschleunigungsmesser im HMD kommunizieren Bewegung und übertragen diese Telemetriedaten schneller, als das menschliche Auge Latenzen erkennen kann. Bei HMD-Modellen mit Positionskameras geht dies einen Schritt weiter, nicht nur die Drehbewegung wird dargestellt, sondern auch die Seitwärtsbewegung (Von Seite zu Seite).

## <a name="software-based-nausea-reduction"></a>Softwarebasierte Reduzierung der Minderung

Zusätzlich zu Hardwareverbesserungen und Frameraten hat AltspaceVR mehrere Features implementiert, die Menschen dabei helfen, Minderungen zu reduzieren und zu beseitigen:

* **Teleportierung:** Wenn Sie sich sofort von Punkt zu Punkt bewegen, wird die Bewegung nicht mit dem Gehirn kommuniziert, sodass Bewegungsunterdrückungen vermieden werden.
* **Ausrichtungsschalten:** AltspaceVR bietet auf der gesamten Hardware Mittel für die "ratierte" oder "abgestufte" Drehung der Ansicht in VR. Anders ausgedrückt: Beim Drehen wird die Ansicht etwa 20 Grad drehbar. Auch hier löst dies bei den meisten Personen keine Auslösung aus.
* **Andockbewegung:** Bei bestimmter Hardware wird die Perspektive durch Wischen nach vorn auf dem Touchpad in einem Inkrement nach vorn verschoben, das keine Bewegungsausweitung auslöst. 
 
## <a name="how-to-eliminate-motion-sickness"></a>Entfernen von Bewegungsbewegungen

**Stand Still**

Versuchen Sie nicht, mit den Controllern zu viel zu bewegen, drehen Sie einfach den Kopf oder nach oben/unten, um sich in VR umzusehen.

**Verwenden Sie keine Maus/KB oder keinen Controller.**

AltspaceVR bietet Benutzern die Möglichkeit, Standardmäßige Gaming-Peripheriegeräte wie Maus-/Tastatur- und Gamecontroller zu verwenden, um sich in VR wie in einem Video zu bewegen. Dies schließt mehrdirektionale Bewegung, Bewegungen und eine Turboschaltfläche ein. Es wird empfohlen, diese nur zu verwenden, nachdem Sie sich daran gewöhnt haben, sich an VR zu gewöhnen. Nehmen Sie es auch dann langsam.

**Sie können jederzeit die Ausfälle aus der A-**

Entfernen Sie Ihre HMD sofort, wenn Sie auf Ungnübel zunehmen. Gewinnen Sie Ihre Heiterung zurück, und kehren Sie zur VR-Umgebung zurück, wenn Sie bereit sind. Versuchen Sie, sich die Bewegung zu merken, die dazu geführt hat, dass das Lösch- und Dasinsering nicht wiederholt wurde.

**Wissen, wann es Zeit ist, VR zu beenden**

Am wichtigsten ist, dass Sie wissen, wann es Zeit ist, eine Pause einlegen. Sie kennen Ihren Text, und wenn er Ihnen einen starken Hinweis gibt, dass etwas falsch ist, lauschen Sie. Machen Sie eine Pause, und verschaffen Sie sich etwas Luft. Gehen Sie umher, und richten Sie Ihre Ausgewogenheit neu aus. Sobald Sie sich wieder gut fühlen, kehren Sie zurück, und wir sind sicher, dass die Partei noch weitermachen wird!

## <a name="support"></a>Support

Fragen oder Feedback für das AltspaceVR-Team? 

> [!div class="nextstepaction"]
> [Klicken Sie hier, um eine Supportanfrage zu senden.](https://help.altvr.com/hc/requests/new)