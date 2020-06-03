---
title: /M
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: L’élément MaximumSize représente la taille maximale qu’un message doit être pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 250e0c6aed37b934f5cf6eaed9d93b9f56159d93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461750"
---
# <a name="maximumsize"></a>/M

L’élément **MaximumSize** représente la taille maximale qu’un message doit être pour que la condition ou l’exception s’applique. 
  
```XML
<Maximum/>
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
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est un entier qui identifie la taille maximale du message en octets.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[MinimumSize](minimumsize.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

