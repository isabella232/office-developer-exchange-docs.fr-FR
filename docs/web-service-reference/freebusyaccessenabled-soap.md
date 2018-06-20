---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: L’élément FreeBusyAccessEnabled représente l’indicateur FreeBusyAccessEnabled(). L’élément FreeBusyAccessEnabled est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756483"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="72ae7-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72ae7-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="72ae7-106">L’élément **FreeBusyAccessEnabled** représente l’indicateur **FreeBusyAccessEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="72ae7-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="72ae7-107">L’élément **FreeBusyAccessEnabled** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="72ae7-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="72ae7-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="72ae7-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="72ae7-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="72ae7-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72ae7-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="72ae7-110">Attributes and elements</span></span>

<span data-ttu-id="72ae7-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="72ae7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72ae7-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="72ae7-112">Attributes</span></span>

<span data-ttu-id="72ae7-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="72ae7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72ae7-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="72ae7-114">Child elements</span></span>

<span data-ttu-id="72ae7-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="72ae7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72ae7-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="72ae7-116">Parent elements</span></span>

|<span data-ttu-id="72ae7-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="72ae7-117">**Element**</span></span>|<span data-ttu-id="72ae7-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="72ae7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72ae7-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72ae7-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="72ae7-120">Représente une liste des relations d’organisation pour une organisation unique.</span><span class="sxs-lookup"><span data-stu-id="72ae7-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72ae7-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="72ae7-121">Text value</span></span>

<span data-ttu-id="72ae7-122">Une valeur de texte de **la valeur true** pour l’élément **FreeBusyAccessEnabled** indique que la relation de partage doit être utilisée pour récupérer des informations sur la disponibilité des utilisateurs dans l’organisation.</span><span class="sxs-lookup"><span data-stu-id="72ae7-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="72ae7-123">La valeur **false** indique que la relation de partage doit être supprimée.</span><span class="sxs-lookup"><span data-stu-id="72ae7-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="72ae7-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="72ae7-124">Remarks</span></span>

<span data-ttu-id="72ae7-125">Utilisez cet élément pour autoriser ou supprimer les informations de disponibilité à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="72ae7-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="72ae7-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="72ae7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72ae7-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="72ae7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="72ae7-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="72ae7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="72ae7-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="72ae7-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="72ae7-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="72ae7-130">Validation File</span></span>  <br/> |<span data-ttu-id="72ae7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="72ae7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72ae7-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="72ae7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="72ae7-133">True</span><span class="sxs-lookup"><span data-stu-id="72ae7-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72ae7-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="72ae7-134">See also</span></span>



[<span data-ttu-id="72ae7-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="72ae7-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

