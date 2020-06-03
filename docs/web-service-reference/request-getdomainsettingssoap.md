---
title: Request (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: L’élément Request contient une demande de renvoi des paramètres de domaine.
ms.openlocfilehash: c5f666102be8aaeee001a23706732e9e6c44b560
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459587"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="5b529-103">Request (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5b529-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="5b529-104">L’élément **Request** contient une demande de renvoi des paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="5b529-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="5b529-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="5b529-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b529-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5b529-106">Attributes and elements</span></span>

<span data-ttu-id="5b529-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5b529-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b529-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5b529-108">Attributes</span></span>

<span data-ttu-id="5b529-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5b529-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b529-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5b529-110">Child elements</span></span>

|<span data-ttu-id="5b529-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b529-111">**Element**</span></span>|<span data-ttu-id="5b529-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b529-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b529-113">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5b529-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="5b529-114">Représente les domaines dont les configurations sont renvoyées dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou les domaines que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="5b529-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="5b529-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5b529-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="5b529-116">Contient les noms des paramètres de configuration demandés.</span><span class="sxs-lookup"><span data-stu-id="5b529-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b529-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5b529-117">Parent elements</span></span>

|<span data-ttu-id="5b529-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b529-118">**Element**</span></span>|<span data-ttu-id="5b529-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b529-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b529-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5b529-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="5b529-121">Représente une demande d' [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="5b529-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b529-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5b529-122">Text value</span></span>

<span data-ttu-id="5b529-123">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5b529-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b529-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5b529-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b529-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5b529-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5b529-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5b529-126">Schema Name</span></span>  <br/> |<span data-ttu-id="5b529-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5b529-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5b529-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5b529-128">Validation File</span></span>  <br/> |<span data-ttu-id="5b529-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5b529-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b529-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5b529-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b529-131">True</span><span class="sxs-lookup"><span data-stu-id="5b529-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b529-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5b529-132">See also</span></span>



[<span data-ttu-id="5b529-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5b529-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

