---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: L’élément ConflictResults contient le nombre de conflits dans une réponse d’opération UpdateItem.
ms.openlocfilehash: 44b9c6952905274128c3651999b97cb2ee0c1fe8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519939"
---
# <a name="conflictresults"></a>ConflictResults

[L’élément ConflictResults](conflictresults.md) contient le nombre de conflits dans une réponse d’opération [UpdateItem.](updateitem-operation.md) 
  
[UpdateItemResponse](updateitemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[UpdateItemResponseMessage](updateitemresponsemessage.md)
  
[ConflictResults](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 **ConflictResultsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Count](count.md) <br/> |Contient le nombre de conflits dans une réponse [d’opération UpdateItem.](updateitem-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération UpdateItem](updateitem-operation.md) unique.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération UpdateItem](updateitem-operation.md)
  
 **ConflictResultsType**

