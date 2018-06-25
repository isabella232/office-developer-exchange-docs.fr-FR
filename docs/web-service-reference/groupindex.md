---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: L’élément GroupIndex représente la valeur de la propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments dans un appel de l’opération FindItem actuel.
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827762"
---
# <a name="groupindex"></a>GroupIndex

L’élément **GroupIndex** représente la valeur de la propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments dans un appel [FindItem opération](finditem-operation.md) en cours. 
  
[FindItemResponse](finditemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[FindItemResponseMessage](finditemresponsemessage.md)
  
[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
  
[Groupes](groups.md)
  
[GroupedItems](groupeditems.md)
  
[GroupIndex](groupindex.md)
  
```xml
<GroupIndex/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments qui sont le résultat d’une [opération FindItem](finditem-operation.md) groupée appeler.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Cette propriété est en lecture seule.
  
## <a name="remarks"></a>Remarques

Cet élément ne se produit dans une réponse de [l’opération FindItem](finditem-operation.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)


[Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

