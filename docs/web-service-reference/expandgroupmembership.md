---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: L’élément ExpandGroupMembership indique s’il faut développer l’appartenance au groupe renvoyé par une demande GetSearchableMailboxes.
ms.openlocfilehash: fb835f8f1fa9fb957c6b3bf3ddef80e68d9c049f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541398"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

**L’élément ExpandGroupMembership** indique s’il faut développer l’appartenance au groupe renvoyé par une **demande GetSearchableMailboxes.** 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  |  [GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** **l’élément ExpandGroupElement** indique que l’appartenance au groupe est étendue. La valeur **false indique** que l’appartenance au groupe n’est pas étendue pour afficher les membres du groupe. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

