---
title: Flag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: L’élément Flag spécifie un indicateur sur un élément de boîte aux lettres.
ms.openlocfilehash: dffc550dc4235c2121b6641f3a6eac30594f75b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513695"
---
# <a name="flag"></a>Flag

**L’élément Flag** spécifie un indicateur sur un élément de boîte aux lettres. 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 **FlagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FlagStatus](flagstatus.md) <br/> |Contient l’état de l’indicateur agrégé pour les éléments du dossier actuel.  <br/> |
|[StartDate](startdate.md) <br/> |Représente la date de début d’un élément.  <br/> |
|[DueDate](duedate.md) <br/> |Représente la date d’échéance d’un élément.  <br/> |
|[CompleteDate](completedate.md) <br/> |Représente la date à laquelle un élément a été terminé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contient une seule action à appliquer à une seule conversation.  <br/> |
|[Élément](item.md) <br/> |Représente un élément générique dans le magasin Exchange de données.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

