---
title: Groupes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: L’élément groupes contient une collection des groupes qui sont trouvés dans les critères de recherche et d’agrégation identifiée dans la requête d’opération FindItem.
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827786"
---
# <a name="groups"></a>Groupes

L’élément **groupes** contient une collection des groupes qui sont trouvés dans les critères de recherche et d’agrégation identifiée dans la requête [d’opération FindItem](finditem-operation.md) . 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 **ArrayOfGroupedItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments qui sont le résultat d’une [opération FindItem](finditem-operation.md) groupée appeler.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contient les résultats de la recherche d’un dossier racine unique pendant une [opération FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Une seule instance [GroupedItems](groupeditems.md) se produit pour chaque groupe distinct dans le résultat. 
  
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

