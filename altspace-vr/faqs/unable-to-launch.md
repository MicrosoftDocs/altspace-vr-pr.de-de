---
title: Ich kann AltspaceVR nicht starten.
description: Erfahren Sie, wie Sie Probleme im Zusammenhang mit dem Starten Ihrer AltspaceVR-Umgebung identifizieren, melden und beheben.
ms.date: 02/10/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: 50edddef669aca14640fd6e910c12c15864cf46a099e54bceed40494e9817de4
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127928"
---
# <a name="i-cant-launch-altspacevr"></a>Ich kann AltspaceVR nicht starten.

Es gibt mehrere Gründe, warum AltspaceVR möglicherweise nicht für Sie gestartet wird. Probieren Sie die folgenden Schritte aus, um sicherzustellen, dass die Anwendung mit der erforderlichen Drittanbietersoftware ordnungsgemäß installiert ist.

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>Wenn Sie versuchen, ALTSPACEVR zum ersten Mal zu starten:

1. Vergewissern Sie sich, dass Ihr Gerät unterstützt wird und die [angegebenen Mindestanforderungen](../getting-started/system-requirements.md)erfüllt.
2. Stellen Sie sicher, dass die neueste [Oculus Software](https://www.oculus.com/setup) installiert ist und Einstellungen-> Allgemein > Unbekannte Geräte auf EIN festgelegt ist. Wenn Sie im 2D-Modus starten, muss Oculus nicht installiert sein.
3. Stellen Sie sicher, dass Sie über eine funktionierende Internetverbindung verfügen. Wenn Sie versuchen, Altspace innerhalb einer Netzwerkfirewall zu starten, öffnen Sie die UDP-Ports 5055 und 5056 sowie die TCP-Ports 80 und 443. Wenn Sie sich innerhalb des Netzwerks einer Unternehmens- oder Bildungsfirewall befinden, müssen Sie sich möglicherweise an den Netzwerkadministrator oder die IT-Abteilung wenden.
4. Weitere Informationen:
    * [Installieren von AltspaceVR für Oculus Quest](../getting-started/oculus-installation.md)
    * [Installieren von AltspaceVR für Windows Mixed Reality](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>Wenn AltspaceVR meldet, dass die aktuelle Version veraltet ist:

* Die Version der Anwendung, die Sie verwenden, wird nicht mehr unterstützt. Wenn Sie AltspaceVR über eine Storefront heruntergeladen haben, wurde das Update möglicherweise vor Kurzem gestartet, bevor Ihr Store Ihren Client aktualisieren konnte.
* Wenn Sie ein Update erzwingen möchten, können Sie dies über die verschiedenen Storefronts durchführen:
    * **Microsoft Store:** Microsoft Store Support – [Updates für Apps und Spiele in Microsoft Store](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Öffnen Sie Ihre Oculus-Bibliothek, und navigieren Sie in der linken Navigationsleiste zu "Updates".
    * **Steam:** [Steam-Unterstützung](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334) – Update & Installationsprobleme

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>Wenn das Programm funktioniert hat, aber nach dem Update gestartet werden soll:

* Bereinigen Sie die Software neu. Dazu müssen Sie vorhandene Versionen der Anwendung deinstallieren oder entfernen. Nachdem Sie Altspace vollständig aus Ihrem System entfernt haben, installieren Sie altspace über Steam, Oculus oder Microsoft Store.
* Wenn beim Starten von AltspaceVR ein Problem auftritt, teilen Sie uns dies über ein [Supportticket](https://help.altvr.com/hc/requests/new)mit. Fügen Sie eine [Protokolldatei](uploading-client-logs.md) aus Ihrer Sitzung ein.

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>Wenn AltspaceVR nach dem Anpassen Ihres Startbereichs nicht gestartet werden kann:

* Navigieren Sie zur Website Ihres [Heimbereichs.](https://account.altvr.com/users/sign_in)
* Vergewissern Sie sich, dass die Vorlage Ihrer Welt noch vorhanden ist. Wenn die Vorlage für Sie freigegeben wurde, wurde sie möglicherweise vom Besitzer gelöscht, was dazu führen würde, dass Ihr Stammspeicherplatz nicht geladen wird.
    * Wenn die Vorlage gelöscht wurde, ersetzen Sie einfach "Bearbeiten" im linken Bereich "World Tools" die vorhandene Vorlage durch eine andere Vorlage und "Aktualisieren", um Änderungen zu speichern.
* Entfernen Sie alle Objekte, die möglicherweise nicht geladen werden können, indem Sie im linken Bereich "World Tools" die Option "Objekte" auswählen. Problematische Objekte können Folgendes umfassen:
    * Objekte aus gelöschten Kits oder Aus Kits gelöschte Objekte, die noch in Ihrer Welt vorhanden sind.
    * Experimentelle GLTFs.
* Nachdem Sie die oben genannten Elemente adressiert haben, versuchen Sie, AltspaceVR erneut einzusenden.

Eine erweiterte Unterstützung für Netzwerkadministratoren oder IT-Abteilungen, einschließlich Azure-IP-Adressbereiche und Diensttags, finden Sie in unseren [Downloaddetails.](https://www.microsoft.com/en-us/download/details.aspx?id=56519)