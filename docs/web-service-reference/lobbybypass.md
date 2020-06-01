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
# <a name="lobbybypass"></a><span data-ttu-id="7b795-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="7b795-103">LobbyBypass</span></span>

<span data-ttu-id="7b795-104">L’élément **LobbyBypass** spécifie le paramètre de réunion en ligne pour contourner la salle d’attente virtuelle.</span><span class="sxs-lookup"><span data-stu-id="7b795-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="7b795-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="7b795-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b795-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b795-106">Attributes and elements</span></span>

<span data-ttu-id="7b795-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b795-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b795-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b795-108">Attributes</span></span>

<span data-ttu-id="7b795-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b795-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b795-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b795-110">Child elements</span></span>

<span data-ttu-id="7b795-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b795-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b795-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b795-112">Parent elements</span></span>

[<span data-ttu-id="7b795-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="7b795-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="7b795-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7b795-114">Text value</span></span>

<span data-ttu-id="7b795-115">La valeur de texte de l’élément **LobbyBypass** peut être **désactivée** ou **EnabledForGatewayParticipants**.</span><span class="sxs-lookup"><span data-stu-id="7b795-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="7b795-116">La valeur **Disabled** indique que le contournement de la salle d’attente est désactivé afin que tous les participants à la réunion doivent accéder à la salle d’attente virtuelle.</span><span class="sxs-lookup"><span data-stu-id="7b795-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="7b795-117">La valeur **EnabledForGatewayParticipants** indique que le contournement de la salle d’attente est activé pour les participants téléphoniques.</span><span class="sxs-lookup"><span data-stu-id="7b795-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7b795-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b795-118">Remarks</span></span>

<span data-ttu-id="7b795-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7b795-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b795-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b795-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

