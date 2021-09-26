---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: L’élément GroupIndex représente la valeur de propriété utilisée pour grouper des éléments pour le groupe actuel d’éléments dans un appel d’opération FindItem.
ms.openlocfilehash: 5e6e2c36e64edec1647c844209d86ceece840b05
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547343"
---
# <a name="groupindex"></a>GroupIndex

**L’élément GroupIndex représente** la valeur de propriété utilisée pour grouper des éléments pour le groupe actuel d’éléments dans un appel d’opération [FindItem.](finditem-operation.md) 
  
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
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments résultant d’un appel d’opération [FindItem groupé.](finditem-operation.md)  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Cette propriété est en lecture seule.
  
## <a name="remarks"></a>Remarques

Cet élément se produit uniquement dans une [réponse d’opération FindItem.](finditem-operation.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
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

