---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: L’élément DomainNames représente la collection de noms de domaine. L’élément DomainNames est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 45d256f3d5a57028a04572ad67d4be0786ca39e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756031"
---
# <a name="domainnames-soap"></a><span data-ttu-id="daf9f-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="daf9f-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="daf9f-106">L’élément **DomainNames** représente la collection de noms de domaine.</span><span class="sxs-lookup"><span data-stu-id="daf9f-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="daf9f-107">L’élément **DomainNames** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="daf9f-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="daf9f-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="daf9f-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="daf9f-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="daf9f-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="daf9f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="daf9f-110">Attributes and elements</span></span>

<span data-ttu-id="daf9f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="daf9f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="daf9f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="daf9f-112">Attributes</span></span>

<span data-ttu-id="daf9f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="daf9f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="daf9f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="daf9f-114">Child elements</span></span>

|<span data-ttu-id="daf9f-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="daf9f-115">**Element**</span></span>|<span data-ttu-id="daf9f-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="daf9f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="daf9f-117">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="daf9f-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="daf9f-118">Représente une collection de domaines qui sont renvoyés à partir de l' [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou l' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="daf9f-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="daf9f-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="daf9f-119">Parent elements</span></span>

|<span data-ttu-id="daf9f-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="daf9f-120">**Element**</span></span>|<span data-ttu-id="daf9f-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="daf9f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="daf9f-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="daf9f-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="daf9f-123">Représente une liste des relations d’organisation pour une organisation unique.</span><span class="sxs-lookup"><span data-stu-id="daf9f-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="daf9f-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="daf9f-124">Text value</span></span>

<span data-ttu-id="daf9f-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="daf9f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="daf9f-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="daf9f-126">Remarks</span></span>

<span data-ttu-id="daf9f-127">Cet élément représente les domaines SMTP des organisations externes.</span><span class="sxs-lookup"><span data-stu-id="daf9f-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="daf9f-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="daf9f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="daf9f-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="daf9f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="daf9f-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="daf9f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="daf9f-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="daf9f-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="daf9f-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="daf9f-132">Validation File</span></span>  <br/> |<span data-ttu-id="daf9f-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="daf9f-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="daf9f-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="daf9f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="daf9f-135">True</span><span class="sxs-lookup"><span data-stu-id="daf9f-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="daf9f-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="daf9f-136">See also</span></span>

- [<span data-ttu-id="daf9f-137">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="daf9f-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

