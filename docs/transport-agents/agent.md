---
title: agent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Last modified: September 17, 2015'
ms.openlocfilehash: 8bcfdd9bffd4c7a15af40528fd431a99c7868637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520967"
---
# <a name="agent"></a>agent
  
**S’applique à :** Exchange Server 2013
  
**L’élément agent** contient des informations de configuration sur un agent installé. 
  
- [configuration](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
- [agent](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**agentType (complexType)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**nom** <br/> |Nom spécifié lors de l’installation de l’agent. Cet attribut requiert une valeur de chaîne nonempty qui contient un maximum de 64 caractères.  <br/> |
|**baseType** <br/> |Nom complet, y compris l’espace de noms, de la classe dont dérive l’agent. Cet attribut requiert une valeur de chaîne nonempty qui contient au moins un caractère.  <br/> |
|**classFactory** <br/> |Nom complet, y compris l’espace de noms, de la classe qui implémente la fabrique d’agents qui crée des instances de l’agent. Cet attribut doit contenir le nom complet de la classe qui implémente la fabrique d’agents qui crée des instances de l’agent. Cette classe doit dériver de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)  <br/> |
|**assemblyPath** <br/> |Chemin d’accès complet, y compris le nom de fichier, de l’assembly qui contient le code de l’agent. Cet attribut requiert une valeur de chaîne nonempty qui contient au moins un caractère.  <br/> |
|**enabled** <br/> |Valeur boolé américaine qui indique si l’agent est activé. La valeur est **true si** l’agent est activé ; Sinon, la valeur est **false**. Cet attribut est obligatoire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Contient un **élément agent** pour chaque agent installé.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments de fichier de configuration des agents Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

