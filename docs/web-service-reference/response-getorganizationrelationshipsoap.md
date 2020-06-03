---
title: Réponse (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: L’élément Response contient les informations de réponse de l’opération GetOrganizationRelationshipSettings (SOAP). L’élément Response est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 55f8cd549f40b780b2e7438634a851a2c3854f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467941"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="3a962-105">Réponse (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a962-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="3a962-106">L’élément **Response** contient les informations de réponse de l' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="3a962-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="3a962-107">L’élément **Response** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="3a962-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="3a962-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="3a962-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="3a962-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="3a962-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a962-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3a962-110">Attributes and elements</span></span>

<span data-ttu-id="3a962-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3a962-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a962-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3a962-112">Attributes</span></span>

<span data-ttu-id="3a962-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3a962-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a962-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3a962-114">Child elements</span></span>

|<span data-ttu-id="3a962-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a962-115">**Element**</span></span>|<span data-ttu-id="3a962-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a962-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a962-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a962-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3a962-118">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="3a962-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3a962-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a962-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3a962-120">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="3a962-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3a962-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a962-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="3a962-122">Représente la liste des relations d’organisation qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="3a962-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a962-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3a962-123">Parent elements</span></span>

<span data-ttu-id="3a962-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3a962-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3a962-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3a962-125">Text value</span></span>

<span data-ttu-id="3a962-126">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3a962-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a962-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3a962-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a962-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3a962-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3a962-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3a962-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3a962-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="3a962-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3a962-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3a962-131">Validation File</span></span>  <br/> |<span data-ttu-id="3a962-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3a962-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a962-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3a962-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a962-134">True</span><span class="sxs-lookup"><span data-stu-id="3a962-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a962-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3a962-135">See also</span></span>



[<span data-ttu-id="3a962-136">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3a962-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

