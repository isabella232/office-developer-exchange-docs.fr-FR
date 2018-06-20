---
title: Réponse (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: L’élément de réponse contient les informations de réponse de l’opération (SOAP) GetOrganizationRelationshipSettings. L’élément de réponse est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 97bef9ab9f0b860e62646703c35d539b7922a65a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829174"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="a3cb7-105">Réponse (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a3cb7-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="a3cb7-106">L’élément de **réponse** contient les informations de réponse de [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="a3cb7-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="a3cb7-107">L’élément de **réponse** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="a3cb7-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="a3cb7-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="a3cb7-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3cb7-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a3cb7-110">Attributes and elements</span></span>

<span data-ttu-id="a3cb7-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3cb7-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="a3cb7-112">Attributes</span></span>

<span data-ttu-id="a3cb7-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3cb7-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a3cb7-114">Child elements</span></span>

|<span data-ttu-id="a3cb7-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a3cb7-115">**Element**</span></span>|<span data-ttu-id="a3cb7-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="a3cb7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3cb7-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a3cb7-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="a3cb7-118">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a3cb7-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a3cb7-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="a3cb7-120">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a3cb7-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a3cb7-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="a3cb7-122">Représente une liste des relations qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3cb7-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a3cb7-123">Parent elements</span></span>

<span data-ttu-id="a3cb7-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a3cb7-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a3cb7-125">Text value</span></span>

<span data-ttu-id="a3cb7-126">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a3cb7-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3cb7-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a3cb7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3cb7-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a3cb7-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a3cb7-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a3cb7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a3cb7-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="a3cb7-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a3cb7-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a3cb7-131">Validation File</span></span>  <br/> |<span data-ttu-id="a3cb7-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3cb7-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3cb7-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a3cb7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3cb7-134">True</span><span class="sxs-lookup"><span data-stu-id="a3cb7-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3cb7-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a3cb7-135">See also</span></span>



[<span data-ttu-id="a3cb7-136">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a3cb7-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
