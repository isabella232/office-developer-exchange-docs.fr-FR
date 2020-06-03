---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: L’élément IncludeNonIndexableItems contient une valeur booléenne indiquant s’il faut inclure des éléments qui ne peuvent pas être indexés.
ms.openlocfilehash: eab559e938f0b949d79626ae5bf61b3d4a838924
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460623"
---
# <a name="includenonindexableitems"></a>IncludeNonIndexableItems

L’élément **IncludeNonIndexableItems** contient une valeur **booléenne** indiquant s’il faut inclure des éléments qui ne peuvent pas être indexés. 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **IncludeNonIndexableItems** indique que les éléments qui ne peuvent pas être indexés sont inclus dans les conservations des boîtes aux lettres. La valeur **false** indique que les éléments qui ne peuvent pas être indexés ne sont pas inclus dans les conservations des boîtes aux lettres. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

