---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: L’élément LobbyBypass spécifie la réunion en ligne à la salle d’attente virtuelle.
ms.openlocfilehash: 9ecc920acd9e1aea3476ad1194d6c7d0529b21c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828246"
---
# <a name="lobbybypass"></a>LobbyBypass

L’élément **LobbyBypass** spécifie la réunion en ligne à la salle d’attente virtuelle. 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **LobbyBypass** peut être **désactivé** ou **EnabledForGatewayParticipants**. La valeur **désactivé** indique que le contournement de la salle d’attente est désactivé pour tous les participants à la réunion doivent accéder par le biais de la salle d’attente virtuelle. La valeur **EnabledForGatewayParticipants** indique que le contournement de la salle d’attente est activé pour les participants de téléphone. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

