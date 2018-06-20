---
title: ContactSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactSource
api_type:
- schema
ms.assetid: 500b0423-864e-4cde-a39b-6b5b06d1aa6a
description: L’élément ContactSource indique si le contact se trouve dans la banque Exchange ou les Services de domaine Active Directory (AD DS).
ms.openlocfilehash: a82b766fc81b9397fc707415ea82e2f2d63d952d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755567"
---
# <a name="contactsource"></a><span data-ttu-id="3e13d-103">ContactSource</span><span class="sxs-lookup"><span data-stu-id="3e13d-103">ContactSource</span></span>

<span data-ttu-id="3e13d-104">L’élément **ContactSource** indique si le contact se trouve dans la banque Exchange ou les Services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="3e13d-104">The **ContactSource** element describes whether the contact is located in the Exchange store or Active Directory Domain Services (AD DS).</span></span> 
  
```xml
<ContactSource/>
```

 <span data-ttu-id="3e13d-105">**ContactSourceType**</span><span class="sxs-lookup"><span data-stu-id="3e13d-105">**ContactSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e13d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e13d-106">Attributes and elements</span></span>

<span data-ttu-id="3e13d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e13d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e13d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e13d-108">Attributes</span></span>

<span data-ttu-id="3e13d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e13d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e13d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e13d-110">Child elements</span></span>

<span data-ttu-id="3e13d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e13d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e13d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e13d-112">Parent elements</span></span>

|<span data-ttu-id="3e13d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e13d-113">**Element**</span></span>|<span data-ttu-id="3e13d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e13d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e13d-115">Contact</span><span class="sxs-lookup"><span data-stu-id="3e13d-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3e13d-116">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e13d-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e13d-117">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3e13d-117">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3e13d-118">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="3e13d-118">Represents a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e13d-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3e13d-119">Text value</span></span>

<span data-ttu-id="3e13d-120">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="3e13d-120">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="3e13d-121">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="3e13d-121">ActiveDirectory</span></span>
    
- <span data-ttu-id="3e13d-122">Store</span><span class="sxs-lookup"><span data-stu-id="3e13d-122">Store</span></span>
    
## <a name="remarks"></a><span data-ttu-id="3e13d-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e13d-123">Remarks</span></span>

<span data-ttu-id="3e13d-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e13d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e13d-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e13d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e13d-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e13d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e13d-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e13d-127">Schema name</span></span>  <br/> |<span data-ttu-id="3e13d-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3e13d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e13d-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e13d-129">Validation file</span></span>  <br/> |<span data-ttu-id="3e13d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e13d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e13d-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e13d-131">Can be empty</span></span>  <br/> |<span data-ttu-id="3e13d-132">False</span><span class="sxs-lookup"><span data-stu-id="3e13d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e13d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e13d-133">See also</span></span>



- [<span data-ttu-id="3e13d-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e13d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
