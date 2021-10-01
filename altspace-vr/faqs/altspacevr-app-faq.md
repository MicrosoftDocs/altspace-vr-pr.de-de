---
title: Häufig gestellte Fragen zur AltspaceVR-App
description: Problembehandlung und Support für die AltspaceVR-App.
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr, AltspaceVR, Problembehandlung, Support
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311866"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>Häufig gestellte Fragen zur AltspaceVR-App

## <a name="finding-the-altspacevr-app-version"></a>Suchen der AltspaceVR-App-Version

Im Zuge der Problembehandlung werden Sie möglicherweise gefragt, welche Version der AltspaceVR-App Sie gerade ausführen.

### <a name="in-altspacevr"></a>In AltspaceVR

Um die App-Version in AltspaceVR zu finden, navigieren Sie zum Einstellungsmenü, **und** wählen Sie **in** der linken Navigationsleiste About aus. Die "App-Version" wird hier gemeldet, wie im folgenden Screenshot gezeigt.

![Einstellungen menü öffnen mit geöffneter "About"-Leiste](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>In Windows System Einstellungen

Wenn Sie AltspaceVR über die Microsoft Store installiert haben, finden Sie zusätzlich die App-Version in den Windows Systemeinstellungen.  Dieses Szenario ist gut geeignet, wenn Sie die App-Version melden, wenn Sie sich nicht erfolgreich beim Client anmelden können.

Um die App-Version in Windows Systemeinstellungen zu finden, öffnen Sie **das Startmenü,** geben Sie Apps & **Features** ein, und wählen Sie das Ergebnis aus. Navigieren Sie in der Liste der Apps zu **AltspaceVR.** Klicken Sie mit der linken Maustaste auf AltspaceVR, und wählen **Sie im** angezeigten Menü Erweiterte Optionen aus.

![Menü "Apps und Features" mit hervorgehobener Option "Erweitert" geöffnet](images/app-version-img-02.png)

In den **erweiterten Optionen** unter dem **Header Spezifikationen** sollte die **App-Version** rechts neben der Bezeichnung **Version aufgeführt** werden.

![Erweiterte Optionen mit hervorgehobener App-Version geöffnet](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>App-Version in Clientprotokollen

AltspaceVR meldet die App-Version in der Clientprotokolldatei während des Anwendungsstarts als "Altspace-Version". Dies wäre eine gute Option, um die App-Version zu erhalten, wenn Sie sich nicht erfolgreich beim Client anmelden können, aber es wurde versucht, vor dem Fehler zu starten.

### <a name="windows"></a>Windows

Auf Windows sie die Clientprotokolldatei über den Windows Explorer unter:

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

Diese Datei wird jedes Mal überschrieben, wenn Sie AltspaceVR starten. "Player.log" stellt Ihre neueste Sitzung dar, und "Player-prev.log" stellt die vorherige Sitzung dar.

### <a name="via-powershell"></a>Über PowerShell

Fortgeschrittene Benutzer können die Clientprotokolle wie folgt über PowerShell nach dieser Zeichenfolge durchsuchen:

Eingabe:

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

Ausgabe:

[2.047] AltspaceVR Version: 3.2.23.e66c2

## <a name="how-do-i-upload-my-client-logs"></a>Gewusst wie meine Clientprotokolle hoch?

Die AltspaceVR-Clientanwendung speichert ein Protokoll mit Diagnosedaten und Ereignissen, die während der Verwendung von AltspaceVR auftreten. Im Zuge der Problembehandlung werden Sie möglicherweise aufgefordert, "Ihre Protokolle hochzuladen", damit unser Team sie überprüfen kann. Dies ist ein Feature von AltspaceVR, mit dem Sie ihrem Team Ihren lokalen Protokollinhalt senden können, um uns bei der Problembehandlung zu unterstützen.

### <a name="in-altspacevr"></a>In AltspaceVR

Navigieren Sie zum Hochladen von Clientprotokollen in AltspaceVR zum **Einstellungsmenü,** und wählen Sie **in** der linken Navigationsleiste Support aus. Hier sind mehrere Optionen zum Hochladen von Protokollen verfügbar, wie im folgenden Screenshot gezeigt.

![Einstellungen Menü mit geöffneten Supportbereichen und hervorgehobenen Protokollfeldern](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>Felder

**"Was ist schief gelaufen?"**
Beschreiben Sie, was passiert ist. Wenn Sie z. B. einen Fehler finden, beschreiben Sie, was sie erwartet haben, im Gegensatz zu dem, was tatsächlich passiert ist). Diese Informationen werden zusammen mit dem Protokoll gesendet, wenn Sie den Upload drücken.

**"Hochladen Protokolle"** Diese Schaltfläche lädt Protokolle aus der aktuellen Sitzung hoch. Verwenden Sie diese Option, wenn Sie in derselben Sitzung ein Problem finden (z. B. wenn Sie den AltspaceVR-Client nicht geschlossen haben) und ihn melden möchten.

**"Hochladen Letzte Protokolle"** Diese Schaltfläche lädt Protokolle aus der vorherigen Sitzung hoch.

**"Hochladen Letzten Absturzprotokoll"** Diese Schaltfläche lädt weitere Protokollinhalte nach dem letzten Absturz hoch, den Sie gesehen haben.

### <a name="in-client-logs"></a>In Clientprotokollen

Sie können die Protokolldateien auch von Ihrem Computer abrufen. Anweisungen zum Abrufen dieser Protokolle finden Sie [hier.](#app-version-in-client-logs)


Nachdem Sie diese Dateien gefunden haben, öffnen Sie ein [Supportticket,](https://help.altvr.com/hc/en-us/requests/new) und laden Sie Ihre Protokolle in Ihre Ticketanforderung hoch, bevor Sie auf Senden klicken.

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>Was kann ich tun, wenn ich AltspaceVR nicht starten kann?

Es gibt mehrere Gründe, warum AltspaceVR möglicherweise nicht für Sie gestartet wird. Probieren Sie die folgenden Schritte aus, um sicherzustellen, dass die Anwendung ordnungsgemäß mit der erforderlichen Drittanbietersoftware installiert ist.

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>Wenn Sie altspaceVR zum ersten Mal starten möchten:

1. Stellen Sie sicher, dass Ihr Gerät unterstützt wird und die [angegebenen Mindestanforderungen erfüllt.](../getting-started/system-requirements.md)
2. Stellen Sie sicher, dass Die neueste [Oculus Software](https://www.oculus.com/setup) installiert ist und Einstellungen-> Allgemein-> Unbekannte Geräte auf EIN festgelegt ist. Wenn Sie im 2D-Modus starten, muss Oculus nicht installiert sein.
3. Stellen Sie sicher, dass Sie über eine funktionierende Internetverbindung verfügen. Wenn Sie versuchen, Altspace aus einer Netzwerkfirewall zu starten, öffnen Sie die UDP-Ports 5055 und 5056 sowie die TCP-Ports 80 und 443. Wenn Sie sich innerhalb des Netzwerks einer Unternehmens- oder Bildungsfirewall befinden, müssen Sie sich möglicherweise an den Netzwerkadministrator oder die IT-Abteilung wenden.
4. Weitere Informationen:
    * [Installieren von AltspaceVR für Oculus Quest](../getting-started/oculus-installation.md)
    * [Installieren von AltspaceVR für Windows Mixed Reality](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>Wenn AltspaceVR meldet, dass die aktuelle Version veraltet ist:

* Die Version der anwendung, die Sie verwenden, wird nicht mehr unterstützt. Wenn Sie AltspaceVR über eine Storefront heruntergeladen haben, wurde das Update möglicherweise vor Kurzem gestartet, bevor Ihr Store Ihren Client aktualisieren konnte.
* Wenn Sie das Update erzwingen möchten, können Sie dies über die verschiedenen Storefronts tun:
    * **Microsoft Store:** [Microsoft Store Support – Updates für Apps und Spiele in Microsoft Store](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Öffnen Sie Ihre Oculus-Bibliothek, und navigieren Sie in der linken Navigationsleiste zu "Updates".
    * **Wasserturbinen:** [Unterstützung von Wasserturbinen – Update & Installationsprobleme](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>Wenn das Programm funktioniert hat, aber nach dem Update nicht mehr gestartet wurde:

* Installieren Sie die Software neu. Dies erfordert, dass Sie vorhandene Versionen der Anwendung deinstallieren oder entfernen. Nachdem Sie Altspace vollständig aus Ihrem System entfernt haben, installieren Sie Altspace über Steam, Oculus oder Microsoft Store.
* Wenn beim Starten von AltspaceVR ein Problem besteht, teilen Sie uns dies über ein [Supportticket mit.](https://help.altvr.com/hc/requests/new) Schließen Sie [eine Protokolldatei](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) aus Ihrer Sitzung ein.

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>Wenn AltspaceVR nach dem Anpassen Ihres Heimbereichs nicht gestartet werden kann:

* Navigieren Sie zur [Website Ihres Heimbereichs.](https://account.altvr.com/users/sign_in)
* Vergewissern Sie sich, dass die Vorlage Ihrer Welt noch vorhanden ist. Wenn die Vorlage für Sie freigegeben wurde, wurde sie möglicherweise vom Besitzer gelöscht, was dazu führen würde, dass Ihr Heimbereich nicht geladen wird.
    * Wenn die Vorlage gelöscht wurde, "Bearbeiten" Sie einfach die Welt im linken Bereich "World Tools", ersetzen Sie die vorhandene Vorlage durch eine andere Vorlage, und "Aktualisieren", um Änderungen zu speichern.
* Entfernen Sie alle Objekte, die möglicherweise nicht geladen werden können, indem Sie im linken Bereich "World Tools" die Option "Objekte" auswählen. Problematische Objekte können Folgendes sein:
    * Objekte aus gelöschten Kits oder aus Kits gelöschte Objekte, die noch in Ihrer Welt vorhanden sind.
    * Experimentelle GLTFs.
* Nachdem Sie die oben genannten Elemente adressiert haben, versuchen Sie, AltspaceVR erneut zu geben.

Eine erweiterte Unterstützung für Netzwerkadministratoren oder IT-Abteilungen, einschließlich Azure-IP-Adressbereiche und Diensttags, finden Sie in unseren [Downloaddetails.](https://www.microsoft.com/en-us/download/details.aspx?id=56519)

## <a name="support"></a>Support

Fragen oder Feedback für das AltspaceVR-Team? 

> [!div class="nextstepaction"]
> [Klicken Sie hier, um eine Supportanfrage zu senden.](https://help.altvr.com/hc/requests/new)