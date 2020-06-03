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
description: L’élément GetFederationInformationResponse contient la réponse SOAP (GetFederationInformation Operation).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460042"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="f540f-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="f540f-104">L’élément **GetFederationInformationResponse** contient la réponse [SOAP (GetFederationInformation Operation)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f540f-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="f540f-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="f540f-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f540f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f540f-106">Attributes and elements</span></span>

<span data-ttu-id="f540f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f540f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f540f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f540f-108">Attributes</span></span>

<span data-ttu-id="f540f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f540f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f540f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f540f-110">Child elements</span></span>

|<span data-ttu-id="f540f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f540f-111">**Element**</span></span>|<span data-ttu-id="f540f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f540f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f540f-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="f540f-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f540f-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f540f-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="f540f-116">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f540f-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f540f-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="f540f-118">Définit l’emplacement d’une application.</span><span class="sxs-lookup"><span data-stu-id="f540f-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="f540f-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="f540f-120">Représente une collection de jetons de sécurité, qui contiennent des identificateurs de service d’émission de jeton de sécurité et des points de terminaison.</span><span class="sxs-lookup"><span data-stu-id="f540f-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="f540f-121">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="f540f-122">Représente les domaines dont les configurations sont renvoyées dans une opération [GetDomainSettings Operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou les domaines dans lesquels l’organisation a fédéré dans une opération [GetFederationInformation Operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="f540f-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f540f-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f540f-123">Parent elements</span></span>

<span data-ttu-id="f540f-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f540f-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f540f-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f540f-125">Text value</span></span>

<span data-ttu-id="f540f-126">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f540f-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f540f-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f540f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f540f-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f540f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f540f-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f540f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f540f-130">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f540f-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f540f-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f540f-131">Validation File</span></span>  <br/> |<span data-ttu-id="f540f-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f540f-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f540f-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f540f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f540f-134">True</span><span class="sxs-lookup"><span data-stu-id="f540f-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f540f-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f540f-135">See also</span></span>



[<span data-ttu-id="f540f-136">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f540f-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

