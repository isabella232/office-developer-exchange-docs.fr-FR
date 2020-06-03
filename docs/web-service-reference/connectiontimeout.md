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
description: L’élément ConnectionTimeout spécifie le nombre de minutes pendant lesquelles la connexion doit rester ouverte.
ms.openlocfilehash: 671e3cf5466ee8b3543036811708bd7f54afdcce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463852"
---
# <a name="connectiontimeout"></a><span data-ttu-id="05967-103">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="05967-103">ConnectionTimeout</span></span>

<span data-ttu-id="05967-104">L’élément **ConnectionTimeout** spécifie le nombre de minutes pendant lesquelles la connexion doit rester ouverte.</span><span class="sxs-lookup"><span data-stu-id="05967-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="05967-105">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="05967-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="05967-106">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="05967-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="05967-107">**int**</span><span class="sxs-lookup"><span data-stu-id="05967-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05967-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05967-108">Attributes and elements</span></span>

<span data-ttu-id="05967-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05967-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05967-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="05967-110">Attributes</span></span>

<span data-ttu-id="05967-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="05967-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05967-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05967-112">Child elements</span></span>

<span data-ttu-id="05967-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05967-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05967-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05967-114">Parent elements</span></span>

|<span data-ttu-id="05967-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05967-115">**Element**</span></span>|<span data-ttu-id="05967-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="05967-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05967-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="05967-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="05967-118">Définit une demande pour obtenir des notifications d’événement à partir d’une connexion de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="05967-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05967-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="05967-119">Text value</span></span>

<span data-ttu-id="05967-120">La valeur texte représente un entier qui décrit le nombre maximal de minutes pendant lesquelles une connexion de diffusion en continu doit être conservée.</span><span class="sxs-lookup"><span data-stu-id="05967-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="05967-121">La valeur doit être comprise entre 1 et 30 inclus.</span><span class="sxs-lookup"><span data-stu-id="05967-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05967-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="05967-122">Remarks</span></span>

<span data-ttu-id="05967-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="05967-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05967-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05967-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05967-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05967-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05967-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05967-126">Schema name</span></span>  <br/> |<span data-ttu-id="05967-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05967-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="05967-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05967-128">Validation file</span></span>  <br/> |<span data-ttu-id="05967-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05967-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05967-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05967-130">Can be empty</span></span>  <br/> |<span data-ttu-id="05967-131">False</span><span class="sxs-lookup"><span data-stu-id="05967-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05967-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05967-132">See also</span></span>



[<span data-ttu-id="05967-133">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="05967-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="05967-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05967-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

