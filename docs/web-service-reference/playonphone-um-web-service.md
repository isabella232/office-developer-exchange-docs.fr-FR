---
title: PlayOnPhone (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: L’élément PlayOnPhone définit une demande pour lire un élément sur un téléphone.
ms.openlocfilehash: 7e5c1e25512a59d1ac3295b476fcc2b6b0f5a2b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828825"
---
# <a name="playonphone-um-web-service"></a>PlayOnPhone (service web de messagerie unifiée)

L’élément **PlayOnPhone** définit une demande pour lire un élément sur un téléphone. 
  
[PlayOnPhone (service web de messagerie unifiée)](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[propriété entryId (service web de messagerie unifiée)](entryid-um-web-service.md) <br/> |Contient la valeur qui représente l’identificateur de l’élément à lire sur le téléphone dans une requête [d’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) .  <br/> |
|[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Contient la valeur du numéro de téléphone à composer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)

