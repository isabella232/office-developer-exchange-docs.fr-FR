---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: L’élément GetOrganizationRelationshipSettingsResponse contient la réponse de l’opération (SOAP) GetOrganizationRelationshipSettings. L’élément GetOrganizationRelationshipSettingsResponse est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756692"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="265dd-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="265dd-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="265dd-106">L’élément **GetOrganizationRelationshipSettingsResponse** contient la réponse de [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="265dd-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="265dd-107">L’élément **GetOrganizationRelationshipSettingsResponse** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="265dd-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="265dd-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="265dd-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="265dd-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="265dd-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="265dd-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="265dd-110">Attributes and elements</span></span>

<span data-ttu-id="265dd-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="265dd-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="265dd-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="265dd-112">Attributes</span></span>

<span data-ttu-id="265dd-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="265dd-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="265dd-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="265dd-114">Child elements</span></span>

|<span data-ttu-id="265dd-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="265dd-115">**Element**</span></span>|<span data-ttu-id="265dd-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="265dd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="265dd-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="265dd-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="265dd-118">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="265dd-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="265dd-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="265dd-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="265dd-120">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="265dd-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="265dd-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="265dd-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="265dd-122">Représente une collection de relations qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="265dd-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="265dd-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="265dd-123">Parent elements</span></span>

<span data-ttu-id="265dd-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="265dd-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="265dd-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="265dd-125">Text value</span></span>

<span data-ttu-id="265dd-126">Aucun.</span><span class="sxs-lookup"><span data-stu-id="265dd-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="265dd-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="265dd-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="265dd-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="265dd-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="265dd-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="265dd-129">Schema Name</span></span>  <br/> |<span data-ttu-id="265dd-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="265dd-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="265dd-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="265dd-131">Validation File</span></span>  <br/> |<span data-ttu-id="265dd-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="265dd-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="265dd-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="265dd-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="265dd-134">True</span><span class="sxs-lookup"><span data-stu-id="265dd-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="265dd-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="265dd-135">See also</span></span>



[<span data-ttu-id="265dd-136">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="265dd-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

