---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: L’élément ErrorCode représente un code d’erreur retourné par le service de découverte automatique.
ms.openlocfilehash: 2dd91cec4645325c02bc8588af0ee0547909b945
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756204"
---
# <a name="errorcode-soap"></a><span data-ttu-id="b781c-103">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="b781c-104">L’élément **ErrorCode** représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="b781c-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="b781c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="b781c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b781c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b781c-106">Attributes and elements</span></span>

<span data-ttu-id="b781c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b781c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b781c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b781c-108">Attributes</span></span>

<span data-ttu-id="b781c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b781c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b781c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b781c-110">Child elements</span></span>

<span data-ttu-id="b781c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b781c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b781c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b781c-112">Parent elements</span></span>

|<span data-ttu-id="b781c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b781c-113">**Element**</span></span>|<span data-ttu-id="b781c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b781c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b781c-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="b781c-116">Représente le type de base pour toutes les réponses sont renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="b781c-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b781c-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="b781c-118">Contient les paramètres requis pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="b781c-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="b781c-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="b781c-120">Contient la réponse à un appel de [l’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine spécifique.</span><span class="sxs-lookup"><span data-stu-id="b781c-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="b781c-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="b781c-122">Contient la réponse à une demande [d’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="b781c-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b781c-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="b781c-124">Contient la réponse à une demande [d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="b781c-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="b781c-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="b781c-126">Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b781c-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="b781c-127">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="b781c-128">Représente une réponse à une demande de [l’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="b781c-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b781c-129">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b781c-129">Text value</span></span>

<span data-ttu-id="b781c-130">La valeur de texte représente le code d’erreur pour une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="b781c-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="b781c-131">Le tableau suivant répertorie les valeurs de texte possibles pour l’élément de **code d’erreur** .</span><span class="sxs-lookup"><span data-stu-id="b781c-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="b781c-132">**Valeur texte code d’erreur**</span><span class="sxs-lookup"><span data-stu-id="b781c-132">**Error code text value**</span></span>|<span data-ttu-id="b781c-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="b781c-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b781c-134">NoError</span><span class="sxs-lookup"><span data-stu-id="b781c-134">NoError</span></span>  <br/> |<span data-ttu-id="b781c-135">Aucune erreur s’est produite.</span><span class="sxs-lookup"><span data-stu-id="b781c-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="b781c-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="b781c-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="b781c-137">L’appelant doit suivre la redirection d’adresse de messagerie qui a été renvoyée par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="b781c-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="b781c-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="b781c-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="b781c-139">L’appelant doit suivre la redirection d’URL qui a été renvoyée par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="b781c-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="b781c-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="b781c-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="b781c-141">L’utilisateur qui a été passée dans la demande n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b781c-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="b781c-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="b781c-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="b781c-143">La demande n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b781c-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="b781c-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="b781c-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="b781c-145">Un paramètre spécifié n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b781c-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="b781c-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="b781c-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="b781c-147">Un paramètre spécifié n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="b781c-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="b781c-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="b781c-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="b781c-149">Le serveur est trop occupé pour traiter la demande.</span><span class="sxs-lookup"><span data-stu-id="b781c-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="b781c-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="b781c-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="b781c-151">Le domaine demandé n’est pas valid.</span><span class="sxs-lookup"><span data-stu-id="b781c-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="b781c-152">NotFederated</span><span class="sxs-lookup"><span data-stu-id="b781c-152">NotFederated</span></span>  <br/> |<span data-ttu-id="b781c-153">L’organisation n’est pas fédérée.</span><span class="sxs-lookup"><span data-stu-id="b781c-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="b781c-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="b781c-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="b781c-155">Il existe une erreur serveur interne.</span><span class="sxs-lookup"><span data-stu-id="b781c-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="b781c-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b781c-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b781c-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b781c-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b781c-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b781c-158">Schema Name</span></span>  <br/> |<span data-ttu-id="b781c-159">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b781c-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b781c-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b781c-160">Validation File</span></span>  <br/> |<span data-ttu-id="b781c-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b781c-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b781c-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b781c-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="b781c-163">True</span><span class="sxs-lookup"><span data-stu-id="b781c-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b781c-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b781c-164">See also</span></span>



[<span data-ttu-id="b781c-165">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="b781c-166">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="b781c-167">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b781c-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

