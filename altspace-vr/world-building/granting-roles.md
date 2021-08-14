---
title: Gewähren von Weltrollen
description: Erfahren Sie mehr über das Rollen- und Fähigkeitensystem, und erhalten Sie schrittweise Anweisungen zum Erteilen von Benutzerrollen in Ihren AltspaceVR-Welten.
ms.date: 04/14/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: f299f637d77c989be5504532279fb42451367b4ac53095d00627f67402dd8552
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127118"
---
# <a name="granting-world-roles"></a>Gewähren von Weltrollen

Altspace verfügt über ein Rollen- und Fähigkeitensystem. Jede Person kann über mehrere Rollen verfügen, und ihre Rollen können je nach Position unterschiedlich sein. Jede Rolle wiederum bietet Ihnen eine oder mehrere Fähigkeiten. Wenn Sie sich beispielsweise an Ihrem eigenen Ereignis beteiligen, erhalten Sie automatisch die **Host-** und **Moderatorrollen.** Mit diesen beiden Rollen können Sie unruly users (Unruly Users) starten, sich auf der Stage befinden und die Conf dll möglicherweise freigeben.

1. Bearbeiten Sie Ihre Welt, und sehen Sie sich die rechte Spalte für **Kontextrollen** an ([Verwalten von Welten](managing-worlds.md))

![Ändern von Rollen im Abschnitt Kontextrollen von Welten](images/granting-roles.png)

2. Klicken Sie im Feld **Kontextrollen** auf **Benutzer hinzufügen,** wenn Sie bestimmten Benutzern nur für diese Welt bestimmte Rollen gewähren möchten. Wenn Sie mir beispielsweise   +  **Hostmoderator** geben möchten, fügen Sie die oben genannten hinzu und wählen **Speichern** aus. Das Format lautet **Benutzername,** Benutzername beachtet die Groß-/Kleinschreibung nicht. Wählen Sie im Dropdownmenü **Terraformer** die Rolle aus, klicken Sie mehrmals auf Benutzer hinzufügen, um weitere Benutzer hinzuzufügen, und klicken Sie dann auf **Aktualisieren.**

* Damit die Änderung in Altspace wirksam wird, sollten Sie Die Welt auf Den Raum zurücksetzen erzwingen, sodass alle Benutzer erneut teilnehmen müssen, oder dass jeder Benutzer mit einer neuen Rolle der Welt wieder beigeordnet wird.

3. Bearbeiten Sie das Feld **Standardkontextrollen** im Abschnitt **In VR,** wenn Sie jeder Rolle, die Ihrer Welt beitritt, eine Rolle gewähren möchten. Wenn Sie z. B. zulassen möchten, dass Personen das Megaphone verwenden, damit sie sich während des fernen Teils gegenseitig hören können, fügen Sie Folgendes hinzu:

```
pilot,megaphone_only
```

Nachdem Sie **Aktualisieren** ausgewählt haben, setzen Sie Speicherplatz auf der Ganzen Welt zurück. Dies wirkt sich nur auf diese Welt aus. Wenn Sie einem ganzen Universe Rollen gewähren möchten, bearbeiten Sie die gleichen Felder im Universe. Dasselbe gilt für Ereignisse. Wenn sie möchten, dass alle Benutzer in Ihrem Ereignis über diese Rollen verfügen, müssen Sie dies den **Standardkontexualrollen** des Ereignisses selbst hinzufügen.

## <a name="roles"></a>Rollen

* **Megaphone_only:** Fähigkeit, sich überall auf der Welt mit den Benutzern auszusprechen
* **Moderator:** Fähigkeiten wie **Kick** zum Verwalten des Decorums
* **Pilot:** Möglichkeit zum Umschalten des Fly-Modus und zum Erstellen des 6DOF-Flugtools
* **Host:** Funktionen wie die Möglichkeit, auf der Stage zu sein, megaphone
* **Terraformer** : Möglichkeit zur Verwendung des World Editor Weitere Informationen zu ([Rollen in Ereignissen, Welten, Gruppen und in AltspaceVR](../getting-started/roles.md))

## <a name="troubleshooting"></a>Problembehandlung

**Kann ich Rollen löschen?**
Ja, bearbeiten Sie Ihre Welt, klicken Sie unter der Rolle, die Sie löschen möchten, auf **Entfernen,** und klicken Sie auf **Aktualisieren.**

**Werden Rollen kopiert, wenn eine Welt aus einer anderen importiert wird?**
Nein, Rollen werden nicht kopiert