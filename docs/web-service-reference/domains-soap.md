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
description: L’élément de domaines représente la collection de domaine qui est retournée dans une opération de GetDomainSettings (SOAP), les domaines que l’organisation a fédérés dans une opération de GetFederationInformation (SOAP) ou les domaines avec une relation d’organisation renvoyée par l’opération GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 7a21a3a09516de2d1c38021ca3ccd2161d9cdd1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756040"
---
# <a name="domains-soap"></a><span data-ttu-id="15918-103">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-103">Domains (SOAP)</span></span>

<span data-ttu-id="15918-104">L’élément de **domaines** représente la collection de domaine qui est retournée dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), les domaines que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou les domaines avec une relation d’organisation renvoyé par [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="15918-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="15918-105">**Domaines**</span><span class="sxs-lookup"><span data-stu-id="15918-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15918-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="15918-106">Attributes and elements</span></span>

<span data-ttu-id="15918-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="15918-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15918-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="15918-108">Attributes</span></span>

<span data-ttu-id="15918-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15918-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15918-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="15918-110">Child elements</span></span>

|<span data-ttu-id="15918-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15918-111">**Element**</span></span>|<span data-ttu-id="15918-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="15918-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15918-113">Domaine (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="15918-114">Représente un seul domaine.</span><span class="sxs-lookup"><span data-stu-id="15918-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15918-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="15918-115">Parent elements</span></span>

|<span data-ttu-id="15918-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15918-116">**Element**</span></span>|<span data-ttu-id="15918-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="15918-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15918-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="15918-119">Représente une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="15918-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="15918-120">Réponse (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="15918-121">Contient les informations de réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="15918-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="15918-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="15918-123">Représente une demande [d’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="15918-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15918-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="15918-124">Text value</span></span>

<span data-ttu-id="15918-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15918-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15918-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="15918-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15918-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="15918-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="15918-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="15918-128">Schema Name</span></span>  <br/> |<span data-ttu-id="15918-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="15918-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="15918-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="15918-130">Validation File</span></span>  <br/> |<span data-ttu-id="15918-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="15918-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15918-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="15918-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="15918-133">True</span><span class="sxs-lookup"><span data-stu-id="15918-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15918-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15918-134">See also</span></span>

- [<span data-ttu-id="15918-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="15918-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="15918-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)

