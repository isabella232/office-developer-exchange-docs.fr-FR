---
title: Groupes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: L’élément Groups contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d’opération FindItem.
ms.openlocfilehash: f47ab4111137d2e5d98fcc6dcf40fadc073b7af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539681"
---
# <a name="groups"></a>Groupes

**L’élément Groups** contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d’opération [FindItem.](finditem-operation.md) 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 **ArrayOfGroupedItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments résultant d’un appel d’opération [FindItem groupé.](finditem-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contient les résultats d’une recherche d’un dossier racine unique au cours d’une [opération FindItem.](finditem-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Une [instance GroupedItems se](groupeditems.md) produit pour chaque groupe distinct dans le résultat. 
  
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

