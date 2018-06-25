---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: L’élément ErrorMessage représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756214"
---
# <a name="errormessage-soap"></a><span data-ttu-id="1f83c-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="1f83c-104">L’élément **ErrorMessage** représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f83c-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="1f83c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="1f83c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f83c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f83c-106">Attributes and elements</span></span>

<span data-ttu-id="1f83c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f83c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f83c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f83c-108">Attributes</span></span>

<span data-ttu-id="1f83c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1f83c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f83c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f83c-110">Child elements</span></span>

<span data-ttu-id="1f83c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1f83c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f83c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f83c-112">Parent elements</span></span>

|<span data-ttu-id="1f83c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f83c-113">**Element**</span></span>|<span data-ttu-id="1f83c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f83c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f83c-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="1f83c-116">Représente le type de base pour toutes les réponses sont renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f83c-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="1f83c-118">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="1f83c-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="1f83c-120">Contient la réponse à un appel de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine spécifique.</span><span class="sxs-lookup"><span data-stu-id="1f83c-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="1f83c-122">Contient la réponse à une demande [d’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1f83c-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="1f83c-124">Contient la réponse à une demande [d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1f83c-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="1f83c-126">Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1f83c-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="1f83c-127">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="1f83c-128">Représente une réponse à une demande de [l’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="1f83c-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f83c-129">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1f83c-129">Text value</span></span>

<span data-ttu-id="1f83c-130">La valeur de texte représente le message d’erreur.</span><span class="sxs-lookup"><span data-stu-id="1f83c-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f83c-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f83c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f83c-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f83c-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1f83c-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f83c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1f83c-134">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="1f83c-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1f83c-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1f83c-135">Validation File</span></span>  <br/> |<span data-ttu-id="1f83c-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1f83c-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f83c-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f83c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f83c-138">True</span><span class="sxs-lookup"><span data-stu-id="1f83c-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f83c-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f83c-139">See also</span></span>



[<span data-ttu-id="1f83c-140">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="1f83c-141">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="1f83c-142">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f83c-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

