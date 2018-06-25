---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: L’élément ExpandGroupMembership indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: 11bfcf6893a147c726c94df77f7d9a9dfbaa773e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756259"
---
# <a name="expandgroupmembership"></a>ExpandGroupMembership

L’élément **ExpandGroupMembership** indique s’il faut développer l’appartenance au groupe renvoyé à partir d’une demande **GetSearchableMailboxes** . 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **ExpandGroupElement** indique que l’appartenance au groupe est développé. La valeur **false** indique que l’appartenance au groupe n’est pas développé pour afficher les membres du groupe. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

