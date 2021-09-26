---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: L’élément ImItemList contient une liste de groupes de messagerie instantanée et de contacts de messagerie instantanée.
ms.openlocfilehash: fdd2865ceb1553a7f75d7059b08ea96ce89aa096
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547245"
---
# <a name="imitemlist"></a>ImItemList

**L’élément ImItemList** contient une liste de groupes de messagerie instantanée et de contacts de messagerie instantanée. 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 **ImItemListType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  |  [Personas](personas-ex15websvcsotherref.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetImItemsResponse](getimitemsresponse.md)  |  [GetImItemListResponse](getimitemlistresponse.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

