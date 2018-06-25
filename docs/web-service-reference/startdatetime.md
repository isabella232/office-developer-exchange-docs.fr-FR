---
title: StartDateTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDateTime
api_type:
- schema
ms.assetid: 6fd41b7b-6c83-43b6-8b16-0bdb3d173d73
description: L’élément StartDateTime spécifie la date de début et l’heure pour une règle ou d’une recherche.
ms.openlocfilehash: 4bc32ed5626d692fc73dfa8bd7c46923aba72f9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829552"
---
# <a name="startdatetime"></a><span data-ttu-id="7d548-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="7d548-103">StartDateTime</span></span>

<span data-ttu-id="7d548-104">L’élément **StartDateTime** spécifie la date de début et l’heure pour une règle ou d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="7d548-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="7d548-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="7d548-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7d548-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d548-106">Attributes and elements</span></span>

<span data-ttu-id="7d548-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d548-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d548-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d548-108">Attributes</span></span>

<span data-ttu-id="7d548-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d548-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d548-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d548-110">Child elements</span></span>

<span data-ttu-id="7d548-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d548-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d548-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d548-112">Parent elements</span></span>

|<span data-ttu-id="7d548-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d548-113">**Element**</span></span>|<span data-ttu-id="7d548-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d548-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d548-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7d548-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7d548-116">Spécifie les critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="7d548-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="7d548-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="7d548-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="7d548-118">Spécifie la plage de dates dans laquelle les messages entrants ont reçue dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="7d548-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d548-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7d548-119">Text value</span></span>

 <span data-ttu-id="7d548-120">Une valeur de texte qui représente une date/heure est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7d548-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7d548-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d548-121">Remarks</span></span>

<span data-ttu-id="7d548-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d548-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d548-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7d548-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d548-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7d548-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d548-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7d548-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7d548-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7d548-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d548-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7d548-127">Validation File</span></span>  <br/> |<span data-ttu-id="7d548-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7d548-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d548-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7d548-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d548-130">False</span><span class="sxs-lookup"><span data-stu-id="7d548-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d548-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d548-131">See also</span></span>

- [<span data-ttu-id="7d548-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d548-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

