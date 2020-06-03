---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: L’élément ApplyConversationActionResponseMessage contient l’État et les résultats d’une demande d’opération ApplyConversationAction.
ms.openlocfilehash: 377aee12d8cc7d6b4aff8d6fc2a6cb67b3bcd10b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464692"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="63425-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="63425-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="63425-104">L’élément **ApplyConversationActionResponseMessage** contient l’État et les résultats d’une demande d' [opération ApplyConversationAction](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="63425-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="63425-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="63425-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="63425-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="63425-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="63425-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="63425-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="63425-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="63425-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63425-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63425-109">Attributes and elements</span></span>

<span data-ttu-id="63425-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63425-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63425-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="63425-111">Attributes</span></span>

|<span data-ttu-id="63425-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="63425-112">**Attribute**</span></span>|<span data-ttu-id="63425-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="63425-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63425-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="63425-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="63425-115">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="63425-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="63425-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="63425-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="63425-117">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="63425-117">Success</span></span></li><li><span data-ttu-id="63425-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="63425-118">Warning</span></span></li><li><span data-ttu-id="63425-119">Erreur</span><span class="sxs-lookup"><span data-stu-id="63425-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="63425-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="63425-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="63425-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="63425-121">**Value**</span></span>|<span data-ttu-id="63425-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="63425-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63425-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="63425-123">**Success**</span></span> <br/> |<span data-ttu-id="63425-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="63425-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="63425-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="63425-125">**Warning**</span></span> <br/> | <span data-ttu-id="63425-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="63425-126">Describes a request that was not processed.</span></span> <span data-ttu-id="63425-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="63425-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="63425-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="63425-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="63425-129">La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="63425-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="63425-130">Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="63425-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="63425-131">Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="63425-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="63425-132">La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="63425-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="63425-133">Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="63425-133">A password is expired.</span></span></li><li><span data-ttu-id="63425-134">Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="63425-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="63425-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="63425-135">**Error**</span></span> <br/> | <span data-ttu-id="63425-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="63425-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="63425-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="63425-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="63425-138">Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="63425-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="63425-139">Attributs ou éléments en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="63425-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="63425-140">Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="63425-140">An unknown tag</span></span>  </li><li><span data-ttu-id="63425-141">Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="63425-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="63425-142">Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="63425-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="63425-143">Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="63425-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="63425-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="63425-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="63425-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63425-145">Child elements</span></span>

|<span data-ttu-id="63425-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63425-146">**Element**</span></span>|<span data-ttu-id="63425-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="63425-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63425-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="63425-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="63425-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="63425-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="63425-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="63425-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="63425-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="63425-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="63425-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="63425-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="63425-153">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="63425-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="63425-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="63425-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="63425-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="63425-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="63425-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="63425-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63425-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63425-157">Parent elements</span></span>

|<span data-ttu-id="63425-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63425-158">**Element**</span></span>|<span data-ttu-id="63425-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="63425-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63425-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="63425-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="63425-161">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="63425-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63425-162">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="63425-162">Text value</span></span>

<span data-ttu-id="63425-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63425-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63425-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="63425-164">Remarks</span></span>

<span data-ttu-id="63425-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="63425-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="63425-166">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="63425-166">Version differences</span></span>

<span data-ttu-id="63425-167">Dans les versions d’Exchange commençant par Build 15.00.0986.00, l’élément **ApplyConversationActionResponseMessage** est de type **ApplyConversationActionResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="63425-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="63425-168">Dans les versions antérieures, l’élément est de type **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="63425-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63425-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63425-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63425-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63425-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63425-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63425-171">Schema Name</span></span>  <br/> |<span data-ttu-id="63425-172">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="63425-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="63425-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63425-173">Validation File</span></span>  <br/> |<span data-ttu-id="63425-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63425-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63425-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63425-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="63425-176">False</span><span class="sxs-lookup"><span data-stu-id="63425-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63425-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63425-177">See also</span></span>

- [<span data-ttu-id="63425-178">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="63425-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="63425-179">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63425-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

