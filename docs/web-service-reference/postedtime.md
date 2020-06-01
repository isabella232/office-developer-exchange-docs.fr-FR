---
title: PostedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostedTime
api_type:
- schema
ms.assetid: e8b3813c-fc7e-4674-a4c6-6818c13d2bcf
description: L’élément PostedTime représente l’heure à laquelle un PostItem a été publié. Cet élément est en lecture seule. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 5fc670bfee97a46700bc4442d489696a4489f88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459194"
---
# <a name="postedtime"></a><span data-ttu-id="d9e73-105">PostedTime</span><span class="sxs-lookup"><span data-stu-id="d9e73-105">PostedTime</span></span>

<span data-ttu-id="d9e73-106">L’élément **PostedTime** représente l’heure à laquelle un [PostItem](postitem.md) a été publié.</span><span class="sxs-lookup"><span data-stu-id="d9e73-106">The **PostedTime** element represents the time at which a [PostItem](postitem.md) was posted.</span></span> <span data-ttu-id="d9e73-107">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="d9e73-107">This element is read-only.</span></span> <span data-ttu-id="d9e73-108">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d9e73-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PostedTime/>
```

 <span data-ttu-id="d9e73-109">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d9e73-109">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9e73-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d9e73-110">Attributes and elements</span></span>

<span data-ttu-id="d9e73-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d9e73-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9e73-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d9e73-112">Attributes</span></span>

<span data-ttu-id="d9e73-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d9e73-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9e73-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d9e73-114">Child elements</span></span>

<span data-ttu-id="d9e73-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d9e73-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9e73-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d9e73-116">Parent elements</span></span>

|<span data-ttu-id="d9e73-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d9e73-117">**Element**</span></span>|<span data-ttu-id="d9e73-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d9e73-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e73-119">PostItem</span><span class="sxs-lookup"><span data-stu-id="d9e73-119">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="d9e73-120">Représente un PostItem dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e73-120">Represents a PostItem in the Exchange store.</span></span> <span data-ttu-id="d9e73-121">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d9e73-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9e73-122">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d9e73-122">Text value</span></span>

<span data-ttu-id="d9e73-123">La valeur de texte est un dateTime qui représente le moment où un **PostItem** a été publié.</span><span class="sxs-lookup"><span data-stu-id="d9e73-123">The text value is a dateTime that represents when a **PostItem** was posted.</span></span> <span data-ttu-id="d9e73-124">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="d9e73-124">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d9e73-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="d9e73-125">Remarks</span></span>

<span data-ttu-id="d9e73-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d9e73-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9e73-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d9e73-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9e73-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d9e73-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9e73-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d9e73-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d9e73-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d9e73-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9e73-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d9e73-131">Validation File</span></span>  <br/> |<span data-ttu-id="d9e73-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9e73-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9e73-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d9e73-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9e73-134">False</span><span class="sxs-lookup"><span data-stu-id="d9e73-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9e73-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d9e73-135">See also</span></span>



- [<span data-ttu-id="d9e73-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d9e73-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

