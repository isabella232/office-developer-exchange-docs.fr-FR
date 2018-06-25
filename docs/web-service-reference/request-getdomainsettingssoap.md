---
title: Demande (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: L’élément de demande contient une demande pour renvoyer les paramètres de domaine.
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829135"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="ddf36-103">Demande (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ddf36-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="ddf36-104">L’élément de **demande** contient une demande pour renvoyer les paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="ddf36-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="ddf36-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="ddf36-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddf36-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ddf36-106">Attributes and elements</span></span>

<span data-ttu-id="ddf36-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ddf36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddf36-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ddf36-108">Attributes</span></span>

<span data-ttu-id="ddf36-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddf36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddf36-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ddf36-110">Child elements</span></span>

|<span data-ttu-id="ddf36-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ddf36-111">**Element**</span></span>|<span data-ttu-id="ddf36-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ddf36-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddf36-113">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ddf36-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="ddf36-114">Représente les domaines les configurations pour lesquelles sont retournées dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou les domaines de que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="ddf36-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="ddf36-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ddf36-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="ddf36-116">Contient les noms des paramètres de configuration demandé.</span><span class="sxs-lookup"><span data-stu-id="ddf36-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ddf36-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ddf36-117">Parent elements</span></span>

|<span data-ttu-id="ddf36-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ddf36-118">**Element**</span></span>|<span data-ttu-id="ddf36-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="ddf36-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddf36-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ddf36-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="ddf36-121">Représente une demande [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="ddf36-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ddf36-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ddf36-122">Text value</span></span>

<span data-ttu-id="ddf36-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ddf36-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddf36-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ddf36-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddf36-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ddf36-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ddf36-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ddf36-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ddf36-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ddf36-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ddf36-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ddf36-128">Validation File</span></span>  <br/> |<span data-ttu-id="ddf36-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ddf36-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ddf36-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ddf36-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ddf36-131">True</span><span class="sxs-lookup"><span data-stu-id="ddf36-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ddf36-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ddf36-132">See also</span></span>



[<span data-ttu-id="ddf36-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ddf36-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

