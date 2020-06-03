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
description: L’élément GroupIndex représente la valeur de propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments en cours dans un appel d’opération FindItem.
ms.openlocfilehash: 05f303be92885a15dddf85c85251af04910d835c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530267"
---
# <a name="groupindex"></a>GroupIndex

L’élément **GroupIndex** représente la valeur de propriété qui est utilisée pour regrouper des éléments pour le groupe d’éléments en cours dans un appel d' [opération FindItem](finditem-operation.md) . 
  
[FindItemResponse](finditemresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[FindItemResponseMessage](finditemresponsemessage.md)
  
[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
  
[Groups](groups.md)
  
[GroupedItems](groupeditems.md)
  
[GroupIndex](groupindex.md)
  
```xml
<GroupIndex/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments qui sont le résultat d’un appel d' [opération FindItem](finditem-operation.md) groupé.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Cette propriété est en lecture seule.
  
## <a name="remarks"></a>Remarques

Cet élément ne se produit que dans une réponse d' [opération FindItem](finditem-operation.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)


[Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

