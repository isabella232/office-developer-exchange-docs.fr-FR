---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: L’élément DomainNames représente la collection de noms de domaine. L’élément DomainNames est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 0b425b3cd4c0e7cb2427920d61feb04010a3b123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458417"
---
# <a name="domainnames-soap"></a><span data-ttu-id="14f77-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14f77-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="14f77-106">L’élément **DomainNames** représente la collection de noms de domaine.</span><span class="sxs-lookup"><span data-stu-id="14f77-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="14f77-107">L’élément **DomainNames** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="14f77-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="14f77-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="14f77-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="14f77-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="14f77-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14f77-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="14f77-110">Attributes and elements</span></span>

<span data-ttu-id="14f77-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="14f77-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14f77-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="14f77-112">Attributes</span></span>

<span data-ttu-id="14f77-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="14f77-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14f77-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="14f77-114">Child elements</span></span>

|<span data-ttu-id="14f77-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="14f77-115">**Element**</span></span>|<span data-ttu-id="14f77-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="14f77-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14f77-117">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14f77-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="14f77-118">Représente une collection de domaines qui sont renvoyés à partir de l’opération [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), [GETFEDERATIONINFORMATION Operation (SOAP)](getfederationinformation-operation-soap.md)ou l' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="14f77-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14f77-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="14f77-119">Parent elements</span></span>

|<span data-ttu-id="14f77-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="14f77-120">**Element**</span></span>|<span data-ttu-id="14f77-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="14f77-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14f77-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14f77-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="14f77-123">Représente une liste de relations d’organisation pour une seule organisation.</span><span class="sxs-lookup"><span data-stu-id="14f77-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14f77-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="14f77-124">Text value</span></span>

<span data-ttu-id="14f77-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14f77-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14f77-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="14f77-126">Remarks</span></span>

<span data-ttu-id="14f77-127">Cet élément représente les domaines SMTP de l’organisation externe.</span><span class="sxs-lookup"><span data-stu-id="14f77-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14f77-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="14f77-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14f77-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="14f77-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="14f77-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="14f77-130">Schema Name</span></span>  <br/> |<span data-ttu-id="14f77-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="14f77-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="14f77-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="14f77-132">Validation File</span></span>  <br/> |<span data-ttu-id="14f77-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="14f77-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14f77-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="14f77-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="14f77-135">True</span><span class="sxs-lookup"><span data-stu-id="14f77-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14f77-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14f77-136">See also</span></span>

- [<span data-ttu-id="14f77-137">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14f77-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

