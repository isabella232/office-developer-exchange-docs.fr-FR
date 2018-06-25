---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: L’élément ClientExtension contient des informations utilisateur et de configuration sur une application.
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755510"
---
# <a name="clientextension"></a><span data-ttu-id="a62b6-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="a62b6-103">ClientExtension</span></span>

<span data-ttu-id="a62b6-104">L’élément **ClientExtension** contient des informations utilisateur et de configuration sur une application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="a62b6-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="a62b6-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a62b6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a62b6-106">Attributes and elements</span></span>

<span data-ttu-id="a62b6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a62b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a62b6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a62b6-108">Attributes</span></span>

|<span data-ttu-id="a62b6-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a62b6-109">**Attribute**</span></span>|<span data-ttu-id="a62b6-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62b6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a62b6-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="a62b6-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="a62b6-112">Spécifie si l’application est disponible.</span><span class="sxs-lookup"><span data-stu-id="a62b6-112">Specifies whether the app is available.</span></span> <span data-ttu-id="a62b6-113">Une valeur de texte de **la valeur true** pour l’attribut **IsAvailable** indique que l’application est disponible.</span><span class="sxs-lookup"><span data-stu-id="a62b6-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="a62b6-114">La valeur **false** indique que l’application n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="a62b6-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="a62b6-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a62b6-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a62b6-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="a62b6-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="a62b6-117">Spécifie si l’application est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a62b6-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="a62b6-118">Une valeur de texte de **la valeur true** pour l’attribut **IsMandatory** indique que l’application est obligatoire pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a62b6-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="a62b6-119">La valeur **false** indique que l’application n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="a62b6-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="a62b6-120">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a62b6-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a62b6-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="a62b6-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="a62b6-122">Spécifie si l’application est activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="a62b6-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="a62b6-123">Une valeur de texte de **la valeur true** pour l’attribut **IsEnabledByDefault** indique que l’application est activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="a62b6-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="a62b6-124">La valeur **false** indique que l’application n’est pas activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="a62b6-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="a62b6-125">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a62b6-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a62b6-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="a62b6-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="a62b6-127">Spécifie l’emplacement auquel l’application est fournie.</span><span class="sxs-lookup"><span data-stu-id="a62b6-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="a62b6-128">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a62b6-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="a62b6-129">Type</span><span class="sxs-lookup"><span data-stu-id="a62b6-129">Type</span></span>  <br/> |<span data-ttu-id="a62b6-130">Spécifie le type de l’application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="a62b6-131">Domaine d’application</span><span class="sxs-lookup"><span data-stu-id="a62b6-131">Scope</span></span>  <br/> |<span data-ttu-id="a62b6-132">Spécifie l’étendue de l’application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="a62b6-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="a62b6-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="a62b6-134">Spécifie l’identificateur de biens marketplace de l’application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="a62b6-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="a62b6-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="a62b6-136">Spécifie le contenu de site marketplace que l’utilisateur voit pour plus d’informations et passe en revue sur une application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="a62b6-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="a62b6-137">AppStatus</span></span>  <br/> |<span data-ttu-id="a62b6-138">Spécifie le code d’état d’une application de messagerie dans un état inattendu.</span><span class="sxs-lookup"><span data-stu-id="a62b6-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="a62b6-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="a62b6-139">Etoken</span></span>  <br/> |<span data-ttu-id="a62b6-140">Spécifie le jeton de licence pour les applications de messagerie payantes ou d’évaluation.</span><span class="sxs-lookup"><span data-stu-id="a62b6-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="a62b6-141">Type</span><span class="sxs-lookup"><span data-stu-id="a62b6-141">Type</span></span>

