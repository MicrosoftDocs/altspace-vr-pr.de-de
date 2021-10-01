---
title: Häufig gestellte Fragen zu AltspaceVR-Audio
description: Problembehandlung und Support für Audioprobleme.
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: VR, Audio, Problembehandlung, Support
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311869"
---
# <a name="frequently-asked-questions-about-audio"></a>Häufig gestellte Fragen zu Audio

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>Verfügt mein VR-Headset über ein integriertes Mikrofon?

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus Rift/Rift S, Oculus Quest/Quest 2, Windows Mixed Reality und QUEST Vive

Ja, diese VR-Headsets verfügen über integrierte Mikrofone.

### <a name="windows"></a>Windows

Für Headsets, die mit Windows verwendet werden, sollten Sie das Mikrofon unter Ihren **Aufzeichnungsgeräten** finden können, während Sie das Headset angeschlossen haben.

### <a name="further-troubleshooting"></a>Weitere Problembehandlung

* [AltspaceVR-Support: Andere Benutzer können mich nicht hören](#what-do-i-do-if-other-users-cant-hear-me)
* [AltspaceVR-Unterstützung : Verwalten von Berechtigungen für Oculus Quest](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>Gibt es eine Taste, die zum Sprechen gedrückt wird?

Es gibt keine Push-to-Talk-Schaltfläche.  Wenn Sie auf die untere linke Seite ihrer Ansicht sehen, gibt es ein Mikrofonsymbol, das zum Umschalten der Stimme verwendet werden kann. Alternativ können Sie die Tastenkombination Leertaste verwenden, um das Mikrofon zu stummschalten/zu stummschalten.

Wenn das Symbol blinkt, wenn Sie sprechen, funktioniert Ihr Mikrofon!
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>Was kann ich tun, wenn meine Audiodaten geschnitten sind?

Einige Benutzer haben bemerkt, dass die Audiodaten, wenn ein anderer Avatar spricht, als "choppy" oder mit regulären Ausfällen angezeigt werden. Sie können in anderen Fällen von anderen Benutzern darüber informiert werden, dass Ihre eigenen Audiodaten durch Drosselung oder Roboter stammen.

Der erste Versuch besteht darin, immer wieder den Speicherplatz einzufahren, in dem Sie sich befinden, oder sogar altspaceVR neu zu starten, wenn dies fehlschlägt. Audioprobleme sind nicht üblich, aber wenn sie auftreten, ist dies oft eine einfache Lösung. 

Wenn dies fehlschlägt, können Sie Folgendes untersuchen:

#### <a name="cpu-performance-for-desktop-users"></a>CPU-Leistung für Desktopbenutzer

Lesen Sie unsere [empfohlenen Systemspezifikationen](../getting-started/system-requirements.md) für Hardware, die wir für die Ausführung von AltspaceVR vorschlagen. Wir haben festgestellt, dass i3 oder niedrigere CPUs nicht nur probleme mit den Frameraten des Videos verursachen, sondern auch zu Audioproblemen wie Aussteigern und schlechter Qualität beitragen können.

#### <a name="internet-bandwidth-and-network-connection"></a>Internetbandbreite und Netzwerkverbindung

Bei Benutzern mit langsamen Internetverbindungen (weniger als 5 MBit/s) oder WLAN können Audioprobleme auftreten, z. B. Dropdowns. Es wird empfohlen, eine Hardlineverbindung eines Ethernet-Kabels mit Ihrem Computer und eine Verbindung schneller als 5 MBit/s herzustellen. Möglicherweise möchten Sie alle Programme beenden, die möglicherweise eine Internetverbindung im Hintergrund verwenden.

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>Was kann ich tun, wenn andere Benutzer mich nicht hören können?

Ermitteln Sie zunächst, ob AltspaceVR die Audiodaten von Ihrem Mikrofon erkennt. Sie können dies ermitteln, indem Sie sich ansehen, ob das Mikrofonsymbol in der unteren linken Seite Ihrer Ansicht blinkt, wenn Sie sprechen. Wenn das Symbol blinkt, wenn Sie sprechen, funktioniert Ihr Mikrofon. Wenn das Symbol rot ist, werden Sie stummgeschaltet. Wählen Sie das Symbol aus, um sich selbst zu stummschalten oder zu ändern.

Wenn Ihr Mikrofonsymbol nach dem Aufheben der Unveränderlichung nicht blinkt, müssen Sie möglicherweise Ihre Mikrofoneinstellungen in AltspaceVR anpassen, indem Sie zu Menü /Einstellungen/Audio/Audioeingabeauswahl wechseln. Wählen Sie dann mithilfe der Pfeilschaltflächen das Mikrofon aus, das Sie verwenden möchten.
 
### <a name="oculus-questquest-2"></a>Oculus Quest/Quest 2

Stellen Sie sicher, dass Sie Beim Installieren von ALTSPACEVR Berechtigungen für die Verwendung Ihres Mikrofonaudios erteilen. Eine weitere Überprüfung, die Sie durchführen können, ist die Auswahl von Menü/Einstellungen/Audio/Audioeingabe und das Festlegen der Einstellung auf Android-Audioeingabe, das Standard-Mikrofon von Quest/Quest2.
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality, Oculus Rift/Rift S, ICE Vive oder 2D-Modus

Stellen Sie sicher, dass Sie in ALTSPACEVR über die richtigen Mikrofoneinstellungen verfügen: Menü/Einstellungen/Audio/Audioeingabeauswahl. Wählen Sie dann mithilfe der Pfeilschaltflächen das Mikrofon aus, das Sie verwenden möchten.

Stellen Sie vor dem Starten von AltspaceVR sicher, dass das richtige Mikrofon als Standardaufzeichnungsgerät in Windows festgelegt ist. Oculus Rift/Rift S und DIE Vive VON OCulus verfügen jeweils über ein integriertes Mikrofon. Wenn Sie ein anderes Mikrofon angeschlossen haben, versucht AltspaceVR möglicherweise, dieses Gerät zu verwenden.
 
So ändern Sie Ihr Standardaufzeichnungsgerät in Windows:

* Klicken Sie in Windows mit der rechten Maustaste auf ihr Lautsprechersymbol, und wählen Sie **Soundeinstellungen öffnen** aus.
* Navigieren Sie zur Dropdown-Dropdowndatei **Eingabe/Eingabegerät auswählen.**
* Wählen Sie im Dropdownmenü das Mikrofon aus, das Sie verwenden möchten: 
    * Das MIKROFON VON Vive wird mit **Mikrofon – USB-Audiogerät** bezeichnet.
    * Das Oculus Rift-Mikrofon wird als **Headset-Mikrofon (Oculus Virtual Audio Device)** bezeichnet.
* Nach dem Neustart von AltspaceVR wird Ihr Mikrofon nun übernommen.
 
Wenn nach dem Ausführen dieser Schritte weiterhin Probleme auftreten, kann dies folgende Auswirkungen haben:

* Wenn Sie mehr als 30 Sekunden Alt-Tab, werden Sie von AltspaceVR automatisch stummgeschaltet. Sie können dies im **Menü -> Einstellungen -> Audio -> Mute deaktivieren, wenn altspaceVR im Leerlauf ist.**
* Das AltspaceVR-Audiosystem weist einen Lautstärkeschwellenwert auf, den Sie möglicherweise unterschreiten. Legen Sie die Mikrofonwerte auf max fest, legen Sie das Mikrofon näher an Ihrem Mund fest, und sprechen Sie bei normaler Lautstärke.
* Beenden Sie VR, und schließen Sie Ihr USB-Kabel von Ihrem Headset an einen alternativen USB 3.0-Anschluss an. Unserer Erfahrung nach verursachen einige USB 3.0-Anschlüsse Probleme.

AltspaceVR erkennt möglicherweise keine Änderungen an der Soundeinstellung, die während des Spiels vorgenommen wurden. Daher müssen Sie altspaceVR möglicherweise neu starten, damit die oben genannten Mikrofonänderungen wirksam werden.  Wenn Sie das Spiel erneut eingeben, sehen Sie sich das Mikrofonsymbol an, und sehen Sie, ob es blinkt, wenn Sie sprechen. Wenn das Symbol blinkt, funktioniert Ihr Mikrofon.

## <a name="support"></a>Support

Fragen oder Feedback für das AltspaceVR-Team? 

> [!div class="nextstepaction"]
> [Klicken Sie hier, um eine Supportanfrage zu senden.](https://help.altvr.com/hc/requests/new)