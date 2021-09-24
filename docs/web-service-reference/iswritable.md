---
title: IsWritable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d4af8eee-7001-4a8e-b9bd-d14882f2406b
description: L’élément IsWritable spécifie si le contact sous-jacent ou le destinataire Active Directory peut être écrit.
ms.openlocfilehash: 2663e18f2589516f304930b86a717455b6ab77c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516712"
---
# <a name="iswritable"></a>IsWritable

**L’élément IsWritable** spécifie si le contact sous-jacent ou le destinataire Active Directory peut être écrit. 
  
```XML
<IsWritable> true | false </IsWritable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **IsWritable** indique que le contact ou l’objet Active Directory est disponible pour un accès en écriture. La valeur **false indique** que le contact ou l’objet Active Directory n’est pas disponible pour l’accès en écriture. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

