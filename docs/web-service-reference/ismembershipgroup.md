---
title: IsMembershipGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0dc3e285-8f49-48ad-b844-37041c0d782b
description: L’élément IsMembershipGroup spécifie une valeur Boolean qui indique si l’entité est un groupe de distribution ou une boîte aux lettres.
ms.openlocfilehash: 111a517a5258a48aada1c7768c908d62f3a47b9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540978"
---
# <a name="ismembershipgroup"></a>IsMembershipGroup

**L’élément IsMembershipGroup spécifie** une valeur Boolean qui indique si l’entité est un groupe de distribution ou une boîte aux lettres. 
  
```XML
<IsMembershipGroup>true | false</IsMembershipGroup>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SearchableMailbox](searchablemailbox.md) <br/> |Spécifie une boîte aux lettres renvoyée par une **demande GetSearchableMailboxes.**  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **IsMembershipGroup** indique que l’entité est un groupe de distribution ou une boîte aux lettres. La valeur false indique que l’entité n’est pas un groupe de distribution ou une boîte aux lettres. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

