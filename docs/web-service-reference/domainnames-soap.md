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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458417"
---
# <a name="domainnames-soap"></a><span data-ttu-id="ad861-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad861-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="ad861-106">L’élément **DomainNames** représente la collection de noms de domaine.</span><span class="sxs-lookup"><span data-stu-id="ad861-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="ad861-107">L’élément **DomainNames** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="ad861-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="ad861-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="ad861-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="ad861-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="ad861-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad861-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad861-110">Attributes and elements</span></span>

<span data-ttu-id="ad861-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad861-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad861-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad861-112">Attributes</span></span>

<span data-ttu-id="ad861-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad861-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad861-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad861-114">Child elements</span></span>

|<span data-ttu-id="ad861-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad861-115">**Element**</span></span>|<span data-ttu-id="ad861-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad861-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad861-117">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad861-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="ad861-118">Représente une collection de domaines qui sont renvoyés à partir de l’opération [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), [GETFEDERATIONINFORMATION Operation (SOAP)](getfederationinformation-operation-soap.md)ou l' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="ad861-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad861-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad861-119">Parent elements</span></span>

|<span data-ttu-id="ad861-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad861-120">**Element**</span></span>|<span data-ttu-id="ad861-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad861-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad861-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad861-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="ad861-123">Représente une liste de relations d’organisation pour une seule organisation.</span><span class="sxs-lookup"><span data-stu-id="ad861-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad861-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad861-124">Text value</span></span>

<span data-ttu-id="ad861-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad861-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad861-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad861-126">Remarks</span></span>

<span data-ttu-id="ad861-127">Cet élément représente les domaines SMTP de l’organisation externe.</span><span class="sxs-lookup"><span data-stu-id="ad861-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad861-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad861-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad861-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad861-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ad861-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad861-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ad861-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ad861-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ad861-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad861-132">Validation File</span></span>  <br/> |<span data-ttu-id="ad861-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ad861-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad861-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad861-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad861-135">True</span><span class="sxs-lookup"><span data-stu-id="ad861-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad861-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad861-136">See also</span></span>

- [<span data-ttu-id="ad861-137">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad861-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

