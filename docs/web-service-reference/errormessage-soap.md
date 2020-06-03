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
description: L’élément ErrorMessage représente un message qui est associé à un code d’erreur renvoyé par le service de découverte automatique.
ms.openlocfilehash: 4ebaf91fe26083cf241826e1fc16ac184fddf57c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530641"
---
# <a name="errormessage-soap"></a><span data-ttu-id="f36f8-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="f36f8-104">L’élément **ErrorMessage** représente un message qui est associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f36f8-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="f36f8-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="f36f8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f36f8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f36f8-106">Attributes and elements</span></span>

<span data-ttu-id="f36f8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f36f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f36f8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f36f8-108">Attributes</span></span>

<span data-ttu-id="f36f8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f36f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f36f8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f36f8-110">Child elements</span></span>

<span data-ttu-id="f36f8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f36f8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f36f8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f36f8-112">Parent elements</span></span>

|<span data-ttu-id="f36f8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f36f8-113">**Element**</span></span>|<span data-ttu-id="f36f8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f36f8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f36f8-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="f36f8-116">Représente le type de base pour toutes les réponses renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f36f8-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="f36f8-118">Contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="f36f8-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="f36f8-120">Contient la réponse à un appel [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) pour un domaine individuel.</span><span class="sxs-lookup"><span data-stu-id="f36f8-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="f36f8-122">Contient la réponse à une demande d' [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f36f8-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="f36f8-124">Contient la réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f36f8-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="f36f8-126">Représente une erreur renvoyée lors de la récupération d’un paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f36f8-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="f36f8-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="f36f8-128">Représente une réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="f36f8-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f36f8-129">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f36f8-129">Text value</span></span>

<span data-ttu-id="f36f8-130">La valeur texte représente le message d’erreur.</span><span class="sxs-lookup"><span data-stu-id="f36f8-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f36f8-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f36f8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f36f8-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f36f8-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f36f8-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f36f8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f36f8-134">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f36f8-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f36f8-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f36f8-135">Validation File</span></span>  <br/> |<span data-ttu-id="f36f8-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f36f8-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f36f8-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f36f8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f36f8-138">True</span><span class="sxs-lookup"><span data-stu-id="f36f8-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f36f8-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f36f8-139">See also</span></span>



[<span data-ttu-id="f36f8-140">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="f36f8-141">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="f36f8-142">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f36f8-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

