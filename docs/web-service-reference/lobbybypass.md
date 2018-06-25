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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828246"
---
# <a name="lobbybypass"></a><span data-ttu-id="d59f5-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="d59f5-103">LobbyBypass</span></span>

<span data-ttu-id="d59f5-104">L’élément **LobbyBypass** spécifie la réunion en ligne à la salle d’attente virtuelle.</span><span class="sxs-lookup"><span data-stu-id="d59f5-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="d59f5-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="d59f5-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d59f5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d59f5-106">Attributes and elements</span></span>

<span data-ttu-id="d59f5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d59f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d59f5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d59f5-108">Attributes</span></span>

<span data-ttu-id="d59f5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d59f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d59f5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d59f5-110">Child elements</span></span>

<span data-ttu-id="d59f5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d59f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d59f5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d59f5-112">Parent elements</span></span>

[<span data-ttu-id="d59f5-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="d59f5-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="d59f5-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d59f5-114">Text value</span></span>

<span data-ttu-id="d59f5-115">La valeur de texte de l’élément **LobbyBypass** peut être **désactivé** ou **EnabledForGatewayParticipants**.</span><span class="sxs-lookup"><span data-stu-id="d59f5-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="d59f5-116">La valeur **désactivé** indique que le contournement de la salle d’attente est désactivé pour tous les participants à la réunion doivent accéder par le biais de la salle d’attente virtuelle.</span><span class="sxs-lookup"><span data-stu-id="d59f5-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="d59f5-117">La valeur **EnabledForGatewayParticipants** indique que le contournement de la salle d’attente est activé pour les participants de téléphone.</span><span class="sxs-lookup"><span data-stu-id="d59f5-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d59f5-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="d59f5-118">Remarks</span></span>

<span data-ttu-id="d59f5-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d59f5-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d59f5-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d59f5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

