---
title: Andere Benutzer können mich nicht hören
description: Erfahren Sie, wie Sie Probleme im Zusammenhang mit anderen Benutzern identifizieren und beheben können, die in altspacevr nicht zu hören sind.
ms.date: 03/11/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: b6248e46b62e1a29324e831e686aee7b1de4505a
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213363"
---
# <a name="other-users-cant-hear-me"></a>Andere Benutzer können mich nicht hören

Legen Sie zunächst fest, ob altspacevr die Audiodaten von Ihrem Mikrofon erkennt. Sie können dies ermitteln, indem Sie sehen, ob das Mikrofon Symbol links unten in der Ansicht blinklos ist, wenn Sie sprechen. Wenn das Symbol beim Gespräch blinkt ist, funktioniert Ihr Mikrofon. Wenn das Symbol rot ist, werden Sie stumm geschaltet. Wählen Sie das Symbol aus, um sich selbst zu stumm schalten

Wenn das Mikrofon Symbol nach dem Aufheben der Entsperrung nicht blinkende angezeigt wird, müssen Sie möglicherweise die Mikrofon Einstellungen in altspacevr anpassen. wechseln Sie zu Menü/Einstellungen/Audioeingabe und Audioeingabe. Verwenden Sie dann die Pfeil Schaltflächen, um das MIC auszuwählen, das Sie verwenden möchten.
 
## <a name="oculus-quest"></a>Oculus Quest 

Stellen Sie sicher, dass Sie beim Installieren von altspacevr Berechtigungen für die Verwendung Ihres MIC-audiozugriffs erteilt haben. Eine weitere Möglichkeit besteht darin, Folgendes anzuzeigen: Menü/Einstellungen/Audio-/Audio-Eingabeauswahl und sicherstellen, dass Sie auf Android-Audioeingabe festgelegt ist (das ist das Quest/Quest2's-standardmic).
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality, oculus Rift, HTC Vive oder 2D-Modus

Stellen Sie sicher, dass Sie über die richtigen Mikrofon Einstellungen in der Option "altspacevr: Menü/Einstellungen/Audio/Audioeingabe" verfügen. Verwenden Sie dann die Pfeil Schaltflächen, um das MIC auszuwählen, das Sie verwenden möchten.

Vergewissern Sie sich vor dem Starten von altspacevr, dass das richtige Mikrofon als Standard Aufzeichnungsgerät in Windows festgelegt ist. Sowohl Oculus Rift als auch HTC Vive verfügen über ein integriertes Mikrofon, wenn in altspacevr ein weiteres Mikrofon angeschlossen ist, das möglicherweise versucht, dieses Gerät zu verwenden.
 
So ändern Sie das Standard Aufzeichnungsgerät in Windows:
* Klicken Sie mit der rechten Maustaste auf das Redner Symbol in Windows, und wählen Sie **Wiedergabe Geräte**
* Zur Registerkarte " **Aufzeichnung** " navigieren
* Suchen Sie das Mikrofon, das Sie verwenden möchten. Das HTC Vive-Mikrofon erhält die Bezeichnung **Mikrofon-USB-Audiogerät** , und das Oculus-Rift **-** Mikrofon wird als Mikrofon mit Mikrofon Bezeichnung bezeichnet.
* Klicken Sie mit der rechten Maustaste auf das Mikrofon, und wählen Sie **als Standardgerät festlegen** .
* Nachdem Sie altspacevr neu gestartet haben, wird Ihr Mikrofon nun übernommen.
 
Wenn Sie nach dem Ausführen dieser Schritte weiterhin Probleme haben, treten einige andere Probleme auf, die sich möglicherweise auf Sie auswirken:
* Wenn Sie mehr als 30 Sekunden nicht mehr Alt-Tab, werden Sie von altspacevr automatisiert, Sie können dies deaktivieren, indem Sie die Leertaste zum Ein-/Ausschalten von stumm schalten verwenden.
* Das altspacevr-Audiosystem weist einen volumeschwell Wert auf, den Sie möglicherweise unten haben. Legen Sie MIC-Ebenen auf Max fest, legen Sie die MIC näher auf den Mund und sprechen Sie auf normalem Volume.
* Beenden Sie VR, versuchen Sie, Ihr USB-Kabel von Ihrem Headset an einen alternativen USB 3,0-Port zu binden. In unserem Prozess verursachen einige USB 3,0-Ports Probleme.

Altspacevr erkennt möglicherweise keine Sound Einstellungsänderungen, die während des Spiels vorgenommen wurden. Daher müssen Sie möglicherweise altspacevr der obigen Mikrofon Änderungen neu starten, damit Sie wirksam werden.  Wenn Sie das Spiel erneut eingeben, sehen Sie sich das Mikrofon Symbol an, und überprüfen Sie, ob es Blinks ist. Wenn das Symbol Blinks ist, funktioniert Ihr Mikrofon.