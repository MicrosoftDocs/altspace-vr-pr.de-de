---
title: Gewähren von World-Rollen
description: Erfahren Sie mehr über das Rollen- und Fähigkeitssystem, und erhalten Sie schritt-für-Schritt-Anweisungen zum Zuweisen von Rollen für Benutzer in Ihren AltspaceVR-Welten.
ms.date: 04/14/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923192"
---
# <a name="granting-world-roles"></a>Gewähren von World-Rollen

Altspace verfügt über ein Rollen- und Fähigkeitssystem. Jede Person kann über mehrere Rollen verfügen, und ihre Rollen können sich je nach Ihrem Ort unterscheiden. Jede Rolle wiederum bietet Ihnen eine oder mehrere Fähigkeiten. Wenn Sie sich beispielsweise in Ihrem eigenen Ereignis sind, erhalten Sie automatisch die **Host-** und **Moderatorrollen.** Mit diesen beiden Rollen können Sie unbändige Benutzer starten, auf der Stage sein und die Conf conf zu veröffentlichen.

1. Bearbeiten Sie Ihre Welt, und sehen Sie sich die rechte Spalte für **Kontextrollen** [(Verwalten von Welten) an.](managing-worlds.md)

![Ändern von Rollen im Abschnitt "Kontextrollen" von Welten](images/granting-roles.png)

2. Klicken **Sie im Feld** **Kontextrollen** auf Benutzer hinzufügen, wenn Sie bestimmten Benutzern nur für diese Welt bestimmte Rollen zuweisen möchten. Wenn Sie mir z. B. host moderator **geben** möchten, fügen Sie  +  den oben genannten hinzu, und wählen Sie **Speichern aus.** Das Format ist **Benutzername,** bei Benutzername wird die Groß-/Kleinschreibung nicht beachtet. Wählen Sie die Rolle im Dropdownmenü **Terraformer** aus, klicken Sie mehrmals auf Benutzer hinzufügen, um weitere Benutzer hinzuzufügen, und klicken Sie dann **auf Aktualisieren.**

* Damit die Änderung in Altspace wirksam wird, sollten Sie "Space the world" zurücksetzen, um alle Benutzer zu zwingen, wieder dabei zu sein oder jeden Benutzer mit einer neuen Rolle wieder in die Welt zu nehmen.

3. Bearbeiten Sie **das Feld Standardmäßige** kontextbezogene Rollen im Abschnitt **In VR,** wenn Sie jeder Rolle, die Ihrer Welt beitritt, eine Rolle zuweisen möchten. Wenn Sie z. B. personen das Megaphone zum Fliegt und verwenden möchten, damit sie sich im fernen Teil hören können, fügen Sie Folgendes hinzu:

```
pilot,megaphone_only
```

Nachdem Sie Aktualisieren **ausgewählt haben,** setzen Sie den Speicherplatz in der Welt zurück. Dies wirkt sich nur auf diese Welt aus. Wenn Sie einem gesamten Universe Rollen zuweisen möchten, bearbeiten Sie die gleichen Felder im Universe. Dasselbe gilt für Ereignisse. Wenn Sie möchten, dass alle Benutzer in Ihrem Ereignis über diese Rollen verfügen, müssen Sie diese zu den **Standardkontexrollen** des Ereignisses selbst hinzufügen.

## <a name="roles"></a>Rollen

* **Megaphone_only:** Möglichkeit, überall auf der Welt in die Menschen zu sprechen
* **Moderator:** Fähigkeiten wie **"Kick"** zum Verwalten des Anstands
* **Pilot:** Möglichkeit zum Umschalten des Flymodus und Zum Erstellen des 6DOF-Flugtools
* **Host:** Fähigkeiten wie die Möglichkeit, auf der Stage zu sein, megaphone
* **Terraformer:** Möglichkeit, den World Editor zu verwenden Weitere Informationen zu ( Rollen in Ereignissen, Welten, Gruppen und [in AltspaceVR](../getting-started/roles.md))

## <a name="troubleshooting"></a>Problembehandlung

**Kann ich Rollen löschen?**
Ja, bearbeiten Sie Ihre Welt, klicken Sie **unterhalb** der Rolle, die Sie löschen möchten, auf Entfernen, und klicken Sie auf **Aktualisieren.**

**Werden Rollen kopiert, wenn eine Welt aus einer anderen importiert wird?**
Nein, Rollen werden nicht kopiert.