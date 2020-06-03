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
description: L’élément StartDateTime spécifie la date et l’heure de début d’une règle ou d’une recherche.
ms.openlocfilehash: 28b78fad87abb1148cfe49fee4f9bb98f822eae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462842"
---
# <a name="startdatetime"></a><span data-ttu-id="24ed8-103">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="24ed8-103">StartDateTime</span></span>

<span data-ttu-id="24ed8-104">L’élément **StartDateTime** spécifie la date et l’heure de début d’une règle ou d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="24ed8-104">The **StartDateTime** element specifies the start date and time for a rule or a search.</span></span> 
  
```XML
<StartDate/>
```

<span data-ttu-id="24ed8-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="24ed8-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="24ed8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24ed8-106">Attributes and elements</span></span>

<span data-ttu-id="24ed8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24ed8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24ed8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="24ed8-108">Attributes</span></span>

<span data-ttu-id="24ed8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="24ed8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24ed8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24ed8-110">Child elements</span></span>

<span data-ttu-id="24ed8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="24ed8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24ed8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24ed8-112">Parent elements</span></span>

|<span data-ttu-id="24ed8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24ed8-113">**Element**</span></span>|<span data-ttu-id="24ed8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="24ed8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24ed8-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="24ed8-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="24ed8-116">Spécifie les critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="24ed8-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="24ed8-117">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="24ed8-117">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="24ed8-118">Spécifie la plage de dates au cours de laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="24ed8-118">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24ed8-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="24ed8-119">Text value</span></span>

 <span data-ttu-id="24ed8-120">Une valeur de texte qui représente une date/heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="24ed8-120">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="24ed8-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="24ed8-121">Remarks</span></span>

<span data-ttu-id="24ed8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="24ed8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24ed8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24ed8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24ed8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24ed8-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24ed8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24ed8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="24ed8-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="24ed8-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="24ed8-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24ed8-127">Validation File</span></span>  <br/> |<span data-ttu-id="24ed8-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24ed8-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24ed8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24ed8-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="24ed8-130">False</span><span class="sxs-lookup"><span data-stu-id="24ed8-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24ed8-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24ed8-131">See also</span></span>

- [<span data-ttu-id="24ed8-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="24ed8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

