---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: L’élément FindMailboxStatisticsByKeywordsResponseMessage spécifie le message de réponse pour une demande FindMailboxStatisticsByKeywords.
ms.openlocfilehash: 704eebbf82db2871ab36be8e5b30c88c6959baa5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525975"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="34f05-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="34f05-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="34f05-104">L’élément **FindMailboxStatisticsByKeywordsResponseMessage** spécifie le message de réponse pour une demande **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="34f05-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="34f05-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="34f05-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34f05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34f05-106">Attributes and elements</span></span>

<span data-ttu-id="34f05-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34f05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34f05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="34f05-108">Attributes</span></span>

|<span data-ttu-id="34f05-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="34f05-109">**Attribute**</span></span>|<span data-ttu-id="34f05-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="34f05-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34f05-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="34f05-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="34f05-112">Spécifie la classe Response.</span><span class="sxs-lookup"><span data-stu-id="34f05-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="34f05-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="34f05-113">ResponseClass</span></span>

|<span data-ttu-id="34f05-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="34f05-114">**Value**</span></span>|<span data-ttu-id="34f05-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="34f05-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34f05-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="34f05-116">Success</span></span>  <br/> |<span data-ttu-id="34f05-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="34f05-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="34f05-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="34f05-118">Warning</span></span>  <br/> |<span data-ttu-id="34f05-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="34f05-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="34f05-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="34f05-120">Error</span></span>  <br/> |<span data-ttu-id="34f05-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="34f05-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="34f05-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34f05-122">Child elements</span></span>

|<span data-ttu-id="34f05-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34f05-123">**Element**</span></span>|<span data-ttu-id="34f05-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="34f05-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34f05-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="34f05-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="34f05-126">Spécifie le résultat d’une recherche de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="34f05-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="34f05-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="34f05-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="34f05-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="34f05-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="34f05-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="34f05-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="34f05-130">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="34f05-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="34f05-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="34f05-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="34f05-132">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="34f05-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="34f05-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="34f05-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="34f05-134">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="34f05-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34f05-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34f05-135">Parent elements</span></span>

|<span data-ttu-id="34f05-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="34f05-136">**Element**</span></span>|<span data-ttu-id="34f05-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="34f05-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34f05-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="34f05-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="34f05-139">Spécifie un tableau de messages de réponse.</span><span class="sxs-lookup"><span data-stu-id="34f05-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34f05-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="34f05-140">Remarks</span></span>

<span data-ttu-id="34f05-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34f05-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34f05-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="34f05-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34f05-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34f05-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34f05-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34f05-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34f05-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34f05-145">Schema Name</span></span>  <br/> |<span data-ttu-id="34f05-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="34f05-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="34f05-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34f05-147">Validation File</span></span>  <br/> |<span data-ttu-id="34f05-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34f05-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34f05-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34f05-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="34f05-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="34f05-150">See also</span></span>



- [<span data-ttu-id="34f05-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="34f05-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

