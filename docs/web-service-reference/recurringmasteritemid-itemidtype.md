---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: L’élément RecurringMasterItemId (ItemIdType) identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829010"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="097df-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="097df-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="097df-104">L’élément **RecurringMasterItemId (ItemIdType)** identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.</span><span class="sxs-lookup"><span data-stu-id="097df-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="097df-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="097df-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="097df-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="097df-106">Attributes and elements</span></span>

<span data-ttu-id="097df-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="097df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="097df-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="097df-108">Attributes</span></span>

****

|<span data-ttu-id="097df-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="097df-109">**Attribute**</span></span>|<span data-ttu-id="097df-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="097df-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="097df-111">ID</span><span class="sxs-lookup"><span data-stu-id="097df-111">Id</span></span>  <br/> |<span data-ttu-id="097df-112">Identifie une seule occurrence d’un rendez-vous périodique.</span><span class="sxs-lookup"><span data-stu-id="097df-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="097df-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="097df-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="097df-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="097df-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="097df-115">Identifie une version spécifique d’une seule occurrence d’un rendez-vous périodique.</span><span class="sxs-lookup"><span data-stu-id="097df-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="097df-116">En outre, le rendez-vous périodique est également identifié, car elle et l’occurrence contiendra la même clé change.</span><span class="sxs-lookup"><span data-stu-id="097df-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="097df-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="097df-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="097df-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="097df-118">Child elements</span></span>

<span data-ttu-id="097df-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="097df-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="097df-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="097df-120">Parent elements</span></span>

[<span data-ttu-id="097df-121">Rappel</span><span class="sxs-lookup"><span data-stu-id="097df-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="097df-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="097df-122">Remarks</span></span>

<span data-ttu-id="097df-123">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="097df-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="097df-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="097df-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="097df-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="097df-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="097df-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="097df-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="097df-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="097df-127">Schema Name</span></span>  <br/> |<span data-ttu-id="097df-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="097df-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="097df-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="097df-129">Validation File</span></span>  <br/> |<span data-ttu-id="097df-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="097df-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="097df-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="097df-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="097df-132">True</span><span class="sxs-lookup"><span data-stu-id="097df-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="097df-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="097df-133">See also</span></span>



[<span data-ttu-id="097df-134">Rappel</span><span class="sxs-lookup"><span data-stu-id="097df-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="097df-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="097df-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

