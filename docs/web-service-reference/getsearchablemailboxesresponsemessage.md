---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: L’élément GetSearchableMailboxesResponseMessage spécifie le message de réponse pour une demande GetSearchableMailboxes.
ms.openlocfilehash: 69f45d87cfbd398013d021cdd39b55497d78ae04
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458256"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="29841-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29841-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="29841-104">L’élément **GetSearchableMailboxesResponseMessage** spécifie le message de réponse pour une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="29841-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="29841-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="29841-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29841-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="29841-106">Attributes and elements</span></span>

<span data-ttu-id="29841-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="29841-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29841-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="29841-108">Attributes</span></span>

|<span data-ttu-id="29841-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="29841-109">**Attribute**</span></span>|<span data-ttu-id="29841-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="29841-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29841-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="29841-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="29841-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="29841-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="29841-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="29841-113">ResponseClass</span></span>

|<span data-ttu-id="29841-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="29841-114">**Value**</span></span>|<span data-ttu-id="29841-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="29841-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="29841-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="29841-116">Success</span></span>  <br/> |<span data-ttu-id="29841-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="29841-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="29841-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="29841-118">Warning</span></span>  <br/> |<span data-ttu-id="29841-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="29841-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="29841-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="29841-120">Error</span></span>  <br/> |<span data-ttu-id="29841-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="29841-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="29841-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="29841-122">Child elements</span></span>

|<span data-ttu-id="29841-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29841-123">**Element**</span></span>|<span data-ttu-id="29841-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="29841-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29841-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="29841-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="29841-126">Contient un tableau des boîtes aux lettres retournées à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="29841-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="29841-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="29841-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="29841-128">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="29841-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="29841-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="29841-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="29841-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="29841-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="29841-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="29841-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="29841-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="29841-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="29841-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29841-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="29841-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="29841-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29841-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="29841-135">Parent elements</span></span>

|<span data-ttu-id="29841-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29841-136">**Element**</span></span>|<span data-ttu-id="29841-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="29841-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29841-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29841-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="29841-139">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="29841-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="29841-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="29841-140">Remarks</span></span>

<span data-ttu-id="29841-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="29841-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="29841-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="29841-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29841-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="29841-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29841-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="29841-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29841-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="29841-145">Schema Name</span></span>  <br/> |<span data-ttu-id="29841-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="29841-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="29841-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="29841-147">Validation File</span></span>  <br/> |<span data-ttu-id="29841-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="29841-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29841-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="29841-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="29841-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29841-150">See also</span></span>



- [<span data-ttu-id="29841-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29841-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

