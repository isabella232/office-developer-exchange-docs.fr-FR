---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: L’élément FindMailboxStatisticsByKeywordsResponseMessage Spécifie le message de réponse pour une demande FindMailboxStatisticsByKeywords.
ms.openlocfilehash: 9479252ed53335d07a6402707bc69e5eaadfa7c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756408"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="55972-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="55972-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="55972-104">L’élément **FindMailboxStatisticsByKeywordsResponseMessage** Spécifie le message de réponse pour une demande **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="55972-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="55972-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="55972-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55972-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55972-106">Attributes and elements</span></span>

<span data-ttu-id="55972-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55972-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55972-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55972-108">Attributes</span></span>

|<span data-ttu-id="55972-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="55972-109">**Attribute**</span></span>|<span data-ttu-id="55972-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="55972-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55972-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="55972-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="55972-112">Spécifie la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="55972-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="55972-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="55972-113">ResponseClass</span></span>

|<span data-ttu-id="55972-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="55972-114">**Value**</span></span>|<span data-ttu-id="55972-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="55972-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55972-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="55972-116">Success</span></span>  <br/> |<span data-ttu-id="55972-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="55972-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="55972-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="55972-118">Warning</span></span>  <br/> |<span data-ttu-id="55972-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="55972-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="55972-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="55972-120">Error</span></span>  <br/> |<span data-ttu-id="55972-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="55972-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="55972-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55972-122">Child elements</span></span>

|<span data-ttu-id="55972-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55972-123">**Element**</span></span>|<span data-ttu-id="55972-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="55972-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55972-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="55972-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="55972-126">Spécifie le résultat d’une recherche de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="55972-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="55972-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="55972-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="55972-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="55972-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="55972-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="55972-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="55972-130">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="55972-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="55972-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="55972-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="55972-132">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="55972-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="55972-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="55972-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="55972-134">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="55972-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55972-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55972-135">Parent elements</span></span>

|<span data-ttu-id="55972-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55972-136">**Element**</span></span>|<span data-ttu-id="55972-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="55972-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55972-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="55972-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="55972-139">Spécifie un tableau de messages de réponse.</span><span class="sxs-lookup"><span data-stu-id="55972-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55972-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="55972-140">Remarks</span></span>

<span data-ttu-id="55972-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55972-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55972-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55972-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55972-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55972-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55972-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55972-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55972-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55972-145">Schema Name</span></span>  <br/> |<span data-ttu-id="55972-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="55972-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="55972-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55972-147">Validation File</span></span>  <br/> |<span data-ttu-id="55972-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="55972-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55972-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55972-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="55972-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55972-150">See also</span></span>



- [<span data-ttu-id="55972-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="55972-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

