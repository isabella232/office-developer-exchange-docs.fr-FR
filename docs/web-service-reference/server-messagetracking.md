---
title: Serveur (MessageTracking)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Server
api_type:
- schema
ms.assetid: eb5408bd-6fa5-4415-9224-24d5e07ec5b3
description: L’élément serveur représente le serveur physique où l’événement s’est produite.
ms.openlocfilehash: 95117eb2b5d195bc8b7ff90098e4138b67722f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829372"
---
# <a name="server-messagetracking"></a><span data-ttu-id="7dc62-103">Serveur (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="7dc62-103">Server (MessageTracking)</span></span>

<span data-ttu-id="7dc62-104">L’élément **serveur** représente le serveur physique où l’événement s’est produite.</span><span class="sxs-lookup"><span data-stu-id="7dc62-104">The **Server** element represents the physical server where the event occurred.</span></span> 
  
```XML
<Server/>
```

 <span data-ttu-id="7dc62-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="7dc62-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dc62-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7dc62-106">Attributes and elements</span></span>

<span data-ttu-id="7dc62-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7dc62-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dc62-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7dc62-108">Attributes</span></span>

<span data-ttu-id="7dc62-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7dc62-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7dc62-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7dc62-110">Child elements</span></span>

<span data-ttu-id="7dc62-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7dc62-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7dc62-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7dc62-112">Parent elements</span></span>

|<span data-ttu-id="7dc62-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7dc62-113">**Element**</span></span>|<span data-ttu-id="7dc62-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dc62-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dc62-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="7dc62-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="7dc62-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="7dc62-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7dc62-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7dc62-117">Text value</span></span>

<span data-ttu-id="7dc62-118">Une valeur de texte qui représente une chaîne est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7dc62-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7dc62-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="7dc62-119">Remarks</span></span>

<span data-ttu-id="7dc62-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dc62-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dc62-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7dc62-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dc62-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7dc62-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7dc62-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7dc62-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7dc62-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7dc62-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="7dc62-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7dc62-125">Validation File</span></span>  <br/> |<span data-ttu-id="7dc62-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7dc62-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7dc62-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7dc62-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dc62-128">False</span><span class="sxs-lookup"><span data-stu-id="7dc62-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dc62-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7dc62-129">See also</span></span>



- [<span data-ttu-id="7dc62-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7dc62-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

