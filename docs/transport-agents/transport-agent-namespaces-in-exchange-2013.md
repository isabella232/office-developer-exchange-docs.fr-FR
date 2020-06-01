---
title: Espaces de noms de l’agent de transport dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Découvrez les classes et les membres .NET Framework que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
ms.openlocfilehash: fc2d9108c910a730bb48c5be028797f0f15ad4ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461792"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a>Espaces de noms de l’agent de transport dans Exchange 2013

Découvrez les classes et les membres .NET Framework que vous pouvez utiliser pour créer des agents de transport personnalisés pour Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Cet article fournit des informations sur les espaces de noms qui contiennent des informations de référence que vous pouvez utiliser pour créer des agents de transport pour Exchange Server 2013. Il décrit également les classes que vos agents de transport peuvent utiliser pour lire et modifier les messages électroniques qui transitent via le pipeline de transport.
  
## <a name="transport-agent-class-library"></a>Bibliothèque de classes de l’agent de transport

Les espaces de noms suivants contiennent des types que vous pouvez utiliser pour créer et étendre des agents de transport.

**Tableau 1. Espaces de noms .NET Framework**

|**Namespace**|**Description**|
|:-----|:-----|
|[Microsoft. Exchange. Data](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |Contient les types qui spécifient les exceptions de données et de configuration.  <br/> |
|[Microsoft. Exchange. Data. Common](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |Contient les types qui prennent en charge la localisation et la gestion des erreurs.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. iCalendar](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |Contient les types qui vous permettent de lire et d’écrire des données iCalendar.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. TNEF](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |Contient les types qui vous permettent de lire et d’écrire des données TNEF.  <br/> |
|[Microsoft. Exchange. Data. ContentTypes. vCard](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |Contient les types qui vous permettent de lire et d’écrire des données vCard.  <br/> |
|[Microsoft. Exchange. Data. Globalization](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |Contient les types qui vous permettent d’utiliser des cultures et des jeux de caractères pour produire du contenu localisé.  <br/> |
|[Microsoft. Exchange. Data. MIME](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |Contient les types qui vous permettent de lire et d’écrire des données MIME.  <br/> |
|[Microsoft. Exchange. Data. MIME. encoders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |Contient les types qui vous permettent de coder et de décoder les données MIME.  <br/> |
|[Microsoft. Exchange. Data. TextConverters](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |Contient les types qui vous permettent de lire et d’écrire des données avec différents formats de texte, et de convertir des données vers et à partir de ces formats.  <br/> |
|[Microsoft. Exchange. Data. transport](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |Contient les types qui vous permettent d’accéder aux informations de routage, d’hôte et de domaine relatives au pipeline de transport.  <br/> |
|[Microsoft. Exchange. Data. transport. Delivery](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |Contient les types qui prennent en charge l’extension des agents de remise Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. transport. email](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |Contient les types qui prennent en charge la création, la lecture, l’écriture et la modification de messages électroniques.  <br/> |
|[Microsoft. Exchange. Data. transport. Routing](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |Contient les types qui prennent en charge l’extension du comportement de routage de transport Exchange 2013.  <br/> |
|[Microsoft. Exchange. Data. transport. SMTP](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |Contient les types qui prennent en charge l’extension du comportement SMTP de transport Exchange 2013.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Agents de transport dans Exchange](transport-agents-in-exchange-2013.md)   
- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md) 
- 
  [Référence de l’API serveur pour Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [Éléments du fichier de configuration des agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)
    

