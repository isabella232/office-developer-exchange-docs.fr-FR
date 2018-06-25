---
title: IntendedFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IntendedFreeBusyStatus
api_type:
- schema
ms.assetid: 0e0fa898-69a4-4c57-8bb2-52f716b5b478
description: L’élément IntendedFreeBusyStatus représente l’état souhaité pour l’élément de calendrier qui est associé à la demande de réunion.
ms.openlocfilehash: 3254becf8c6885f7d6dc401ecf31da149e7de2d4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827945"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="73c77-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="73c77-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="73c77-104">L’élément **IntendedFreeBusyStatus** représente l’état souhaité pour l’élément de calendrier qui est associé à la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="73c77-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="73c77-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="73c77-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73c77-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="73c77-106">Attributes and elements</span></span>

<span data-ttu-id="73c77-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="73c77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73c77-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="73c77-108">Attributes</span></span>

<span data-ttu-id="73c77-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73c77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73c77-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="73c77-110">Child elements</span></span>

<span data-ttu-id="73c77-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73c77-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73c77-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="73c77-112">Parent elements</span></span>

|<span data-ttu-id="73c77-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73c77-113">**Element**</span></span>|<span data-ttu-id="73c77-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="73c77-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73c77-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="73c77-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="73c77-116">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="73c77-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73c77-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="73c77-117">Text value</span></span>

<span data-ttu-id="73c77-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="73c77-118">A text value is required.</span></span> <span data-ttu-id="73c77-119">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="73c77-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="73c77-120">Gratuit</span><span class="sxs-lookup"><span data-stu-id="73c77-120">Free</span></span>
    
- <span data-ttu-id="73c77-121">Provisoire</span><span class="sxs-lookup"><span data-stu-id="73c77-121">Tentative</span></span>
    
- <span data-ttu-id="73c77-122">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="73c77-122">Busy</span></span>
    
- <span data-ttu-id="73c77-123">ABSENCE DU BUREAU</span><span class="sxs-lookup"><span data-stu-id="73c77-123">OOF</span></span>
    
- <span data-ttu-id="73c77-124">NoData</span><span class="sxs-lookup"><span data-stu-id="73c77-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="73c77-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="73c77-125">Remarks</span></span>

<span data-ttu-id="73c77-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="73c77-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73c77-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="73c77-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73c77-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="73c77-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73c77-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="73c77-129">Schema Name</span></span>  <br/> |<span data-ttu-id="73c77-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="73c77-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="73c77-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="73c77-131">Validation File</span></span>  <br/> |<span data-ttu-id="73c77-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73c77-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73c77-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="73c77-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="73c77-134">False</span><span class="sxs-lookup"><span data-stu-id="73c77-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73c77-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="73c77-135">See also</span></span>



- [<span data-ttu-id="73c77-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="73c77-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

