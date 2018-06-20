---
title: agent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755112"
---
# <a name="agent"></a>agent
  
**S’applique à :** Exchange Server 2013
  
L’élément de **l’agent** contient des informations de configuration sur un agent installé. 
  
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

**type_agent (type complexe)**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**nom** <br/> |Le nom spécifié lors de l’agent a été installé. Cet attribut requiert une valeur de chaîne non vide qui contient un maximum de 64 caractères.  <br/> |
|**baseType** <br/> |Le nom complet, y compris l’espace de noms de la classe qui dérive de l’agent. Cet attribut requiert une valeur de chaîne non vide qui contient au moins un caractère.  <br/> |
|**classFactory** <br/> |Le nom complet, y compris l’espace de noms de la classe qui implémente la fabrique de l’agent qui crée des instances de l’agent. Cet attribut doit contenir le nom qualifié complet de la classe qui implémente la fabrique de l’agent qui crée des instances de l’agent. Cette classe doit dériver de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou de [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**assemblyPath** <br/> |Chemin d’accès complet, y compris le nom de fichier de l’assembly qui contient le code pour l’agent. Cet attribut requiert une valeur de chaîne non vide qui contient au moins un caractère.  <br/> |
|**activé** <br/> |Une valeur de type Boolean qui indique si l’agent est activé. La valeur est **true** si l’agent est activé ; dans le cas contraire, la valeur est **false**. Cet attribut est requis.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Contient un élément de **l’agent** pour chaque agent installé.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas un espace de noms.  <br/> |
|Nom du schéma  <br/> |N’est pas disponible.  <br/> |
|Fichier de validation  <br/> |N’est pas disponible.  <br/> |
|Peut être vide  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

