---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: L’élément GetAppManifestsResponseMessage Spécifie le message de réponse pour une demande GetAppManifests.
ms.openlocfilehash: 05eeef7f7194c1dc05be93ed13ebff93d5013e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756516"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="27d48-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="27d48-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="27d48-104">L’élément **GetAppManifestsResponseMessage** Spécifie le message de réponse pour une demande **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="27d48-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="27d48-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="27d48-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27d48-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="27d48-106">Attributes and elements</span></span>

<span data-ttu-id="27d48-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="27d48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27d48-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="27d48-108">Attributes</span></span>

|<span data-ttu-id="27d48-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="27d48-109">**Attribute**</span></span>|<span data-ttu-id="27d48-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="27d48-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27d48-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="27d48-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="27d48-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="27d48-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="27d48-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="27d48-113">ResponseClass</span></span>

|<span data-ttu-id="27d48-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="27d48-114">**Value**</span></span>|<span data-ttu-id="27d48-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="27d48-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27d48-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="27d48-116">Success</span></span>  <br/> |<span data-ttu-id="27d48-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="27d48-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="27d48-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="27d48-118">Warning</span></span>  <br/> |<span data-ttu-id="27d48-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="27d48-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="27d48-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="27d48-120">Error</span></span>  <br/> |<span data-ttu-id="27d48-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="27d48-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="27d48-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="27d48-122">Child elements</span></span>

|<span data-ttu-id="27d48-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="27d48-123">**Element**</span></span>|<span data-ttu-id="27d48-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="27d48-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27d48-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="27d48-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="27d48-126">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="27d48-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="27d48-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="27d48-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="27d48-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="27d48-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="27d48-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="27d48-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="27d48-130">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="27d48-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="27d48-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="27d48-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="27d48-132">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="27d48-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="27d48-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="27d48-133">Parent elements</span></span>

|<span data-ttu-id="27d48-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="27d48-134">**Element**</span></span>|<span data-ttu-id="27d48-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="27d48-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27d48-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="27d48-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="27d48-137">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="27d48-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="27d48-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="27d48-138">Remarks</span></span>

<span data-ttu-id="27d48-139">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="27d48-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="27d48-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="27d48-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27d48-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="27d48-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27d48-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="27d48-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27d48-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="27d48-143">Schema Name</span></span>  <br/> |<span data-ttu-id="27d48-144">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="27d48-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="27d48-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="27d48-145">Validation File</span></span>  <br/> |<span data-ttu-id="27d48-146">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27d48-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27d48-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="27d48-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="27d48-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="27d48-148">See also</span></span>



- [<span data-ttu-id="27d48-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="27d48-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

