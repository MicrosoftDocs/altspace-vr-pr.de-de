---
title: Verwenden des Webprojektors zum Streamen eines Browsers
description: Erfahren Sie, wie Sie den Webprojektor verwenden, um Inhalte aus einem bestimmten Browser in AltspaceVR-Funktionen zu streamen.
ms.date: 03/11/2021
ms.topic: article
keywords: Webprojektor, Stream, Browser
ms.openlocfilehash: 2c5cb6ef917b7e799b8da3f1a769d77258866992
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112922997"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>Verwenden des Webprojektors zum Streamen eines Browsers

Der AltspaceVR-Webprojektor ist eine robuste Lösung für die Medienfreigabe, mit der Sie eine festgelegte Browserregisterkarte direkt von Ihrem Desktop-PC in AltspaceVR streamen können. Sie kann zum Freigeben von Folien, Videos, Fotos und fast allen anderen Funktionen verwendet werden, die Sie in einem Browser öffnen können.* Der Webprojektor erfordert das Herunterladen einer Browsererweiterung und ist derzeit ausschließlich über den World Editor verfügbar. Im Folgenden finden Sie eine vollständige Übersicht über das Feature und seine Verwendung:

## <a name="requirements"></a>Requirements (Anforderungen)

1. Sie müssen einen PC oder Mac verwenden, um Ihren Browser zu streamen.
2. Die erforderliche Browsererweiterung wird derzeit vom Edge-Browser unterstützt. (Wir arbeiten daran, diese Liste zu erweitern.)
3. Sie können zwar von einem Mac-Computer streamen, der Webprojektor ist jedoch noch nicht auf dem AltspaceVR Mac-Client verfügbar.
4. Wenn Sie alles richtig eingerichtet haben (bei der Browsererweiterung/AltspaceVR mit demselben Konto angemeldet, mit Web-Projektor in AltspaceVR verbunden/übertragen) und weiterhin einen grünen Bildschirm sehen, muss WebProjector tcp-Port 443 geöffnet und den UDP-Portbereich 20000-20400.

> [!NOTE]
> Dieses Feature dient in erster Linie zum Streamen einer Browserregisterkarte Ihrer Wahl. Wenn Sie versuchen, stattdessen Ihre Desktopanwendung zu streamen, streamt der Web-Projektor alle Computeraudiodaten (einschließlich AltspaceVR), was zu Echo/Feedback führen kann. Sie müssen AltspaceVR stummschalten, um dies zu verhindern. Alternativ können Sie auch ein separates Gerät verwenden, um AltspaceVR auszuführen, während Sie von Ihrem PC streamen.

## <a name="getting-started"></a>Erste Schritte

