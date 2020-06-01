---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: L’élément LobbyBypass spécifie le paramètre de réunion en ligne pour contourner la salle d’attente virtuelle.
ms.openlocfilehash: 6940428c944b9d4d64acc6dbbf3993576e1932eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458095"
---
# <a name="lobbybypass"></a>LobbyBypass

L’élément **LobbyBypass** spécifie le paramètre de réunion en ligne pour contourner la salle d’attente virtuelle. 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **LobbyBypass** peut être **désactivée** ou **EnabledForGatewayParticipants**. La valeur **Disabled** indique que le contournement de la salle d’attente est désactivé afin que tous les participants à la réunion doivent accéder à la salle d’attente virtuelle. La valeur **EnabledForGatewayParticipants** indique que le contournement de la salle d’attente est activé pour les participants téléphoniques. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

