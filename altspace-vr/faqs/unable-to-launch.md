---
title: Ich kann "altspacevr" nicht starten.
description: Erfahren Sie, wie Sie Probleme im Zusammenhang mit dem Starten Ihrer altspacevr-Umgebung identifizieren, melden und beheben.
ms.date: 02/10/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: fc49b5b7ed708e43a12616d782a397a364b2264e
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213132"
---
# <a name="i-cant-launch-altspacevr"></a>Ich kann "altspacevr" nicht starten.

Es gibt mehrere Gründe, warum altspacevr möglicherweise nicht für Sie gestartet wird. Führen Sie die folgenden Schritte aus, um sicherzustellen, dass die Anwendung mit der erforderlichen Drittanbieter Software ordnungsgemäß installiert ist.

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>Wenn Sie versuchen, altspacevr zum ersten Mal zu starten, gehen Sie wie folgt vor:

1. Stellen Sie sicher, dass Ihr Gerät unterstützt wird und den [mindestens angegebenen Anforderungen](../getting-started/system-requirements.md)entspricht.
2. Stellen Sie sicher, dass die neueste [Oculus-Software](https://www.oculus.com/setup) installiert ist und dass Einstellungen-> Allgemein > unbekannte Geräte auf ON festgelegt sind. Wenn Sie im 2D-Modus starten, ist die Installation von Oculus nicht erforderlich.
3. Stellen Sie sicher, dass Sie über eine funktionierende Internetverbindung verfügen. Wenn Sie versuchen, altspace innerhalb einer Netzwerk Firewall zu starten, öffnen Sie die UDP-Ports 5055 und 5056 sowie die TCP-Ports 80 und 443. Wenn Sie sich im Netzwerk einer Unternehmens-oder Bildungs Firewall befinden, müssen Sie sich möglicherweise an den Netzwerkadministrator oder die IT-Abteilung wenden.
4. Weitere Informationen:
    * [Installieren von altspacevr für Oculus Quest](../getting-started/oculus-installation.md)
    * [Installieren von altspacevr für Windows Mixed Reality](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>Wenn altspacevr meldet, dass die aktuelle Version veraltet ist:

* Die Version der Anwendung, die Sie verwenden, wird nicht mehr unterstützt. Wenn Sie altspacevr über eine Store Front heruntergeladen haben, wurde das Update möglicherweise vor kurzem gestartet, bevor Ihr Kunde den Client aktualisieren konnte.
* Wenn Sie die Aktualisierung erzwingen möchten, können Sie dies über die verschiedenen Storefronts durchführen:
    * **Microsoft Store:** [Microsoft Store-Unterstützung: Updates für apps und Spiele in Microsoft Store erhalten](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Öffnen Sie Ihre Oculus-Bibliothek, und navigieren Sie in der linken Navigationsleiste zu "Updates".
    * **Steam:** [Unterstützung für das Update & Installationsprobleme](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>Wenn das Programm funktioniert, aber nach dem Update nicht mehr gestartet wurde:

* Führen Sie eine Neuinstallation der Software durch. Dies erfordert, dass Sie vorhandene Versionen der Anwendung deinstallieren oder entfernen. Installieren Sie nach dem vollständigen Entfernen aus Ihrem System altspace über "Steam", "Oculus" oder "Microsoft Store".
* Wenn Sie ein Problem beim Starten von altspacevr haben, informieren Sie uns über ein [Support Ticket](https://help.altvr.com/hc/requests/new). Fügen Sie eine [Protokolldatei](uploading-client-logs.md) aus Ihrer Sitzung ein.

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>Wenn "altspacevr" nicht gestartet werden kann, nachdem Sie Ihren Home-Bereich angepasst haben:

* Navigieren Sie zur [Website Ihres Heim Platzes](https://account.altvr.com/users/sign_in).
* Vergewissern Sie sich, dass die Vorlage ihrer Welt noch vorhanden ist. Wenn die Vorlage für Sie freigegeben wurde, wurde Sie möglicherweise vom Besitzer gelöscht, was dazu führen würde, dass der Startbereich nicht geladen wird.
    * Wenn die Vorlage gelöscht wurde, können Sie die Welt einfach im linken Bereich "World Tools" Bearbeiten, die vorhandene Vorlage durch eine andere Vorlage ersetzen und "Aktualisieren", um die Änderungen zu speichern.
* Entfernen Sie alle Objekte, die möglicherweise nicht geladen werden können, indem Sie im linken Bereich "World Tools" den Wert "Objects" auswählen. Problematische Objekte können Folgendes umfassen:
    * Objekte aus gelöschten Kits oder Objekten, die aus Kits gelöscht wurden und in ihrer Welt noch vorhanden sind.
    * Experimentelles gltfs.
* Nachdem Sie die obigen Elemente adressiert haben, versuchen Sie, altspacevr erneut einzugeben.

Erweiterte Unterstützung für Netzwerkadministratoren oder IT-Abteilungen, einschließlich Azure-IP-Adressbereichen und Dienst Tags, finden Sie in unseren [Download Details](https://www.microsoft.com/en-us/download/details.aspx?id=56519).