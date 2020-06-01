---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: L’élément UpdatedItemIds spécifie les identificateurs des éléments de rappel mis à jour.
ms.openlocfilehash: 4a87bf50f90e80c0c887ee3a66b9f201ea1c8440
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465035"
---
# <a name="updateditemids"></a>UpdatedItemIds

L’élément **UpdatedItemIds** spécifie les identificateurs des éléments de rappel mis à jour. 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 **NonEmptyArrayOfItemIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemid.md)
  
### <a name="parent-elements"></a>Éléments parents

[PerformReminderActionResponse](performreminderactionresponse.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Si l’opération [PerformReminderAction](performreminderaction-operation.md) ne s’est pas terminée correctement ou qu’aucune modification n’a été apportée sur le serveur, l’élément **UpdatedItemIds** est renvoyé sous la forme d’une valeur vide. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[PerformReminderActionResponse](performreminderactionresponse.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

