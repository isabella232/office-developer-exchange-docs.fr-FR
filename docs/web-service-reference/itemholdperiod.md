---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: L’élément ItemHoldPeriod spécifie la durée de la prise en main du contenu qui correspond à la requête de boîte aux lettres.
ms.openlocfilehash: de56c410c876917bbe8d545c9ef4f38ee6948b21
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522851"
---
# <a name="itemholdperiod"></a>ItemHoldPeriod

**L’élément ItemHoldPeriod** spécifie la durée de la prise en main du contenu qui correspond à la requête de boîte aux lettres. 
  
```XML
<ItemHoldPeriod/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte peut être « Unlimited » ou la valeur de chaîne de n’importe quelle [valeur Timespan.](https://msdn.microsoft.com/library/1ecy8h51%28v=vs.110%29.aspx) 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[SetHoldOnMailboxes](setholdonmailboxes.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

