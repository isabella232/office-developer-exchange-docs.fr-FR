---
title: Réponse (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: L’élément Response contient les informations de réponse de l’opération GetFederationInformation (SOAP).
ms.openlocfilehash: 0b9a2c518b968faa6ef86b7c1f544eac40f8e5c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530585"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="d3339-103">Réponse (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="d3339-104">L’élément **Response** contient les informations de réponse de l' [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d3339-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="d3339-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="d3339-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3339-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3339-106">Attributes and elements</span></span>

<span data-ttu-id="d3339-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3339-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3339-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3339-108">Attributes</span></span>

<span data-ttu-id="d3339-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d3339-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3339-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3339-110">Child elements</span></span>

|<span data-ttu-id="d3339-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3339-111">**Element**</span></span>|<span data-ttu-id="d3339-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3339-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3339-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="d3339-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="d3339-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d3339-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="d3339-116">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="d3339-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d3339-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="d3339-118">Définit l’emplacement d’une application.</span><span class="sxs-lookup"><span data-stu-id="d3339-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="d3339-119">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d3339-120">Représente la collection de domaines dont les configurations sont renvoyées dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou les domaines que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d3339-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3339-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3339-121">Parent elements</span></span>

|<span data-ttu-id="d3339-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3339-122">**Element**</span></span>|<span data-ttu-id="d3339-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3339-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3339-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="d3339-125">Définit une réponse à une demande d' [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d3339-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3339-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d3339-126">Text value</span></span>

<span data-ttu-id="d3339-127">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d3339-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3339-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3339-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3339-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3339-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d3339-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3339-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d3339-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d3339-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d3339-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3339-132">Validation File</span></span>  <br/> |<span data-ttu-id="d3339-133">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d3339-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3339-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3339-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3339-135">True</span><span class="sxs-lookup"><span data-stu-id="d3339-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3339-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3339-136">See also</span></span>



[<span data-ttu-id="d3339-137">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3339-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

