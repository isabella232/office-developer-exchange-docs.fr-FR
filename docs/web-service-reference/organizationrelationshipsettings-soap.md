---
title: OrganizationRelationshipSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: L’élément OrganizationRelationshipSettings représente une liste des relations d’organisation pour une organisation unique. L’élément OrganizationRelationshipSettings est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: ed6cc0ef1891cd92c02a8e088e913886048623ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828660"
---
# <a name="organizationrelationshipsettings-soap"></a><span data-ttu-id="d923b-105">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-105">OrganizationRelationshipSettings (SOAP)</span></span>

<span data-ttu-id="d923b-106">L’élément **OrganizationRelationshipSettings** représente une liste des relations d’organisation pour une organisation unique.</span><span class="sxs-lookup"><span data-stu-id="d923b-106">The **OrganizationRelationshipSettings** element represents a list of organization relationships for a single organization.</span></span> <span data-ttu-id="d923b-107">L’élément **OrganizationRelationshipSettings** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="d923b-107">The **OrganizationRelationshipSettings** element is for internal use only.</span></span> <span data-ttu-id="d923b-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="d923b-108">This element is not used by clients.</span></span> 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 <span data-ttu-id="d923b-109">**OrganizationRelationshipSettings**</span><span class="sxs-lookup"><span data-stu-id="d923b-109">**OrganizationRelationshipSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d923b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d923b-110">Attributes and elements</span></span>

<span data-ttu-id="d923b-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d923b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d923b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d923b-112">Attributes</span></span>

<span data-ttu-id="d923b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d923b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d923b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d923b-114">Child elements</span></span>

|<span data-ttu-id="d923b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d923b-115">**Element**</span></span>|<span data-ttu-id="d923b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d923b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d923b-117">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-117">DeliveryReportEnabled (SOAP)</span></span>](deliveryreportenabled-soap.md) <br/> |<span data-ttu-id="d923b-118">Représente l’indicateur [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-118">Represents the [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="d923b-119">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-119">DomainNames (SOAP)</span></span>](domainnames-soap.md) <br/> |<span data-ttu-id="d923b-120">Représente la collection de noms de domaine.</span><span class="sxs-lookup"><span data-stu-id="d923b-120">Represents the domain names collection.</span></span>  <br/> |
|[<span data-ttu-id="d923b-121">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-121">FreeBusyAccessEnabled (SOAP)</span></span>](freebusyaccessenabled-soap.md) <br/> |<span data-ttu-id="d923b-122">Représente l’indicateur [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-122">Represents the [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="d923b-123">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-123">FreeBusyAccessLevel (SOAP)</span></span>](freebusyaccesslevel-soap.md) <br/> |<span data-ttu-id="d923b-124">Représente la propriété [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-124">Represents the [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="d923b-125">MailTipsAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-125">MailTipsAccessEnabled (SOAP)</span></span>](mailtipsaccessenabled-soap.md) <br/> |<span data-ttu-id="d923b-126">Représente l’indicateur [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-126">Represents the [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="d923b-127">MailTipsAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-127">MailTipsAccessLevel (SOAP)</span></span>](mailtipsaccesslevel-soap.md) <br/> |<span data-ttu-id="d923b-128">Représente la propriété [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-128">Represents the [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="d923b-129">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-129">MailboxMoveEnabled (SOAP)</span></span>](mailboxmoveenabled-soap.md) <br/> |<span data-ttu-id="d923b-130">Représente l’indicateur [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-130">Represents the [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="d923b-131">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-131">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="d923b-132">Représente le nom de la relation d’organisation.</span><span class="sxs-lookup"><span data-stu-id="d923b-132">Represents the name of the organization relationship.</span></span>  <br/> |
|[<span data-ttu-id="d923b-133">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-133">TargetApplicationUri (SOAP)</span></span>](targetapplicationuri-soap.md) <br/> |<span data-ttu-id="d923b-134">Définit l’URI d’application cible.</span><span class="sxs-lookup"><span data-stu-id="d923b-134">Defines the target application URI.</span></span>  <br/> |
|[<span data-ttu-id="d923b-135">TargetAutodiscoverEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-135">TargetAutodiscoverEpr (SOAP)</span></span>](targetautodiscoverepr-soap.md) <br/> |<span data-ttu-id="d923b-136">Représente la propriété [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-136">Represents the [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="d923b-137">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-137">TargetSharingEpr (SOAP)</span></span>](targetsharingepr-soap.md) <br/> |<span data-ttu-id="d923b-138">Représente la propriété [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d923b-138">Represents the [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d923b-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d923b-139">Parent elements</span></span>

|<span data-ttu-id="d923b-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d923b-140">**Element**</span></span>|<span data-ttu-id="d923b-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="d923b-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d923b-142">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d923b-142">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="d923b-143">Représente une liste des relations qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="d923b-143">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d923b-144">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d923b-144">Text value</span></span>

<span data-ttu-id="d923b-145">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d923b-145">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d923b-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d923b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d923b-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d923b-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d923b-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d923b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="d923b-149">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d923b-149">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d923b-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d923b-150">Validation File</span></span>  <br/> |<span data-ttu-id="d923b-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d923b-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d923b-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d923b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="d923b-153">True</span><span class="sxs-lookup"><span data-stu-id="d923b-153">True</span></span>  <br/> |
   

