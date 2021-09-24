---
title: Espaces de noms d’agent de transport Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Découvrez les classes .NET Framework et les membres que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
ms.openlocfilehash: 076ddb8e2ccbdfa195a68aca6b296337a2876b55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537129"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Espaces de noms d’agent de transport Exchange 2013

Découvrez les classes .NET Framework et les membres que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les espaces de noms qui contiennent des informations de référence que vous pouvez utiliser pour créer des agents de transport pour Exchange Server 2013. Il décrit également les classes que vos agents de transport peuvent utiliser pour lire et modifier les messages électroniques qui passent par le pipeline de transport.
  
## <a name="transport-agent-class-library"></a>Bibliothèque de classes d’agent de transport

Les espaces de noms suivants contiennent des types que vous pouvez utiliser pour créer et étendre des agents de transport.

**Tableau 1. .NET Framework de noms**

|**Namespace**|**Description**|
|:-----|:-----|
|[Microsoft. Exchange. Données](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contient des types qui spécifient des exceptions de données et de configuration.  <br/> |
|[Microsoft. Exchange.Data.Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contient les types qui gèrent la localisation et la gestion des erreurs.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des données iCalendar.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.Tnef](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des données TNEF.  <br/> |
|[Microsoft. Exchange. Data.ContentTypes.vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des données vCard.  <br/> |
|[Microsoft. Exchange. Data.Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contient des types qui vous permettent d’travailler avec des cultures et des jeux de caractères pour produire du contenu localisée.  <br/> |
|[Microsoft. Exchange. Data.Mime](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des données MIME.  <br/> |
|[Microsoft. Exchange. Data.Mime.Encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contient des types qui vous permettent de coder et décoder des données MIME.  <br/> |
|[Microsoft. Exchange. Data.TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contient des types qui vous permettent de lire et d’écrire des données avec différents formats de texte, et de convertir des données vers et à partir de ces formats.  <br/> |
|[Microsoft. Exchange. Data.Transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contient des types qui vous permettent d’accéder aux informations de routage, d’hôte et de domaine sur le pipeline de transport.  <br/> |
|[Microsoft. Exchange. Data.Transport.Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contient des types qui prisent en charge l’extension Exchange agents de remise 2013.  <br/> |
|[Microsoft. Exchange. Data.Transport.Email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contient des types qui prisent en charge la création, la lecture, l’écriture et la modification de messages électroniques.  <br/> |
|[Microsoft. Exchange. Data.Transport.Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contient des types qui prisent en charge l’extension du Exchange de transport 2013.  <br/> |
|[Microsoft. Exchange. Data.Transport.Smtp](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contient des types qui prisent en charge l’extension Exchange comportement SMTP de transport 2013.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)   
- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Référence de l’API serveur pour Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

