---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: L’élément GetAppMarketplaceUrlResponse spécifie la réponse à une demande GetAppMarketplaceUrl.
ms.openlocfilehash: 7ff000908a2f73f41575cae8a7795644dd60565d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530852"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="7bbdb-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="7bbdb-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="7bbdb-104">L’élément **GetAppMarketplaceUrlResponse** spécifie la réponse à une demande **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="7bbdb-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="7bbdb-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bbdb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7bbdb-106">Attributes and elements</span></span>

<span data-ttu-id="7bbdb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bbdb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7bbdb-108">Attributes</span></span>

|<span data-ttu-id="7bbdb-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-109">**Attribute**</span></span>|<span data-ttu-id="7bbdb-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7bbdb-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7bbdb-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="7bbdb-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="7bbdb-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7bbdb-113">ResponseClass</span></span>

|<span data-ttu-id="7bbdb-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-114">**Value**</span></span>|<span data-ttu-id="7bbdb-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7bbdb-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="7bbdb-116">Success</span></span>  <br/> |<span data-ttu-id="7bbdb-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="7bbdb-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="7bbdb-118">Warning</span></span>  <br/> |<span data-ttu-id="7bbdb-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="7bbdb-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="7bbdb-120">Error</span></span>  <br/> |<span data-ttu-id="7bbdb-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7bbdb-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7bbdb-122">Child elements</span></span>

|<span data-ttu-id="7bbdb-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-123">**Element**</span></span>|<span data-ttu-id="7bbdb-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bbdb-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="7bbdb-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="7bbdb-126">Spécifie l’URL de l’application.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="7bbdb-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7bbdb-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7bbdb-128">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="7bbdb-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="7bbdb-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7bbdb-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7bbdb-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7bbdb-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7bbdb-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7bbdb-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7bbdb-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7bbdb-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7bbdb-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7bbdb-135">Parent elements</span></span>

|<span data-ttu-id="7bbdb-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-136">**Element**</span></span>|<span data-ttu-id="7bbdb-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="7bbdb-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bbdb-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7bbdb-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7bbdb-139">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7bbdb-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="7bbdb-140">Remarks</span></span>

<span data-ttu-id="7bbdb-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7bbdb-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bbdb-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bbdb-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7bbdb-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bbdb-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7bbdb-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7bbdb-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7bbdb-145">Schema Name</span></span>  <br/> |<span data-ttu-id="7bbdb-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="7bbdb-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="7bbdb-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7bbdb-147">Validation File</span></span>  <br/> |<span data-ttu-id="7bbdb-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7bbdb-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7bbdb-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7bbdb-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7bbdb-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7bbdb-150">See also</span></span>



- [<span data-ttu-id="7bbdb-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bbdb-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