1. Zunächst müssen Sie die Browsererweiterung herunterladen und installieren, die Sie [HIER](https://account.altvr.com/web_projector)finden.
2. Laden Sie als Nächstes [die Erweiterung in Ihren Edge-Browser.](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading)
    * Sobald der Download abgeschlossen ist, wechseln Sie zum Abschnitt **Erweiterungen** Ihres Browsers. (Gefunden unter **Einstellungen**)
    * Entzippen Sie die .zip-Datei.
    * Umschalten im **Entwicklermodus** und Auswählen von **"Entladen laden"**
    * Wählen Sie den Ordner aus, den Sie gerade entpackt haben. Dies ist die Web-Projektor-Erweiterung.
    * Nachdem Ihre Erweiterung hinzugefügt wurde, können Sie zu **Details** wechseln, um Ihre Einstellungen einzurichten.

## <a name="setting-up-a-shareable-browser"></a>Einrichten eines freigegebenen Browsers

Sobald Ihre Erweiterung heruntergeladen und installiert wurde, können Sie sie verwenden!

1. Öffnen Sie eine Registerkarte in Ihrem Edge-Browser, und navigieren Sie zu den Medien, die Sie freigeben möchten.
2. Richten Sie Ihr Fenster ein, damit Sie zur Freigabe bereit sind. (Hinweis: Ihr gesamtes Browserfenster wird weltweit projiziert.)
3. Suchen Sie die neu installierte Erweiterung (die als AltspaceVR-Symbol in der Nähe Ihrer URL-Leiste in Ihrem Browser angezeigt wird). Wählen Sie AltspaceVR aus. Sie werden aufgefordert, sich bei Ihrem Konto anzumelden. (*Hinweis: Es ist wichtig, dass Sie sich bei demselben Konto anmelden, das Sie zum Einrichten Ihres Webprojektors verwenden.)
4. Sobald Sie angemeldet sind, sollte auf dem Erweiterungsbildschirm die Option **Streaming starten** angezeigt werden. Wählen Sie ihn aus.

## <a name="projecting-your-browser-in-world"></a>Projektieren Ihres Browsers in der Welt

1. Sobald Ihr Browser für die Projektion eingerichtet ist und Sie mit dem Streaming über die Erweiterung begonnen haben, öffnen Sie AltspaceVR.
2. Richten Sie den Webprojektor in Ihrer bevorzugten Umgebung ein, indem Sie Ihren World Editor > Basics > Web Overhead öffnen.
3. Nach der Platzierung können Sie ihre World Editor-Steuerelemente verwenden, um die Größe des Webprojektors zu ändern. (Es enthält auch Anweisungen auf dem Bildschirm.)
4. Wählen Sie die Schaltfläche **Verbinden** aus, um mit dem Streamen Ihres Edge-Browsers zu beginnen.
5. Denken Sie daran, auf **Broadcast** zu klicken, um mit der Freigabe für alle Gäste im Raum zu beginnen.
6. Vergessen Sie nicht, das Streaming zu **beenden.** Für Ihre Sitzung tritt schließlich ein Time out auf, bis zu diesem Zeitpunkt wird ihr Browser jedoch weiterhin live projiziert. Es ist am besten, ihre Sitzung zu beenden, sobald Sie fertig sind.

![In altspaceVR world projizierter Browser](images/web-project-img-01.png)

**Videostreamingtipp:** Wenn video stuttert, beenden Sie das Streaming, passen Sie die Videoqualität auf 480p oder 360p an, und starten Sie den Stream neu, und übertragen Sie ihn. Höhere Auflösungen können die CPU- und Uploadbandbreite beeinträchtigen.

> [!NOTE]
> Zu diesem Zeitpunkt sind die zusätzlichen Steuerelementschaltflächen oben im Webprojektor noch nicht live. Sie bleiben grau und können nicht angeklicken werden. Dies ist kein Fehler, er ist (vorerst) entwurfshalber.

> [!IMPORTANT]
> HAFTUNGSAUSSCHLUSS: Hinweis: Die Nutzung des Webprojektors unterliegt wie alle anderen Features in AltspaceVR unseren [Nutzungsbedingungen](../community/terms-of-service.md) und unseren [Communitystandards.](../community/community-standards.md) Daher kann der Web-Projektor nicht zum Streamen von Inhalten verwendet werden, die gegen eine der beiden Vereinbarungen verstoßen. Dies führt zu Moderationsaktionen, die von ALTSPACEVR ausgeführt werden. Der Zugriff auf die WebProjektor-Betaversion ist nicht garantiert und kann nur für eine temporäre Testversion gewährt werden. Die Dauer der Betaversion und die Dauer Ihrer Teilnahme liegen im Ermessen des AltspaceVR-Teams. Die Verwendung der Betaversion des Web-Projektors ist nicht erforderlich, und die Teilnahme an der Betaversion ist rein freiwillig. Den Teilnehmern wird empfohlen, Feedback zum Webprojektor zu geben, mit dem die Funktionalität und Nutzbarkeit des Features im Zuge der Entwicklung gestaltet werden kann. Die Betaversion des Web-Projektors verfügt möglicherweise über eingeschränkte Funktionalität und kann unerwarteten Fehlern ausgesetzt sein. Vielen Dank im Voraus für Ihre Teilnahme.
