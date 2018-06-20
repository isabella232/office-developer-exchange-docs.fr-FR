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
description: L’élément de réponse contient les informations de réponse de l’opération (SOAP) GetFederationInformation.
ms.openlocfilehash: 946cba56d7503a0e20ec59640f4f1258c00a844e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829171"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="020d4-103">Réponse (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="020d4-104">L’élément de **réponse** contient les informations de réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="020d4-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="020d4-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="020d4-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="020d4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="020d4-106">Attributes and elements</span></span>

<span data-ttu-id="020d4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="020d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="020d4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="020d4-108">Attributes</span></span>

<span data-ttu-id="020d4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="020d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="020d4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="020d4-110">Child elements</span></span>

|<span data-ttu-id="020d4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="020d4-111">**Element**</span></span>|<span data-ttu-id="020d4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="020d4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="020d4-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="020d4-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="020d4-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="020d4-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="020d4-116">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="020d4-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="020d4-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="020d4-118">Définit l’emplacement d’une application.</span><span class="sxs-lookup"><span data-stu-id="020d4-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="020d4-119">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="020d4-120">Représente la collection de domaine les configurations pour lesquelles sont retournées dans une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), ou les domaines de l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="020d4-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="020d4-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="020d4-121">Parent elements</span></span>

|<span data-ttu-id="020d4-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="020d4-122">**Element**</span></span>|<span data-ttu-id="020d4-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="020d4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="020d4-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="020d4-125">Définit une réponse à une demande de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="020d4-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="020d4-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="020d4-126">Text value</span></span>

<span data-ttu-id="020d4-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="020d4-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="020d4-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="020d4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="020d4-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="020d4-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="020d4-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="020d4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="020d4-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="020d4-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="020d4-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="020d4-132">Validation File</span></span>  <br/> |<span data-ttu-id="020d4-133">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="020d4-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="020d4-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="020d4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="020d4-135">True</span><span class="sxs-lookup"><span data-stu-id="020d4-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="020d4-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="020d4-136">See also</span></span>



[<span data-ttu-id="020d4-137">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="020d4-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

