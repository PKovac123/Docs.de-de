---
title: Artikel mit einzelnen Benutzerkonten erstellten ASP.NET Core-Projekten
author: rick-anderson
description: Lesen Sie Artikel, die basierend auf ASP.NET Core-Projekte, die mit individuellen Benutzerkonten erstellt.
ms.author: riande
ms.date: 11/30/2017
uid: security/authentication/individual
ms.openlocfilehash: ac843342ffc73632fbf9f6359c6c1a5878dcef0d
ms.sourcegitcommit: c12ebdab65853f27fbb418204646baf6ce69515e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/21/2018
ms.locfileid: "46523063"
---
# <a name="articles-based-on-aspnet-core-projects-created-with-individual-user-accounts"></a>Artikel mit einzelnen Benutzerkonten erstellten ASP.NET Core-Projekten

ASP.NET Core Identity ist in-Projektvorlagen in Visual Studio mit der Option "Einzelne Benutzerkonten" enthalten.

Die Authentifizierung-Beispielvorlagen stehen im .NET Core-CLI mit `-au Individual`:

::: moniker range=">= aspnetcore-2.1"

```console
dotnet new mvc -au Individual
dotnet new webapi -au Individual
dotnet new webapp -au Individual
```

::: moniker-end

::: moniker range="= aspnetcore-2.0"

```console
dotnet new mvc -au Individual
dotnet new webapi -au Individual
dotnet new razor -au Individual
```

::: moniker-end

<a name="no"></a>
## <a name="no-authentication"></a>Keine Authentifizierung

Gibt die Authentifizierung in .NET Core-CLI mit dem `-au` Option. In Visual Studio die **Authentifizierung ändern** Dialogfeld für neue Webanwendungen verfügbar ist. Der Standardwert für neue Web-apps in Visual Studio ist **keine Authentifizierung**.

Projekte, die ohne Authentifizierung erstellt werden:

* Enthalten Sie nicht, Web Pages und die Benutzeroberfläche für die Anmeldung, und melden Sie sich ab.
* Enthalten Sie nicht Code für die Authentifizierung.

<a name="win"></a>
## <a name="windows-authentication"></a>Windows-Authentifizierung

Windows-Authentifizierung angegeben ist, für die neue Web-apps in .NET Core-CLI mit dem `-au Windows` Option. In Visual Studio die **Authentifizierung ändern** Dialogfeld bietet die **Windows-Authentifizierung** Optionen.

Wenn Windows-Authentifizierung ausgewählt ist, ist die app zur Verwendung konfiguriert die [-Modul für Windows-Authentifizierung IIS](xref:host-and-deploy/iis/modules). Windows-Authentifizierung ist für Intranet-Websites gedacht.

## <a name="additional-resources"></a>Zusätzliche Ressourcen

Die folgenden Artikel zeigen, wie mit den generierten Code in ASP.NET Core-Vorlagen, die einzelne Benutzerkonten zu verwenden:

* [Zweistufige Authentifizierung mit SMS](xref:security/authentication/2fa)
* [Account confirmation and password recovery in ASP.NET Core (Kontobestätigung und Kennwortwiederherstellung in ASP.NET Core)](xref:security/authentication/accconfirm)
* [Erstellen einer ASP.NET Core-app mit Benutzerdaten, die durch Autorisierung geschützt sind](xref:security/authorization/secure-data)
