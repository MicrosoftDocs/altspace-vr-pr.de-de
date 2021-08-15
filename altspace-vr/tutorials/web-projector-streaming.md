---
title: Verwenden des Webprojektors zum Streamen eines Browsers
description: Erfahren Sie, wie Sie den Webprojektor verwenden, um Inhalte aus einem bestimmten Browser in AltspaceVR-Funktionen zu streamen.
ms.date: 03/11/2021
ms.topic: article
keywords: Webprojektor, Stream, Browser
ms.openlocfilehash: 8f25de68ba633e10b9192b85c883de4ba48fd7987ec5d301ebac8443982a1a55
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127305"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>Verwenden des Webprojektors zum Streamen eines Browsers

Der AltspaceVR-Webprojektor ist eine stabile Medienfreigabelösung, mit der Sie eine bestimmte Browserregisterkarte direkt von Ihrem Desktop-PC in AltspaceVR streamen können. Es kann verwendet werden, um Folien, Videos, Fotos und fast alles andere, was Sie über einen Browser öffnen können, frei zu geben.* Der Webprojektor erfordert das Herunterladen einer Browsererweiterung und ist derzeit ausschließlich über den World Editor verfügbar. Im Folgenden finden Sie eine vollständige Übersicht über das Feature und seine Verwendung:

## <a name="requirements"></a>Anforderungen

1. Sie müssen einen PC oder Mac verwenden, um Ihren Browser zu streamen.
2. Die erforderliche Browsererweiterung wird derzeit vom Edge-Browser unterstützt. (Wir arbeiten daran, diese Liste zu erweitern.)
3. Sie können zwar von einem Mac-Computer streamen, der Webprojektor ist jedoch noch nicht im AltspaceVR Mac-Client verfügbar.
4. Wenn Alles ordnungsgemäß eingerichtet ist (bei der Browsererweiterung/AltspaceVR mit demselben Konto angemeldet, mit Webprojektor in AltspaceVR verbunden/übertragen) und immer noch ein grüner Bildschirm angezeigt wird, benötigt WebProjector den geöffneten TCP-Port 443 und den UDP-Portbereich 20000-20400.

> [!NOTE]
> Dieses Feature dient in erster Linie zum Streamen einer Browserregisterkarte Ihrer Wahl. Wenn Sie stattdessen versuchen, Ihre Desktopanwendung zu streamen, streamt der Webprojektor alle Computeraudiodaten (einschließlich AltspaceVR), was zu Echo/Feedback führen kann. Sie müssen AltspaceVR stummschalten, um zu verhindern, dass dies geschieht. Alternativ können Sie altspaceVR auch mit einem separaten Gerät ausführen, während Sie von Ihrem PC streamen.

## <a name="getting-started"></a>Erste Schritte

