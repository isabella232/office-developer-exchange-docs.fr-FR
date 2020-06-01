---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: L’élément ClientExtension contient les informations d’utilisateur et de configuration relatives à une application.
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460196"
---
# <a name="clientextension"></a><span data-ttu-id="d2b2e-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="d2b2e-103">ClientExtension</span></span>

<span data-ttu-id="d2b2e-104">L’élément **ClientExtension** contient les informations d’utilisateur et de configuration relatives à une application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="d2b2e-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2b2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2b2e-106">Attributes and elements</span></span>

<span data-ttu-id="d2b2e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2b2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2b2e-108">Attributes</span></span>

|<span data-ttu-id="d2b2e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-109">**Attribute**</span></span>|<span data-ttu-id="d2b2e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2b2e-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="d2b2e-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="d2b2e-112">Indique si l’application est disponible.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-112">Specifies whether the app is available.</span></span> <span data-ttu-id="d2b2e-113">Une valeur de texte de **true** pour l’attribut **IsAvailable** indique que l’application est disponible.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="d2b2e-114">La valeur **false** indique que l’application n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="d2b2e-115">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="d2b2e-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="d2b2e-117">Indique si l’application est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="d2b2e-118">Une valeur de texte de **true** pour l’attribut **IsMandatory** indique que l’application est obligatoire pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="d2b2e-119">La valeur **false** indique que l’application n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="d2b2e-120">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="d2b2e-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="d2b2e-122">Indique si l’application est activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="d2b2e-123">Une valeur de texte de **true** pour l’attribut **IsEnabledByDefault** indique que l’application est activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="d2b2e-124">La valeur **false** indique que l’application n’est pas activée par défaut.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="d2b2e-125">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="d2b2e-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="d2b2e-127">Indique à qui l’application est fournie.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="d2b2e-128">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-129">Type</span><span class="sxs-lookup"><span data-stu-id="d2b2e-129">Type</span></span>  <br/> |<span data-ttu-id="d2b2e-130">Spécifie le type de l’application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-131">Portée</span><span class="sxs-lookup"><span data-stu-id="d2b2e-131">Scope</span></span>  <br/> |<span data-ttu-id="d2b2e-132">Spécifie l’étendue de l’application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="d2b2e-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="d2b2e-134">Spécifie l’identificateur de l’élément Marketplace de l’application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="d2b2e-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="d2b2e-136">Spécifie le contenu Marketplace qu’un utilisateur voit pour obtenir des détails et des avis sur une application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="d2b2e-137">AppStatus</span></span>  <br/> |<span data-ttu-id="d2b2e-138">Spécifie le code d’état d’une application de messagerie dans un état inattendu.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="d2b2e-139">Etoken</span></span>  <br/> |<span data-ttu-id="d2b2e-140">Spécifie le jeton de licence pour les applications de messagerie payantes ou d’évaluation.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="d2b2e-141">Type</span><span class="sxs-lookup"><span data-stu-id="d2b2e-141">Type</span></span>

|<span data-ttu-id="d2b2e-142">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-142">**Value**</span></span>|<span data-ttu-id="d2b2e-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2b2e-144">Par défaut</span><span class="sxs-lookup"><span data-stu-id="d2b2e-144">Default</span></span>  <br/> |<span data-ttu-id="d2b2e-145">Indique que l’application est disponible par défaut.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-146">Private</span><span class="sxs-lookup"><span data-stu-id="d2b2e-146">Private</span></span>  <br/> |<span data-ttu-id="d2b2e-147">Indique que l’application est privée.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-148">Actuel</span><span class="sxs-lookup"><span data-stu-id="d2b2e-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="d2b2e-149">Indique que l’application est une application Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="d2b2e-150">Portée</span><span class="sxs-lookup"><span data-stu-id="d2b2e-150">Scope</span></span>

|<span data-ttu-id="d2b2e-151">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-151">**Value**</span></span>|<span data-ttu-id="d2b2e-152">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2b2e-153">Aucun</span><span class="sxs-lookup"><span data-stu-id="d2b2e-153">None</span></span>  <br/> |<span data-ttu-id="d2b2e-154">Indique que l’application n’a pas d’étendue.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-155">Utilisateur</span><span class="sxs-lookup"><span data-stu-id="d2b2e-155">User</span></span>  <br/> |<span data-ttu-id="d2b2e-156">Indique que l’application est par utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-157">Organisation</span><span class="sxs-lookup"><span data-stu-id="d2b2e-157">Organization</span></span>  <br/> |<span data-ttu-id="d2b2e-158">Indique que l’application est destinée à une organisation.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="d2b2e-159">Par défaut</span><span class="sxs-lookup"><span data-stu-id="d2b2e-159">Default</span></span>  <br/> |<span data-ttu-id="d2b2e-160">Indique que l’application est une application par défaut.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2b2e-161">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2b2e-161">Child elements</span></span>

|<span data-ttu-id="d2b2e-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-162">**Element**</span></span>|<span data-ttu-id="d2b2e-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2b2e-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="d2b2e-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="d2b2e-165">Spécifie les comptes de messagerie qui peuvent accéder à l’application.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="d2b2e-166">Manifeste</span><span class="sxs-lookup"><span data-stu-id="d2b2e-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="d2b2e-167">Contient le fichier manifeste d’application encodé en base 64.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2b2e-168">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2b2e-168">Parent elements</span></span>

|<span data-ttu-id="d2b2e-169">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-169">**Element**</span></span>|<span data-ttu-id="d2b2e-170">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2b2e-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2b2e-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="d2b2e-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="d2b2e-172">Spécifie un tableau d’éléments **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="d2b2e-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2b2e-173">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2b2e-173">Remarks</span></span>

<span data-ttu-id="d2b2e-174">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2b2e-175">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2b2e-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2b2e-176">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2b2e-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2b2e-177">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2b2e-177">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2b2e-178">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2b2e-178">Schema Name</span></span>  <br/> |<span data-ttu-id="d2b2e-179">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d2b2e-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2b2e-180">Validation File</span><span class="sxs-lookup"><span data-stu-id="d2b2e-180">Validation File</span></span>  <br/> |<span data-ttu-id="d2b2e-181">types. xsd</span><span class="sxs-lookup"><span data-stu-id="d2b2e-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2b2e-182">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2b2e-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2b2e-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2b2e-183">See also</span></span>



- [<span data-ttu-id="d2b2e-184">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2b2e-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

