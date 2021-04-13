---
title: Sichern Ihrer Welt
description: Erfahren Sie, wie Sie Sicherungs Momentaufnahmen Ihrer altspacevr-Welten erstellen, verwalten und beheben.
ms.date: 03/11/2021
ms.topic: article
keywords: Speichern
ms.openlocfilehash: fdef692c737bf2f92db315e04556831d60c2f377
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212130"
---
# <a name="backing-up-your-worlds"></a>Sichern Ihrer Welt

Eine Sicherung ist eine "Momentaufnahme" oder ein Datensatz aller Objekte in einer Welt zu einem bestimmten Zeitpunkt. Angenommen, Sie entwickeln Ihr Traum Haus und einen Tag, an dem Sie versehentlich den Wohnraum gelöscht haben. Wenn Sie den Tag vorher eine Sicherung ihrer Welt erstellt haben, können Sie diese bestimmte Sicherung wiederherstellen, ihre Welt zurücksetzen und einen Panik Angriff vermeiden. Oder vielleicht haben Sie eine Version ihrer in-the-Woods-Version für jede Jahreszeit, und Sie möchten zwischen ihnen hin und her wechseln – Sie können dies mit Sicherungen tun. Jede Sicherung ist für eine einzelne Welt spezifisch und enthält nicht nur die Transformationen (Position, Drehung, Skala), sondern auch andere Einstellungen für die Objekte. Es gibt keine Beschränkung für die Anzahl von Sicherungen, die Sie für eine Welt erstellen können.  

## <a name="whats-included-in-a-backup"></a>Was ist in einer Sicherung enthalten?

Eine Sicherung umfasst derzeit die meisten Dinge, die Sie mit dem Welt-Editor erzeugen können:
* Artefakte (Kit-Objekte)
* Bezeichnungen
* Teleportierer
* Punkt Punkte
* Fotos
* MRE SDK-apps
* Native Apps (z. b. holograms für die Realität)

Folgendes ist nicht enthalten:

* Layoutüberschreibungen
* Skyboxes und Ambient Sound
* Vorlagen
* Anweisungen
* Welt Rollen und kontextabhängige Rollen

## <a name="managing-backups"></a>Verwalten von Sicherungen

Sie können eine Sicherung erstellen, indem Sie den World Editor/altspace öffnen und auf "Backups" klicken. Die erste Schaltfläche ist die Schaltfläche "neue Sicherung". Wenn Sie eine Sicherung erstellen, werden Sie zur Angabe eines Kurznamens aufgefordert. Dies ist optional, wird aber dringend empfohlen, da es verwirrend ist. Vorhandene Sicherungen werden nach der Schaltfläche "erstellen" aufgelistet. Wenn Sie auf eine vorhandene Sicherung klicken, wird eine Wiederherstellung gestartet. Wenn Sie eine Sicherung wiederherstellen, wird Ihre Welt nach einigen Augenblicken zurückgesetzt, die Änderungen werden jedoch möglicherweise nicht angezeigt. Warten Sie ein oder zwei Minuten, und setzen Sie Ihre Welt wieder zurück. **Zurzeit gibt es keine Möglichkeit, eine Sicherung in VR zu bearbeiten oder zu löschen**. Sie müssen Ihre Sicherungen jetzt auf unserer Website verwalten. (Die Sicherungs Verwaltung in VR wird bald verbessert. In der Zwischenzeit haben wir uns mit uns in der Zeit.

So verwalten Sie Ihre Sicherungen auf unserer Website:

1. Navigieren Sie zu "World [>](https://account.altvr.com/users/sign_in)My", suchen Sie nach ihrer Welt, und drücken Sie "Backups" in den Administrator Steuerelementen:

![Administrator Steuerelemente auf der Website Website mit geöffneten Sicherungs Bereich](images/world-backup-img-01.png)

2. Sie können Ihre Sicherungen erstellen, bearbeiten und löschen, überprüfen, wie viele Objekte sich in befinden, und sogar ein Vorschaubild hochladen: 

![Fenster "Sicherungen" mit hervorgehobenen Befehlen zum Erstellen, bearbeiten und löschen](images/world-backup-img-02.png)

Es gibt keine Beschränkung für die Anzahl der Sicherungen, und eine größere Anzahl von Sicherungen wirkt sich nicht auf die Leistung der Welt aus.

## <a name="other-ways-to-back-up-your-worlds"></a>Weitere Möglichkeiten zum Sichern Ihrer Welten

* Erstellen Sie eine andere Welt, zeigen Sie erweiterte Optionen an, und importieren Sie aus der Welt. Wählen Sie im Dropdown Menü die Welt aus, die Sie sichern möchten, in der neuen. Es gibt keine Beschränkung für Importe.
* Wenn Sie das Unity-Uploader verwenden, wird dringend empfohlen, die Versionskontrolle zu verwenden. Beispiel: [GitHub für Unity](https://unity.github.com).

## <a name="troubleshooting"></a>Problembehandlung

**Hilfe! Ich habe versehentlich eine Sicherung wieder hergestellt, und meine Arbeit ist** nicht mit der Sorge. Vor dem Wiederherstellen der alten Sicherung wird automatisch eine neue Sicherung erstellt. Suchen Sie nach einem Namen, der mit " **Auto** " mit dem richtigen Zeitstempel beginnt, und stellen Sie diesen wieder her (z **. b. Auto 2019-01-14t08:23:33-08:00**).  Wenn dies nicht funktioniert, senden Sie eine [Supportanfrage](https://help.altvr.com/hc/requests/new)

**Ich habe eine Sicherung wieder hergestellt, und einige Objekte fehlen** . Waren diese Fotos gelöscht, wenn Sie Fotos waren? Aus Datenschutzgründen können gelöschte Fotos nicht wieder hergestellt werden. Senden Sie eine [Supportanfrage](https://help.altvr.com/hc/requests/new) , damit wir untersuchen können.

**Ich sehe keine Änderungen** . Sicherungen werden asynchron wieder hergestellt, d. h., die Wiederherstellung kann je nach Anzahl der Objekte einige Minuten dauern. Denken Sie daran, ihre Welt zurückzusetzen. Wenn Sie nach einigen Minuten nichts sehen, versuchen Sie es erneut. In Zukunft können wir mehr Feedback zum Status des Wiederherstellungs Vorgangs bereitstellen.