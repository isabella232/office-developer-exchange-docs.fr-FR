---
title: Transport des espaces de noms de l’agent dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Obtenir des informations sur les classes .NET Framework et les membres que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
ms.openlocfilehash: a8189ca9915312b64fefda3091f8f81e51271ad6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755146"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Transport des espaces de noms de l’agent dans Exchange 2013

Obtenir des informations sur les classes .NET Framework et les membres que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les espaces de noms qui contiennent des informations de référence que vous pouvez utiliser pour créer des agents de transport pour Exchange Server 2013. Il décrit également les classes vos agents de transport peuvent utiliser pour lire et modifier des messages électroniques qui transitent par le pipeline de transport.
  
## <a name="transport-agent-class-library"></a>Bibliothèque de classes de l’agent de transport

Espaces de noms suivants contiennent des types que vous pouvez utiliser pour créer et étendre des agents de transport.

**Le tableau 1. Espaces de noms .NET framework**

|**Espace de noms**|**Description**|
|:-----|:-----|
|[Microsoft.Exchange.Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contient les types qui spécifient des exceptions de données et la configuration.  <br/> |
|[Microsoft.Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contient les types qui prennent en charge de la localisation et la gestion des erreurs.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contient les types qui vous permettent de lire et écrire des données de fichier iCalendar.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contient les types qui vous permettent de lire et écrire des données TNEF.  <br/> |
|[Microsoft.Exchange.Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contient les types qui vous permettent de lire et écrire des données de carte de visite.  <br/> |
|[Microsoft.Exchange.Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contient les types qui vous permettent de travailler avec des cultures et pour générer le contenu localisé jeux de caractères.  <br/> |
|[Microsoft.Exchange.Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contient les types qui vous permettent de lire et écrire des données MIME.  <br/> |
|[Microsoft.Exchange.Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contient les types qui permettent de coder et décoder des données MIME.  <br/> |
|[Microsoft.Exchange.Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contient les types qui vous permettent de lire et écrire des données à l’aide de différents formats et convertir des données vers et à partir de ces formats.  <br/> |
|[Microsoft.Exchange.Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contient les types qui vous permettent d’accéder aux routage, hôte et les informations de domaine sur le pipeline de transport.  <br/> |
|[Microsoft.Exchange.Data.transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contient les types qui prennent en charge l’extension des agents de remise Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contient les types qui prennent en charge la création, lecture, écriture et modification les messages électroniques.  <br/> |
|[Microsoft.Exchange.Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contient les types qui prennent en charge l’extension du comportement de routage de transport Exchange 2013.  <br/> |
|[Microsoft.Exchange.Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contient les types qui prennent en charge l’extension du comportement SMTP transport Exchange 2013.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)   
- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md) 
- [Référence des API du serveur pour Exchange](http://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