1. Zunächst müssen Sie die Browsererweiterung herunterladen und installieren. Diese finden Sie [HIER.](https://account.altvr.com/web_projector)
2. Laden Sie [als Nächstes die Erweiterung in Ihren Edge-Browser.](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading)
    * Sobald der Download abgeschlossen ist, wechseln Sie zum Abschnitt **Erweiterungen** Ihres Browsers. (Gefunden unter **Einstellungen**)
    * Entzippen Sie .zip Datei.
    * Umschalten im **Entwicklermodus und** Auswählen **von "Entpackt laden"**
    * Wählen Sie den Ordner aus, den Sie gerade entpackt haben. Dies ist die Webprojektorerweiterung.
    * Nachdem Die Erweiterung hinzugefügt wurde, können Sie unter **Details** ihre Einstellungen einrichten.

## <a name="setting-up-a-shareable-browser"></a>Einrichten eines gemeinsam nutzbaren Browsers

Nachdem Ihre Erweiterung heruntergeladen und installiert wurde, können Sie sie verwenden!

1. Öffnen Sie eine Registerkarte in Ihrem Edge-Browser, und navigieren Sie zu den Medien, die Sie freigeben möchten.
2. Richten Sie Ihr Fenster so ein, dass Sie für die Freigabe bereit sind. (Hinweis: Ihr gesamtes Browserfenster wird weltweit projiziert.)
3. Suchen Sie die neu installierte Erweiterung (die als AltspaceVR-Symbol in der Nähe Ihrer URL-Leiste in Ihrem Browser angezeigt wird). Wählen Sie AltspaceVR aus. Sie werden aufgefordert, sich bei Ihrem Konto anmelden. (*Hinweis: Es ist wichtig, dass Sie sich bei demselben Konto anmelden, das Sie zum Einrichten Ihres Webprojektors verwenden.)
4. Nachdem Sie sich angemeldet haben, sollte ihnen auf dem Erweiterungsbildschirm die Option **Streaming starten angezeigt** werden. Wählen Sie ihn aus.

## <a name="projecting-your-browser-in-world"></a>Weltweites Projektieren Ihres Browsers

1. Sobald Ihr Browser für die Projektion eingerichtet ist und Sie mit dem Streamen über die Erweiterung begonnen haben, öffnen Sie AltspaceVR.
2. Richten Sie den Webprojektor in Ihrer Umgebung Ihrer Wahl ein, indem Sie ihren World Editor > Basics > WebProjektor öffnen.
3. Nach dem Einordnen können Sie die Größe des Webprojektors mithilfe Der Welt-Editor-Steuerelemente ändern. (Er enthält auch Anweisungen auf dem Bildschirm.)
4. Klicken Sie auf **Verbinden,** um mit dem Streamen Ihres Edgebrowsers zu beginnen.
5. Denken Sie daran, auf **Broadcast** zu klicken, um mit der Freigabe für alle Gäste im Raum zu beginnen.
6. Vergessen Sie nicht, das **Streaming zu beenden.** Für Ihre Sitzung kommt es schließlich zu einem Time out, aber bis dahin wird ihr Browser weiterhin live geprojektt. Es ist am besten, ihre Sitzung zu beenden, sobald Sie fertig sind.

![Browser projiziert in AltspaceVR World](images/web-project-img-01.png)

**Videostreaming-Tipp:** Wenn Videos nicht mehr gestreamt werden, beenden Sie das Streaming, passen Sie die Videoqualität auf 480p oder 360p an, und starten Sie dann den Stream und die Übertragung neu. Höhere Auflösungen können CPU- und Uploadbandbreite beanspruchen.

> [!NOTE]
> Zu diesem Zeitpunkt sind die zusätzlichen Steuerschaltflächen am oberen Ende des Webprojektors noch nicht live. Sie bleiben grau und können nicht beklickt werden. Dies ist kein Fehler, sondern standardmäßig (derzeit).

> [!IMPORTANT]
> HAFTUNGSAUSSCHLUSS: Hinweis: Die Verwendung des Webprojektors unterliegt wie alle [](../community/terms-of-service.md) anderen Features in AltspaceVR unseren Nutzungsbedingungen und unseren Community [Standards.](../community/community-standards.md) Daher darf der Webprojektor nicht zum Streamen von Inhalten verwendet werden, die gegen eine der beiden Vereinbarung verstoßen. Dies führt zu Moderationsaktionen, die von AltspaceVR durchgeführt werden. Der Zugriff auf die WebProjektor-Betaversion ist nicht garantiert und kann nur für eine temporäre Testversion gewährt werden. Die Länge der Betaversion und die Länge Ihrer Teilnahme liegen im Ermessen des AltspaceVR-Teams. Die Verwendung der Betaversion des Webprojektors ist nicht erforderlich, und die Teilnahme an der Betaversion ist rein freiwillig. Den Teilnehmern wird empfohlen, Feedback zum Webprojektor zu geben, mit dem die Funktionalität und Nutzbarkeit des Features während der Entwicklung verbessert wird. Die Betaversion des Webprojektors hat möglicherweise eingeschränkte Funktionen und kann unerwarteten Fehlern unterliegen. Vielen Dank für Ihre Teilnahme im Voraus.
