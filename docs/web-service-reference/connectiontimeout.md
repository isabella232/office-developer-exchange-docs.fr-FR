---
title: ConnectionTimeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: L’élément ConnectionTimeout Spécifie le nombre de minutes à conserver une connexion ouverte.
ms.openlocfilehash: 2bb40ba502853c70ef107c4c740fdfe7073abe31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755543"
---
# <a name="connectiontimeout"></a><span data-ttu-id="7da0a-103">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="7da0a-103">ConnectionTimeout</span></span>

<span data-ttu-id="7da0a-104">L’élément **ConnectionTimeout** Spécifie le nombre de minutes à conserver une connexion ouverte.</span><span class="sxs-lookup"><span data-stu-id="7da0a-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="7da0a-105">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="7da0a-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="7da0a-106">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="7da0a-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="7da0a-107">**int**</span><span class="sxs-lookup"><span data-stu-id="7da0a-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7da0a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7da0a-108">Attributes and elements</span></span>

<span data-ttu-id="7da0a-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7da0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da0a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7da0a-110">Attributes</span></span>

<span data-ttu-id="7da0a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7da0a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7da0a-112">Child elements</span></span>

<span data-ttu-id="7da0a-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da0a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7da0a-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7da0a-114">Parent elements</span></span>

|<span data-ttu-id="7da0a-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7da0a-115">**Element**</span></span>|<span data-ttu-id="7da0a-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da0a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da0a-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="7da0a-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="7da0a-118">Définit une demande pour obtenir des notifications d’événement à partir d’une connexion de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="7da0a-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7da0a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7da0a-119">Text value</span></span>

<span data-ttu-id="7da0a-120">La valeur de texte représente un entier qui décrit le nombre maximal de minutes pour maintenir une connexion de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="7da0a-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="7da0a-121">La valeur doit être comprise entre 1 et 30 inclus.</span><span class="sxs-lookup"><span data-stu-id="7da0a-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7da0a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7da0a-122">Remarks</span></span>

<span data-ttu-id="7da0a-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7da0a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7da0a-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7da0a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7da0a-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7da0a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7da0a-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7da0a-126">Schema name</span></span>  <br/> |<span data-ttu-id="7da0a-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7da0a-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7da0a-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7da0a-128">Validation file</span></span>  <br/> |<span data-ttu-id="7da0a-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7da0a-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7da0a-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7da0a-130">Can be empty</span></span>  <br/> |<span data-ttu-id="7da0a-131">False</span><span class="sxs-lookup"><span data-stu-id="7da0a-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7da0a-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7da0a-132">See also</span></span>



[<span data-ttu-id="7da0a-133">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="7da0a-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="7da0a-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7da0a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

