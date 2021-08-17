---
title: Sichern von Welten
description: Erfahren Sie, wie Sie Sicherungsmomentaufnahmen Ihrer AltspaceVR-Welten erstellen, verwalten und beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Speichern
ms.openlocfilehash: 2f4f232fd843b612563b2d7425de2b5d17720c539cc02a1493bc4b118de4f117
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125470"
---
# <a name="backing-up-your-worlds"></a>Sichern von Welten

Eine Sicherung ist eine "Momentaufnahme" oder ein Datensatz aller Objekte in einer Welt zu einem bestimmten Zeitpunkt. Angenommen, Sie erstellen Ihr Dream House, und eines Tages haben Sie versehentlich das Zimmer gelöscht. Wenn Sie am Vortag eine Sicherung Ihrer Welt erstellt haben, können Sie diese bestimmte Sicherung wiederherstellen, Ihre Welt zurücksetzen und einen Panic-Angriff vermeiden. Vielleicht haben Sie auch eine Version Ihrer "NS-In-the-N"-Version für jede Saison und möchten zwischen ihnen hin- und herwechseln– dies können Sie mit Sicherungen tun. Jede Sicherung ist spezifisch für eine einzelne Welt und enthält nicht nur die Transformationen (Position, Drehung, Skalierung), sondern auch andere Einstellungen für die Objekte. Es gibt keine Beschränkung für die Anzahl von Sicherungen, die Sie für eine Welt erstellen können.  

## <a name="whats-included-in-a-backup"></a>Was ist in einer Sicherung enthalten?

Eine Sicherung umfasst derzeit die meisten Dinge, die Sie mit dem World Editor erstellen können:
* Artifacts (Kitobjekte)
* Bezeichnungen
* Teleporter
* Spawn-Punkte
* Fotos
* MRE SDK-Apps
* Native Apps (z.B. Hologramme Against Reality)

Folgendes ist nicht enthalten:

* Layoutüberschreibungen
* Skyboxes und Ambient Sound
* Vorlagen
* Anweisungen
* Weltrollen und kontextbezogene Rollen

## <a name="managing-backups"></a>Verwalten von Sicherungen

Sie können eine Sicherung erstellen, indem Sie ihren World Editor/Altspace öffnen und auf "Sicherungen" klicken. Die erste Schaltfläche ist die Schaltfläche "Neue Sicherung". Beim Erstellen einer Sicherung werden Sie aufgefordert, einen Kurznamen einderherzustellen. Dies ist optional, wird aber dringend empfohlen, da es schnell verwirrend wird. Vorhandene Sicherungen werden nach der Schaltfläche "Erstellen" aufgelistet. Wenn Sie auf eine vorhandene Sicherung klicken, wird eine Wiederherstellung gestartet. Wenn Sie eine Sicherung wiederherstellen, wird Ihre Welt nach einigen Augenblicken zurückgesetzt, aber die Änderungen werden möglicherweise nicht widergespiegelt. Warten Sie ein oder zwei Minuten, und setzen Sie Ihre Welt erneut zurück. **Es gibt derzeit keine Möglichkeit, eine** Sicherung in VR zu bearbeiten oder zu löschen. Sie müssen Ihre Sicherungen vorerst auf unserer Website verwalten. (Die Sicherungsverwaltung in VR wird in Kürze verbessert. In der Zwischenzeit sollten Sie mit uns zusammenarbeiten.

So verwalten Sie Ihre Sicherungen auf unserer Website:

1. Navigieren Sie [zu Worlds > Mine,](https://account.altvr.com/users/sign_in)suchen Sie Ihre Welt, und drücken Sie in den Administratorsteuerelementen "Sicherungen":

![Administratorsteuerelemente auf der Worlds-Website mit geöffneten Sicherungen](images/world-backup-img-01.png)

2. Sie können Sicherungen erstellen, bearbeiten und löschen, überprüfen, wie viele Objekte sich darin befinden, und sogar ein Vorschaubild hochladen: 

![Fenster "Sicherungen" mit hervorgehobenen Befehlen zum Erstellen, Bearbeiten und Löschen](images/world-backup-img-02.png)

Es gibt keine Beschränkung für die Anzahl von Sicherungen, und mehr Sicherungen wirken sich nicht auf die Leistung Ihrer Welt aus.

## <a name="other-ways-to-back-up-your-worlds"></a>Andere Möglichkeiten zum Sichern Ihrer Welten

* Erstellen Sie eine weitere Welt, zeigen Sie erweiterte Optionen an, und importieren Sie aus der Welt. Wählen Sie die Zu sichernde Welt aus dem Dropdownmenü in der neuen aus. Es gibt keine Beschränkung für Importe.
* Wenn Sie unity Uploader verwenden, wird dringend empfohlen, die Versionskontrolle zu verwenden. Beispiel: [GitHub für Unity](https://unity.github.com).

## <a name="troubleshooting"></a>Problembehandlung

**Hilfe! Ich habe versehentlich eine Sicherung wiederhergestellt, und meine Arbeit ist nicht** mehr wichtig. Wir erstellen automatisch eine neue Sicherung, bevor wir die alte Wiederherstellen durchführen. Suchen Sie nach einem Namen mit einem Namen, der mit **Auto** mit dem richtigen Zeitstempel beginnt, und stellen Sie diesen wiederhergestellt (z. B. **Auto 2019-01-14T08:23:33-08:00**).  Wenn dies nicht funktioniert, übermitteln Sie [eine Supportanfrage](https://help.altvr.com/hc/requests/new)

**Ich habe eine Sicherung wiederhergestellt, und einige Objekte fehlen.** Wurden diese Fotos gelöscht, falls fotos? Gelöschte Fotos können aus Datenschutzgründen nicht wiederhergestellt werden. Übermitteln Sie [eine Supportanfrage,](https://help.altvr.com/hc/requests/new) damit wir sie untersuchen können.

**Ich sehe keine Änderungen.** Sicherungen werden asynchron wiederhergestellt, was bedeutet, dass die Wiederherstellung je nach Anzahl der Objekte einige Minuten dauern kann. Denken Sie daran, Ihre Welt zurückzusetzen, und versuchen Sie es erneut, wenn nach einigen Minuten nichts mehr zu sehen ist. In Zukunft können wir weitere Feedback zum Status des Wiederherstellungsprozesses geben.