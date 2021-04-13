---
title: Gewähren von Welt Rollen
description: Erfahren Sie mehr über das System "Rollen und Fähigkeiten" und erhalten Sie Schritt-für-Schritt-Anleitungen für die Bereitstellung von Benutzern in ihren altspacevr-Welten.
ms.date: 03/11/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212200"
---
# <a name="granting-world-roles"></a>Gewähren von Welt Rollen

In "altspace" ist ein System für Rollen und Fähigkeiten fest. Jede Person kann über mehrere Rollen verfügen, und ihre Rollen können abhängig davon, wo Sie sich befinden, unterschiedlich sein. Jede Rolle bietet Ihnen wiederum eine oder mehrere Funktionen. Wenn Sie sich z. b. in Ihrem eigenen Ereignis befinden, erhalten Sie automatisch die **Presenter** -und **Moderator** -Rollen. Mit diesen beiden Rollen können Sie unruly-Benutzer starten, sich in der Phase befinden und das-Programm möglicherweise freigeben. 

1. Bearbeiten Sie Ihre Welt, und Scrollen Sie nach unten zum Abschnitt **in VR** ([Verwalten von Welten](managing-worlds.md)).

![Ändern von Rollen im VR-Abschnitt der Welten](images/granting-roles.png)

2. Bearbeiten Sie das Feld " **Rollen** ", wenn Sie bestimmten Benutzern bestimmte Rollen nur für diese Welt gewähren möchten. Wenn Sie z. b. **Presenter**  +  **Moderator** und Calen **Moderator** geben möchten, fügen Sie Folgendes hinzu, und wählen Sie **Speichern** aus. Das Format ist in jeder Zeile " **{Role}", "{username" oder "Email}** ". Beim Benutzernamen wird die Groß-/Kleinschreibung 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. Wenn Sie erneut **Bearbeiten** auswählen, sollte Folgendes über dem Feld Rollen angezeigt werden. So haben Sie in der Datenbank aktualisiert.

```
Presenters: jimmy
Moderators: jimmy,calen
```

* Damit die Änderungen in altspace wirksam werden, sollten Sie die Welt zurücksetzen und alle wiederherstellen. Unten finden Sie eine vollständige Liste der Rollen.

4. Bearbeiten Sie das Feld " **Kontext Rollen** ", wenn Sie jeder Rolle, die der Welt Beitritt, eine Rolle erteilen möchten. Wenn Sie z. b. möchten, dass die Benutzer das Megafon ausführen und das Megafon verwenden können

```
pilot,megaphone_only
```

Nachdem Sie **Aktualisieren** ausgewählt haben, setzen Sie die Welt zurück. Dies wirkt sich nur auf diese Welt aus. Wenn Sie Rollen einem gesamten Universum zuweisen möchten, bearbeiten Sie die gleichen Felder im Universum. 

## <a name="roles"></a>Rollen 

* **Presenter** -Funktionen wie die Bereitstellung auf der Stufe
* **Moderator** : Funktionen wie " **Kick** " zur Wartung von Decorum
* **Terraex** -Möglichkeit zur Verwendung des World-Editors
* **Pilot Projekt** : Möglichkeit zum Umschalten des laufenden Modus und zum Erzeugen des 6DOF-Flight-Tools
* **Megaphone_only** die Möglichkeit, in den Ohren von Benutzern zu sprechen, wo Sie sich auf der Welt befinden
* **Showcase_new_sdk** Fähigkeit, MRE SDK-apps zu erzeugen

## <a name="troubleshooting"></a>Problembehandlung

**Kann ich Rollen löschen?**
Nicht aus dem Formular zurzeit können Sie eine Supportanfrage unter Help.altvr.com, und wir kümmern uns um die Datei.

**Werden die Rollen kopiert, wenn eine Welt aus einer anderen importiert wird?**
Nein, Rollen werden nicht kopiert.