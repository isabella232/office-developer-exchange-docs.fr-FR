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
description: L’élément Response contient la réponse à une demande d’opération GetUserSettings (SOAP), GetDomainSettings Operation (SOAP) ou GetFederationInformation Operation (SOAP).
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456415"
---
# <a name="response-soap"></a><span data-ttu-id="4a04a-103">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-103">Response (SOAP)</span></span>

<span data-ttu-id="4a04a-104">L’élément **Response** contient la réponse à une demande d’opération [GetUserSettings (SOAP](getusersettings-operation-soap.md)), [GetDomainSettings Operation (SOAP)](getdomainsettings-operation-soap.md)ou [GetFederationInformation Operation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="4a04a-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="4a04a-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="4a04a-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a04a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a04a-106">Attributes and elements</span></span>

<span data-ttu-id="4a04a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a04a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a04a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a04a-108">Attributes</span></span>

<span data-ttu-id="4a04a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a04a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a04a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a04a-110">Child elements</span></span>

|<span data-ttu-id="4a04a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a04a-111">**Element**</span></span>|<span data-ttu-id="4a04a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a04a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a04a-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="4a04a-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="4a04a-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="4a04a-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="4a04a-116">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="4a04a-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="4a04a-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="4a04a-118">Contient les paramètres de configuration de chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="4a04a-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a04a-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a04a-119">Parent elements</span></span>

|<span data-ttu-id="4a04a-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a04a-120">**Element**</span></span>|<span data-ttu-id="4a04a-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a04a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a04a-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="4a04a-123">Définit une réponse à une [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="4a04a-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="4a04a-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="4a04a-125">Définit une réponse à un [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="4a04a-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="4a04a-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="4a04a-127">Définit une réponse à un [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="4a04a-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a04a-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4a04a-128">Text value</span></span>

<span data-ttu-id="4a04a-129">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a04a-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a04a-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a04a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a04a-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a04a-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4a04a-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a04a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4a04a-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4a04a-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4a04a-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a04a-134">Validation File</span></span>  <br/> |<span data-ttu-id="4a04a-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4a04a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a04a-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a04a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a04a-137">True</span><span class="sxs-lookup"><span data-stu-id="4a04a-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a04a-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a04a-138">See also</span></span>



[<span data-ttu-id="4a04a-139">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a04a-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="4a04a-140">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4a04a-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="4a04a-141">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4a04a-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

