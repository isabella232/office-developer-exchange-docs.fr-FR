---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: L’élément GetFederationInformationResponse contient la réponse de l’opération (SOAP) GetFederationInformation.
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756614"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="f3e09-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="f3e09-104">L’élément **GetFederationInformationResponse** contient la réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f3e09-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="f3e09-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="f3e09-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3e09-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3e09-106">Attributes and elements</span></span>

<span data-ttu-id="f3e09-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3e09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3e09-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3e09-108">Attributes</span></span>

<span data-ttu-id="f3e09-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3e09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3e09-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3e09-110">Child elements</span></span>

|<span data-ttu-id="f3e09-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3e09-111">**Element**</span></span>|<span data-ttu-id="f3e09-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3e09-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3e09-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="f3e09-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f3e09-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f3e09-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="f3e09-116">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f3e09-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f3e09-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="f3e09-118">Définit l’emplacement d’une application.</span><span class="sxs-lookup"><span data-stu-id="f3e09-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="f3e09-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="f3e09-120">Représente une collection de jetons de sécurité qui contiennent des points de terminaison et les identificateurs de service de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="f3e09-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="f3e09-121">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="f3e09-122">Représente les domaines les configurations pour lesquelles sont retournées dans une opération de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou les domaines de que l’organisation a fédérés dans une [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Opération **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="f3e09-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3e09-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3e09-123">Parent elements</span></span>

<span data-ttu-id="f3e09-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3e09-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f3e09-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f3e09-125">Text value</span></span>

<span data-ttu-id="f3e09-126">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3e09-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3e09-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3e09-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3e09-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3e09-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f3e09-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3e09-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f3e09-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f3e09-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f3e09-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3e09-131">Validation File</span></span>  <br/> |<span data-ttu-id="f3e09-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3e09-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3e09-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3e09-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3e09-134">True</span><span class="sxs-lookup"><span data-stu-id="f3e09-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3e09-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3e09-135">See also</span></span>



[<span data-ttu-id="f3e09-136">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3e09-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

