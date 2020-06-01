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
description: L’élément ErrorCode représente un code d’erreur renvoyé par le service de découverte automatique.
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460091"
---
# <a name="errorcode-soap"></a><span data-ttu-id="1f203-103">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="1f203-104">L’élément **ErrorCode** représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f203-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="1f203-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="1f203-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f203-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f203-106">Attributes and elements</span></span>

<span data-ttu-id="1f203-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f203-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f203-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f203-108">Attributes</span></span>

<span data-ttu-id="1f203-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1f203-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f203-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f203-110">Child elements</span></span>

<span data-ttu-id="1f203-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1f203-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f203-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f203-112">Parent elements</span></span>

|<span data-ttu-id="1f203-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f203-113">**Element**</span></span>|<span data-ttu-id="1f203-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f203-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f203-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="1f203-116">Représente le type de base pour toutes les réponses renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f203-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1f203-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="1f203-118">Contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="1f203-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="1f203-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="1f203-120">Contient la réponse à un appel [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) pour un domaine individuel.</span><span class="sxs-lookup"><span data-stu-id="1f203-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="1f203-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="1f203-122">Contient la réponse à une demande d' [opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1f203-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1f203-123">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="1f203-124">Contient la réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="1f203-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="1f203-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="1f203-126">Représente une erreur renvoyée lors de la récupération d’un paramètre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1f203-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="1f203-127">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="1f203-128">Représente une réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="1f203-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f203-129">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1f203-129">Text value</span></span>

<span data-ttu-id="1f203-130">La valeur de texte représente le code d’erreur d’une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f203-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="1f203-131">Le tableau suivant répertorie les valeurs de texte possibles pour l’élément **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="1f203-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="1f203-132">**Valeur de texte du code d’erreur**</span><span class="sxs-lookup"><span data-stu-id="1f203-132">**Error code text value**</span></span>|<span data-ttu-id="1f203-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f203-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f203-134">NoError</span><span class="sxs-lookup"><span data-stu-id="1f203-134">NoError</span></span>  <br/> |<span data-ttu-id="1f203-135">Aucune erreur n’est survenue.</span><span class="sxs-lookup"><span data-stu-id="1f203-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="1f203-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="1f203-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="1f203-137">L’appelant doit suivre la redirection de l’adresse de messagerie qui a été renvoyée par la découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f203-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="1f203-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="1f203-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="1f203-139">L’appelant doit suivre la redirection d’URL renvoyée par la découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="1f203-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="1f203-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="1f203-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="1f203-141">L’utilisateur qui a été passé dans la demande n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="1f203-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="1f203-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="1f203-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="1f203-143">La demande n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="1f203-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="1f203-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="1f203-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="1f203-145">Un paramètre spécifié n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="1f203-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="1f203-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="1f203-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="1f203-147">Un paramètre spécifié n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="1f203-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="1f203-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="1f203-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="1f203-149">Le serveur est trop occupé pour traiter la demande.</span><span class="sxs-lookup"><span data-stu-id="1f203-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="1f203-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="1f203-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="1f203-151">Le domaine demandé n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="1f203-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="1f203-152">NotFederated</span><span class="sxs-lookup"><span data-stu-id="1f203-152">NotFederated</span></span>  <br/> |<span data-ttu-id="1f203-153">L’organisation n’est pas fédérée.</span><span class="sxs-lookup"><span data-stu-id="1f203-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="1f203-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="1f203-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="1f203-155">Erreur de serveur interne.</span><span class="sxs-lookup"><span data-stu-id="1f203-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="1f203-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f203-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f203-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f203-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1f203-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f203-158">Schema Name</span></span>  <br/> |<span data-ttu-id="1f203-159">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="1f203-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1f203-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1f203-160">Validation File</span></span>  <br/> |<span data-ttu-id="1f203-161">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1f203-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f203-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f203-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f203-163">True</span><span class="sxs-lookup"><span data-stu-id="1f203-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f203-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f203-164">See also</span></span>



[<span data-ttu-id="1f203-165">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="1f203-166">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="1f203-167">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f203-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

