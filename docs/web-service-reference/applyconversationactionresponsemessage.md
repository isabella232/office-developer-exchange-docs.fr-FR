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
description: L’élément ApplyConversationActionResponseMessage contient l’état et les résultats d’une requête d’opération ApplyConversationAction.
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755298"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="ffaf4-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ffaf4-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="ffaf4-104">L’élément **ApplyConversationActionResponseMessage** contient l’état et les résultats d’une requête [d’opération ApplyConversationAction](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ffaf4-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="ffaf4-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="ffaf4-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="ffaf4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffaf4-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ffaf4-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ffaf4-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="ffaf4-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffaf4-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ffaf4-109">Attributes and elements</span></span>

<span data-ttu-id="ffaf4-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffaf4-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ffaf4-111">Attributes</span></span>

|<span data-ttu-id="ffaf4-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-112">**Attribute**</span></span>|<span data-ttu-id="ffaf4-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffaf4-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ffaf4-115">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="ffaf4-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="ffaf4-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="ffaf4-117">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="ffaf4-117">Success</span></span></li><li><span data-ttu-id="ffaf4-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="ffaf4-118">Warning</span></span></li><li><span data-ttu-id="ffaf4-119">Erreur</span><span class="sxs-lookup"><span data-stu-id="ffaf4-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ffaf4-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ffaf4-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="ffaf4-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-121">**Value**</span></span>|<span data-ttu-id="ffaf4-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffaf4-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-123">**Success**</span></span> <br/> |<span data-ttu-id="ffaf4-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ffaf4-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-125">**Warning**</span></span> <br/> | <span data-ttu-id="ffaf4-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ffaf4-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="ffaf4-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="ffaf4-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="ffaf4-129">La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="ffaf4-130">Services de domaine Active Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="ffaf4-131">Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="ffaf4-132">La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="ffaf4-133">Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-133">A password is expired.</span></span></li><li><span data-ttu-id="ffaf4-134">Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="ffaf4-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-135">**Error**</span></span> <br/> | <span data-ttu-id="ffaf4-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="ffaf4-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="ffaf4-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="ffaf4-138">Attributs non valides ou des éléments</span><span class="sxs-lookup"><span data-stu-id="ffaf4-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="ffaf4-139">Attributs ou éléments qui sont hors de portée</span><span class="sxs-lookup"><span data-stu-id="ffaf4-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="ffaf4-140">Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="ffaf4-140">An unknown tag</span></span>  </li><li><span data-ttu-id="ffaf4-141">Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="ffaf4-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="ffaf4-142">Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="ffaf4-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="ffaf4-143">Une défaillance côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="ffaf4-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="ffaf4-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ffaf4-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ffaf4-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ffaf4-145">Child elements</span></span>

|<span data-ttu-id="ffaf4-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-146">**Element**</span></span>|<span data-ttu-id="ffaf4-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffaf4-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ffaf4-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ffaf4-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ffaf4-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ffaf4-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ffaf4-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ffaf4-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ffaf4-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ffaf4-153">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="ffaf4-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ffaf4-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ffaf4-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ffaf4-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffaf4-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ffaf4-157">Parent elements</span></span>

|<span data-ttu-id="ffaf4-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-158">**Element**</span></span>|<span data-ttu-id="ffaf4-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffaf4-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffaf4-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffaf4-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ffaf4-161">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ffaf4-162">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ffaf4-162">Text value</span></span>

<span data-ttu-id="ffaf4-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffaf4-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="ffaf4-164">Remarks</span></span>

<span data-ttu-id="ffaf4-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ffaf4-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="ffaf4-166">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="ffaf4-166">Version differences</span></span>

<span data-ttu-id="ffaf4-167">Dans les versions d’Exchange commençant par version 15.00.0986.00, l’élément **ApplyConversationActionResponseMessage** est de type **ApplyConversationActionResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="ffaf4-168">Dans les versions précédentes, l’élément est de type **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="ffaf4-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffaf4-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ffaf4-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffaf4-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ffaf4-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffaf4-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ffaf4-171">Schema Name</span></span>  <br/> |<span data-ttu-id="ffaf4-172">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="ffaf4-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="ffaf4-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ffaf4-173">Validation File</span></span>  <br/> |<span data-ttu-id="ffaf4-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ffaf4-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffaf4-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ffaf4-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffaf4-176">False</span><span class="sxs-lookup"><span data-stu-id="ffaf4-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffaf4-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffaf4-177">See also</span></span>

- [<span data-ttu-id="ffaf4-178">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ffaf4-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="ffaf4-179">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ffaf4-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

