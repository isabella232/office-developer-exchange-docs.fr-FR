---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: L’élément MinimumSize représente la taille minimale d’un message pour que la condition ou l’exception s’applique.
ms.openlocfilehash: c3f1284a5a82731093863b0a621bcf2f7f55cf22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540649"
---
# <a name="minimumsize"></a>MinimumSize

**L’élément MinimumSize** représente la taille minimale d’un message pour que la condition ou l’exception s’applique. 
  
```XML
<MinimumSize/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie la taille minimale et maximale des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est un nombre complet qui identifie la taille minimale du message en octets.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[MaximumSize](maximumsize.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

