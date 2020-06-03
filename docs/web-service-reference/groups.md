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
description: L’élément Groups contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d’opération FindItem.
ms.openlocfilehash: 915d9dffd6d8cec1def6634e6b70642d563b5242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530788"
---
# <a name="groups"></a>Groupes

L’élément **groups** contient une collection de groupes trouvés avec les critères de recherche et d’agrégation identifiés dans la demande d' [opération FindItem](finditem-operation.md) . 
  
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
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments qui sont le résultat d’un appel d' [opération FindItem](finditem-operation.md) groupé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contient les résultats d’une recherche d’un dossier racine unique pendant une opération d' [opération FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Une instance [GroupedItems](groupeditems.md) se produira pour chaque groupe distinct dans le résultat. 
  
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

