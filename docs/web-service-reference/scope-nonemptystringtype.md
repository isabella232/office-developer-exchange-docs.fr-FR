---
title: Étendue (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: L’élément de portée Spécifie l’étendue du rapport de suivi des messages.
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829280"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="97974-103">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="97974-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="97974-104">L’élément de **portée** Spécifie l’étendue du rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="97974-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="97974-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="97974-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97974-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97974-106">Attributes and elements</span></span>

<span data-ttu-id="97974-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97974-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97974-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97974-108">Attributes</span></span>

<span data-ttu-id="97974-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97974-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97974-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97974-110">Child elements</span></span>

<span data-ttu-id="97974-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97974-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97974-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97974-112">Parent elements</span></span>

<span data-ttu-id="97974-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="97974-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="97974-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="97974-114">Text value</span></span>

<span data-ttu-id="97974-115">Le tableau suivant répertorie les valeurs possibles pour l’élément **d’étendue** .</span><span class="sxs-lookup"><span data-stu-id="97974-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="97974-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="97974-116">**Value**</span></span>|<span data-ttu-id="97974-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="97974-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97974-118">Organisation</span><span class="sxs-lookup"><span data-stu-id="97974-118">Organization</span></span>  <br/> |<span data-ttu-id="97974-119">Les étendues de suivi des messages s’étend sur une organisation.</span><span class="sxs-lookup"><span data-stu-id="97974-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="97974-120">Forêt</span><span class="sxs-lookup"><span data-stu-id="97974-120">Forest</span></span>  <br/> |<span data-ttu-id="97974-121">Les étendues de suivi des messages s’étend sur une forêt.</span><span class="sxs-lookup"><span data-stu-id="97974-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="97974-122">Site</span><span class="sxs-lookup"><span data-stu-id="97974-122">Site</span></span>  <br/> |<span data-ttu-id="97974-123">Les étendues de suivi des messages s’étend sur un site.</span><span class="sxs-lookup"><span data-stu-id="97974-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97974-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="97974-124">Remarks</span></span>

<span data-ttu-id="97974-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="97974-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97974-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97974-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97974-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97974-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97974-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97974-128">Schema Name</span></span>  <br/> |<span data-ttu-id="97974-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="97974-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97974-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="97974-130">Validation File</span></span>  <br/> |<span data-ttu-id="97974-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="97974-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97974-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97974-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="97974-133">False</span><span class="sxs-lookup"><span data-stu-id="97974-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97974-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97974-134">See also</span></span>



- [<span data-ttu-id="97974-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97974-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

