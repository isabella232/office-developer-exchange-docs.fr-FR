---
title: PlayOnPhone (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: L’élément PlayOnPhone définit une demande de lecture d’un élément sur un téléphone.
ms.openlocfilehash: 240c8f474c87e0c123a6d8239eb691079385e348
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527988"
---
# <a name="playonphone-um-web-service"></a>PlayOnPhone (service web de messagerie unifiée)

**L’élément PlayOnPhone** définit une demande de lecture d’un élément sur un téléphone. 
  
[PlayOnPhone (service web de messagerie unifiée)](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[entryId (service web de messagerie unifiée)](entryid-um-web-service.md) <br/> |Contient la valeur qui représente l’identificateur de l’élément à lire sur le téléphone dans une demande [d’opération PlayOnPhone (service web de um).](playonphone-operation-um-web-service.md)  <br/> |
|[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md) <br/> |Contient la valeur du numéro de téléphone à composer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md)

