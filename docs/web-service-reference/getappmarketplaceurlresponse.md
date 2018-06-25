---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: L’élément GetAppMarketplaceUrlResponse spécifie la réponse à une demande de GetAppMarketplaceUrl.
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756518"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="e27fa-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="e27fa-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="e27fa-104">L’élément **GetAppMarketplaceUrlResponse** spécifie la réponse à une demande de **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="e27fa-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="e27fa-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e27fa-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e27fa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e27fa-106">Attributes and elements</span></span>

<span data-ttu-id="e27fa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e27fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e27fa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e27fa-108">Attributes</span></span>

|<span data-ttu-id="e27fa-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e27fa-109">**Attribute**</span></span>|<span data-ttu-id="e27fa-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e27fa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e27fa-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e27fa-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e27fa-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e27fa-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e27fa-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e27fa-113">ResponseClass</span></span>

|<span data-ttu-id="e27fa-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e27fa-114">**Value**</span></span>|<span data-ttu-id="e27fa-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="e27fa-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e27fa-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="e27fa-116">Success</span></span>  <br/> |<span data-ttu-id="e27fa-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="e27fa-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e27fa-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="e27fa-118">Warning</span></span>  <br/> |<span data-ttu-id="e27fa-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="e27fa-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e27fa-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="e27fa-120">Error</span></span>  <br/> |<span data-ttu-id="e27fa-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="e27fa-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e27fa-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e27fa-122">Child elements</span></span>

|<span data-ttu-id="e27fa-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e27fa-123">**Element**</span></span>|<span data-ttu-id="e27fa-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="e27fa-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e27fa-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="e27fa-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="e27fa-126">Spécifie l’URL de l’application.</span><span class="sxs-lookup"><span data-stu-id="e27fa-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="e27fa-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e27fa-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e27fa-128">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="e27fa-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e27fa-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="e27fa-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e27fa-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e27fa-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e27fa-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e27fa-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e27fa-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="e27fa-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e27fa-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e27fa-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e27fa-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="e27fa-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e27fa-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e27fa-135">Parent elements</span></span>

|<span data-ttu-id="e27fa-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e27fa-136">**Element**</span></span>|<span data-ttu-id="e27fa-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="e27fa-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e27fa-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e27fa-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e27fa-139">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e27fa-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e27fa-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="e27fa-140">Remarks</span></span>

<span data-ttu-id="e27fa-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e27fa-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e27fa-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e27fa-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e27fa-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e27fa-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e27fa-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e27fa-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e27fa-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e27fa-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e27fa-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="e27fa-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e27fa-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e27fa-147">Validation File</span></span>  <br/> |<span data-ttu-id="e27fa-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e27fa-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e27fa-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e27fa-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e27fa-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e27fa-150">See also</span></span>



- [<span data-ttu-id="e27fa-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e27fa-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

