---
title: Domaines (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: L’élément Domains représente la collection de domaines qui est renvoyée dans une opération GetDomainSettings (SOAP), les domaines que l’organisation a fédérés dans une opération GetFederationInformation (SOAP) ou les domaines avec une relation organisationnelle renvoyée par GetOrganizationRelationshipSettings Operation (SOAP).
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526304"
---
# <a name="domains-soap"></a><span data-ttu-id="65093-103">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-103">Domains (SOAP)</span></span>

<span data-ttu-id="65093-104">L’élément **Domains** représente la collection de domaines qui est renvoyée dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), les domaines que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou les domaines avec une relation organisationnelle renvoyée par [GetOrganizationRelationshipSettings Operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="65093-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="65093-105">**Domaines**</span><span class="sxs-lookup"><span data-stu-id="65093-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65093-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65093-106">Attributes and elements</span></span>

<span data-ttu-id="65093-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65093-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65093-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65093-108">Attributes</span></span>

<span data-ttu-id="65093-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="65093-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65093-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65093-110">Child elements</span></span>

|<span data-ttu-id="65093-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65093-111">**Element**</span></span>|<span data-ttu-id="65093-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="65093-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65093-113">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="65093-114">Représente un domaine unique.</span><span class="sxs-lookup"><span data-stu-id="65093-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65093-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65093-115">Parent elements</span></span>

|<span data-ttu-id="65093-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65093-116">**Element**</span></span>|<span data-ttu-id="65093-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="65093-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65093-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="65093-119">Représente une demande d' [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="65093-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="65093-120">Réponse (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="65093-121">Contient les informations de réponse de l' [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="65093-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="65093-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="65093-123">Représente une demande d' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="65093-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65093-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="65093-124">Text value</span></span>

<span data-ttu-id="65093-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="65093-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65093-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65093-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65093-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65093-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="65093-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65093-128">Schema Name</span></span>  <br/> |<span data-ttu-id="65093-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="65093-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="65093-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65093-130">Validation File</span></span>  <br/> |<span data-ttu-id="65093-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="65093-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65093-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65093-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="65093-133">True</span><span class="sxs-lookup"><span data-stu-id="65093-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65093-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65093-134">See also</span></span>

- [<span data-ttu-id="65093-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="65093-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="65093-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)