|<span data-ttu-id="a62b6-142">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a62b6-142">**Value**</span></span>|<span data-ttu-id="a62b6-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62b6-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a62b6-144">Default (Défaut)</span><span class="sxs-lookup"><span data-stu-id="a62b6-144">Default</span></span>  <br/> |<span data-ttu-id="a62b6-145">Indique que l’application est disponible par défaut.</span><span class="sxs-lookup"><span data-stu-id="a62b6-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="a62b6-146">Private</span><span class="sxs-lookup"><span data-stu-id="a62b6-146">Private</span></span>  <br/> |<span data-ttu-id="a62b6-147">Indique que l’application est privée.</span><span class="sxs-lookup"><span data-stu-id="a62b6-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="a62b6-148">Site marketPlace</span><span class="sxs-lookup"><span data-stu-id="a62b6-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="a62b6-149">Indique que l’application est une application marketplace.</span><span class="sxs-lookup"><span data-stu-id="a62b6-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="a62b6-150">Domaine d’application</span><span class="sxs-lookup"><span data-stu-id="a62b6-150">Scope</span></span>

|<span data-ttu-id="a62b6-151">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a62b6-151">**Value**</span></span>|<span data-ttu-id="a62b6-152">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62b6-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a62b6-153">None</span><span class="sxs-lookup"><span data-stu-id="a62b6-153">None</span></span>  <br/> |<span data-ttu-id="a62b6-154">Indique ne qu’aucune étendue de l’application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="a62b6-155">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="a62b6-155">User</span></span>  <br/> |<span data-ttu-id="a62b6-156">Indique que l’application est par utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a62b6-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="a62b6-157">Organisation</span><span class="sxs-lookup"><span data-stu-id="a62b6-157">Organization</span></span>  <br/> |<span data-ttu-id="a62b6-158">Indique que l’application est pour une organisation.</span><span class="sxs-lookup"><span data-stu-id="a62b6-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="a62b6-159">Default (Défaut)</span><span class="sxs-lookup"><span data-stu-id="a62b6-159">Default</span></span>  <br/> |<span data-ttu-id="a62b6-160">Indique que l’application est une application par défaut.</span><span class="sxs-lookup"><span data-stu-id="a62b6-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a62b6-161">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a62b6-161">Child elements</span></span>

|<span data-ttu-id="a62b6-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a62b6-162">**Element**</span></span>|<span data-ttu-id="a62b6-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62b6-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a62b6-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="a62b6-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="a62b6-165">Spécifie les comptes de messagerie qui peuvent accéder à l’application.</span><span class="sxs-lookup"><span data-stu-id="a62b6-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="a62b6-166">Manifeste</span><span class="sxs-lookup"><span data-stu-id="a62b6-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="a62b6-167">Contient le fichier de manifeste d’application codée en base 64.</span><span class="sxs-lookup"><span data-stu-id="a62b6-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a62b6-168">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a62b6-168">Parent elements</span></span>

|<span data-ttu-id="a62b6-169">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a62b6-169">**Element**</span></span>|<span data-ttu-id="a62b6-170">**Description**</span><span class="sxs-lookup"><span data-stu-id="a62b6-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a62b6-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="a62b6-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="a62b6-172">Spécifie un tableau d’éléments **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="a62b6-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a62b6-173">Remarques</span><span class="sxs-lookup"><span data-stu-id="a62b6-173">Remarks</span></span>

<span data-ttu-id="a62b6-174">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a62b6-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a62b6-175">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a62b6-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a62b6-176">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a62b6-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a62b6-177">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a62b6-177">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a62b6-178">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a62b6-178">Schema Name</span></span>  <br/> |<span data-ttu-id="a62b6-179">Schéma type</span><span class="sxs-lookup"><span data-stu-id="a62b6-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="a62b6-180">Validation File</span><span class="sxs-lookup"><span data-stu-id="a62b6-180">Validation File</span></span>  <br/> |<span data-ttu-id="a62b6-181">types.xsd</span><span class="sxs-lookup"><span data-stu-id="a62b6-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a62b6-182">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a62b6-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a62b6-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a62b6-183">See also</span></span>



- [<span data-ttu-id="a62b6-184">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a62b6-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

