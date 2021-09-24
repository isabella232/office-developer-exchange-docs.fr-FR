---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: L’élément LobbyBypass spécifie le paramètre de réunion en ligne pour contourner la salle d’attente virtuelle.
ms.openlocfilehash: 41ab9c3f846112d2b679bbb477a0de355a477ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540782"
---
# <a name="lobbybypass"></a>LobbyBypass

**L’élément LobbyBypass spécifie** le paramètre de réunion en ligne pour contourner la salle d’attente virtuelle. 
  
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

La valeur de texte de **l’élément LobbyBypass** peut être **Disabled** ou **EnabledForGatewayParticipants**. La **valeur Disabled** indique que le contournement de la salle d’accès est désactivé afin que tous les participants à la réunion doivent accéder via la salle d’accueil virtuelle. La **valeur EnabledForGatewayParticipants** indique que le contournement de la salle d’écoute est activé pour les participants au téléphone. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

