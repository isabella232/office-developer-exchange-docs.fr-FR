---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: L’élément DeliveryReportEnabled représente l’indicateur DeliveryReportEnabled(). L’élément DeliveryReportEnabled est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755891"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="6309f-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6309f-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="6309f-106">L’élément **DeliveryReportEnabled** représente l’indicateur **DeliveryReportEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="6309f-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="6309f-107">L’élément **DeliveryReportEnabled** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="6309f-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="6309f-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="6309f-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="6309f-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6309f-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6309f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6309f-110">Attributes and elements</span></span>

<span data-ttu-id="6309f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6309f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6309f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="6309f-112">Attributes</span></span>

<span data-ttu-id="6309f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6309f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6309f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6309f-114">Child elements</span></span>

<span data-ttu-id="6309f-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6309f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6309f-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6309f-116">Parent elements</span></span>

|<span data-ttu-id="6309f-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6309f-117">**Element**</span></span>|<span data-ttu-id="6309f-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="6309f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6309f-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6309f-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="6309f-120">Représente une liste des relations d’organisation pour une organisation unique.</span><span class="sxs-lookup"><span data-stu-id="6309f-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6309f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6309f-121">Text value</span></span>

<span data-ttu-id="6309f-122">Une valeur de texte de la valeur true pour l’élément DeliveryReportEnabled indique que vous pouvant utiliser les rapports de remise parmi les utilisateurs de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="6309f-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="6309f-123">La valeur false indique que les rapports de remise doit être supprimée.</span><span class="sxs-lookup"><span data-stu-id="6309f-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6309f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="6309f-124">Remarks</span></span>

<span data-ttu-id="6309f-125">Utilisez cet élément pour autoriser ou supprimer des rapports de remise à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="6309f-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6309f-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6309f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6309f-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6309f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6309f-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6309f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6309f-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="6309f-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6309f-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6309f-130">Validation File</span></span>  <br/> |<span data-ttu-id="6309f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6309f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6309f-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6309f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6309f-133">True</span><span class="sxs-lookup"><span data-stu-id="6309f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6309f-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6309f-134">See also</span></span>

- [<span data-ttu-id="6309f-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6309f-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

