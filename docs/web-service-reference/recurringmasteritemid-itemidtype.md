---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: L’élément RecurringMasterItemId (ItemIdType) identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.
ms.openlocfilehash: c725998ad3a728ef1f47ff6491592b461753b895
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468438"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="6dcca-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="6dcca-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="6dcca-104">L’élément **RecurringMasterItemId (ItemIdType)** identifie un élément de la forme de base de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.</span><span class="sxs-lookup"><span data-stu-id="6dcca-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="6dcca-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="6dcca-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dcca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6dcca-106">Attributes and elements</span></span>

<span data-ttu-id="6dcca-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6dcca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dcca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6dcca-108">Attributes</span></span>

****

|<span data-ttu-id="6dcca-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6dcca-109">**Attribute**</span></span>|<span data-ttu-id="6dcca-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6dcca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6dcca-111">ID</span><span class="sxs-lookup"><span data-stu-id="6dcca-111">Id</span></span>  <br/> |<span data-ttu-id="6dcca-112">Identifie une seule occurrence d’un élément maître périodique.</span><span class="sxs-lookup"><span data-stu-id="6dcca-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6dcca-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="6dcca-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6dcca-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6dcca-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6dcca-115">Identifie une version spécifique d’une occurrence d’un élément maître périodique.</span><span class="sxs-lookup"><span data-stu-id="6dcca-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6dcca-116">En outre, l’élément de gabarit périodique est également identifié, car il et la seule occurrence contiendront la même clé de modification.</span><span class="sxs-lookup"><span data-stu-id="6dcca-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="6dcca-117">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="6dcca-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6dcca-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6dcca-118">Child elements</span></span>

<span data-ttu-id="6dcca-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6dcca-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6dcca-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6dcca-120">Parent elements</span></span>

[<span data-ttu-id="6dcca-121">Reminder</span><span class="sxs-lookup"><span data-stu-id="6dcca-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="6dcca-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="6dcca-122">Remarks</span></span>

<span data-ttu-id="6dcca-123">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6dcca-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6dcca-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dcca-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dcca-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6dcca-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dcca-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6dcca-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6dcca-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6dcca-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6dcca-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6dcca-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6dcca-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6dcca-129">Validation File</span></span>  <br/> |<span data-ttu-id="6dcca-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6dcca-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6dcca-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6dcca-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6dcca-132">True</span><span class="sxs-lookup"><span data-stu-id="6dcca-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6dcca-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6dcca-133">See also</span></span>



[<span data-ttu-id="6dcca-134">Reminder</span><span class="sxs-lookup"><span data-stu-id="6dcca-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="6dcca-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6dcca-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

