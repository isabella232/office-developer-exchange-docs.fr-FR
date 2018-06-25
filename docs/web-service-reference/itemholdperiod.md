---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: L’élément ItemHoldPeriod spécifie la quantité de temps pour bloquer le contenu qui correspond à la requête de la boîte aux lettres.
ms.openlocfilehash: 212d765aa3f0493dd4f3051de483fa08a6fa8ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828144"
---
# <a name="itemholdperiod"></a>ItemHoldPeriod

L’élément **ItemHoldPeriod** spécifie la quantité de temps pour bloquer le contenu qui correspond à la requête de la boîte aux lettres. 
  
```XML
<ItemHoldPeriod/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte peut être « Unlimited » ou la valeur de chaîne de n’importe quelle valeur [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) . 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[SetHoldOnMailboxes](setholdonmailboxes.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

