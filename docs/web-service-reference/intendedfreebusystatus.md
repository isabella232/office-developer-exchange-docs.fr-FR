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
description: L’élément IntendedFreeBusyStatus représente l’État prévu pour l’élément de calendrier qui est associé à la demande de réunion.
ms.openlocfilehash: c5502bcfb308aa2f02a9575ab43f80261b5fa4ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465617"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="7b647-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="7b647-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="7b647-104">L’élément **IntendedFreeBusyStatus** représente l’État prévu pour l’élément de calendrier qui est associé à la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="7b647-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="7b647-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="7b647-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b647-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b647-106">Attributes and elements</span></span>

<span data-ttu-id="7b647-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b647-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b647-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b647-108">Attributes</span></span>

<span data-ttu-id="7b647-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b647-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b647-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b647-110">Child elements</span></span>

<span data-ttu-id="7b647-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b647-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b647-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b647-112">Parent elements</span></span>

|<span data-ttu-id="7b647-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b647-113">**Element**</span></span>|<span data-ttu-id="7b647-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b647-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b647-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="7b647-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7b647-116">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b647-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b647-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7b647-117">Text value</span></span>

<span data-ttu-id="7b647-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="7b647-118">A text value is required.</span></span> <span data-ttu-id="7b647-119">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7b647-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="7b647-120">Gratuit</span><span class="sxs-lookup"><span data-stu-id="7b647-120">Free</span></span>
    
- <span data-ttu-id="7b647-121">Provisoire</span><span class="sxs-lookup"><span data-stu-id="7b647-121">Tentative</span></span>
    
- <span data-ttu-id="7b647-122">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="7b647-122">Busy</span></span>
    
- <span data-ttu-id="7b647-123">Bureau</span><span class="sxs-lookup"><span data-stu-id="7b647-123">OOF</span></span>
    
- <span data-ttu-id="7b647-124">NoData</span><span class="sxs-lookup"><span data-stu-id="7b647-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7b647-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b647-125">Remarks</span></span>

<span data-ttu-id="7b647-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7b647-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b647-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b647-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b647-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b647-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b647-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b647-129">Schema Name</span></span>  <br/> |<span data-ttu-id="7b647-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7b647-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b647-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b647-131">Validation File</span></span>  <br/> |<span data-ttu-id="7b647-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b647-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b647-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b647-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b647-134">False</span><span class="sxs-lookup"><span data-stu-id="7b647-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b647-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b647-135">See also</span></span>



- [<span data-ttu-id="7b647-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b647-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

