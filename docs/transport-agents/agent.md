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
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455680"
---
# <a name="agent"></a>agent
  
**S’applique à :** Exchange Server 2013
  
L’élément **agent** contient des informations de configuration sur un agent installé. 
  
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
|**nom** <br/> |Nom qui a été spécifié lors de l’installation de l’agent. Cet attribut requiert une valeur de chaîne non vide contenant un maximum de 64 caractères.  <br/> |
|**baseType** <br/> |Nom complet, y compris l’espace de noms, de la classe à partir de laquelle l’agent dérive. Cet attribut requiert une valeur de chaîne non vide contenant au moins un caractère.  <br/> |
|**classFactory** <br/> |Nom complet, y compris l’espace de noms, de la classe qui implémente la fabrique d’agent qui crée des instances de l’agent. Cet attribut doit contenir le nom complet de la classe qui implémente la fabrique d’agent qui crée des instances de l’agent. Cette classe doit dériver de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**assemblyPath** <br/> |Chemin d’accès complet, y compris le nom de fichier, de l’assembly qui contient le code de l’agent. Cet attribut requiert une valeur de chaîne non vide contenant au moins un caractère.  <br/> |
|**enabled** <br/> |Valeur booléenne qui indique si l’agent est activé. La valeur est **true** si l’agent est activé ; Sinon, la valeur est **false**. Cet attribut est obligatoire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Contient un élément **agent** pour chaque agent installé.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |Ce fichier ne définit pas d’espace de noms.  <br/> |
|Nom du schéma  <br/> |Non disponible.  <br/> |
|Fichier de validation  <br/> |Non disponible.  <br/> |
|Peut être vide  <br/> |Faux.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier de configuration des agents pour Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

