---
title: Réponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: L’élément de réponse contient la réponse à une opération GetUserSettings (SOAP), l’opération GetDomainSettings (SOAP) ou une demande d’opération (SOAP) GetFederationInformation.
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829179"
---
# <a name="response-soap"></a><span data-ttu-id="ded0b-103">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-103">Response (SOAP)</span></span>

<span data-ttu-id="ded0b-104">L’élément de **réponse** contient la réponse à une [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md), [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou une demande [d’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ded0b-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="ded0b-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="ded0b-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ded0b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ded0b-106">Attributes and elements</span></span>

<span data-ttu-id="ded0b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ded0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ded0b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ded0b-108">Attributes</span></span>

<span data-ttu-id="ded0b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ded0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ded0b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ded0b-110">Child elements</span></span>

|<span data-ttu-id="ded0b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ded0b-111">**Element**</span></span>|<span data-ttu-id="ded0b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ded0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded0b-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="ded0b-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ded0b-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="ded0b-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="ded0b-116">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ded0b-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="ded0b-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="ded0b-118">Contient les paramètres de configuration pour chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="ded0b-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ded0b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ded0b-119">Parent elements</span></span>

|<span data-ttu-id="ded0b-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ded0b-120">**Element**</span></span>|<span data-ttu-id="ded0b-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="ded0b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded0b-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="ded0b-123">Définit une réponse à une [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="ded0b-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="ded0b-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="ded0b-125">Définit une réponse à une [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="ded0b-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="ded0b-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="ded0b-127">Définit une réponse à une [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="ded0b-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ded0b-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ded0b-128">Text value</span></span>

<span data-ttu-id="ded0b-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ded0b-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ded0b-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ded0b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ded0b-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ded0b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ded0b-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ded0b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ded0b-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ded0b-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ded0b-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ded0b-134">Validation File</span></span>  <br/> |<span data-ttu-id="ded0b-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ded0b-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ded0b-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ded0b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ded0b-137">True</span><span class="sxs-lookup"><span data-stu-id="ded0b-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ded0b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ded0b-138">See also</span></span>



[<span data-ttu-id="ded0b-139">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ded0b-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="ded0b-140">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ded0b-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="ded0b-141">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ded0b-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

