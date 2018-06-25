---
title: SubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponseMessage
api_type:
- schema
ms.assetid: d121d38a-a61a-4f9c-a477-fc6d7f9af77e
description: L’élément SubscribeResponseMessage contient l’état et les résultats d’une seule demande d’opération s’abonner.
ms.openlocfilehash: 97c7bd9f12511ff226e75f53278c13481679c8a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="bd15a-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bd15a-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="bd15a-104">L’élément **SubscribeResponseMessage** contient l’état et les résultats d’une seule demande [d’opération de s’abonner](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bd15a-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="bd15a-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="bd15a-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="bd15a-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bd15a-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="bd15a-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bd15a-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
```xml
<SubscribeResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SubscriptionId/>
   <Watermark/>
</SubscribeResponseMessage>
```

 <span data-ttu-id="bd15a-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bd15a-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd15a-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd15a-109">Attributes and elements</span></span>

<span data-ttu-id="bd15a-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd15a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd15a-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd15a-111">Attributes</span></span>

|<span data-ttu-id="bd15a-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bd15a-112">**Attribute**</span></span>|<span data-ttu-id="bd15a-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd15a-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd15a-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bd15a-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bd15a-115">Décrit l’état d’une réponse de [l’opération de s’abonner](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bd15a-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="bd15a-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="bd15a-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="bd15a-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="bd15a-117">-  Success</span></span>  <br/><span data-ttu-id="bd15a-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="bd15a-118">-  Warning</span></span>  <br/><span data-ttu-id="bd15a-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="bd15a-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bd15a-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bd15a-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bd15a-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bd15a-121">**Value**</span></span>|<span data-ttu-id="bd15a-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd15a-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bd15a-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="bd15a-123">**Success**</span></span> <br/> |<span data-ttu-id="bd15a-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="bd15a-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bd15a-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="bd15a-125">**Warning**</span></span> <br/> | <span data-ttu-id="bd15a-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="bd15a-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bd15a-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="bd15a-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="bd15a-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="bd15a-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="bd15a-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="bd15a-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bd15a-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bd15a-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bd15a-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="bd15a-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bd15a-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bd15a-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bd15a-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="bd15a-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bd15a-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="bd15a-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bd15a-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="bd15a-135">**Error**</span></span> <br/> | <span data-ttu-id="bd15a-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="bd15a-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bd15a-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="bd15a-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bd15a-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="bd15a-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bd15a-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="bd15a-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="bd15a-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="bd15a-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="bd15a-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="bd15a-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="bd15a-142">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="bd15a-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bd15a-143">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="bd15a-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="bd15a-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bd15a-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bd15a-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd15a-145">Child elements</span></span>

|<span data-ttu-id="bd15a-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd15a-146">**Element**</span></span>|<span data-ttu-id="bd15a-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd15a-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd15a-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="bd15a-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bd15a-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="bd15a-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bd15a-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bd15a-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bd15a-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="bd15a-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bd15a-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bd15a-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bd15a-153">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="bd15a-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bd15a-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="bd15a-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bd15a-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bd15a-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bd15a-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="bd15a-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bd15a-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="bd15a-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="bd15a-158">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="bd15a-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="bd15a-159">Filigrane</span><span class="sxs-lookup"><span data-stu-id="bd15a-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="bd15a-160">Représente un signet d’événements dans la file d’attente des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bd15a-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd15a-161">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd15a-161">Parent elements</span></span>

|<span data-ttu-id="bd15a-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd15a-162">**Element**</span></span>|<span data-ttu-id="bd15a-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd15a-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd15a-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bd15a-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bd15a-165">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd15a-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd15a-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd15a-166">Remarks</span></span>

<span data-ttu-id="bd15a-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="bd15a-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd15a-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bd15a-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd15a-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bd15a-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd15a-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bd15a-170">Schema Name</span></span>  <br/> |<span data-ttu-id="bd15a-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bd15a-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd15a-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bd15a-172">Validation File</span></span>  <br/> |<span data-ttu-id="bd15a-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bd15a-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd15a-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bd15a-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd15a-175">False</span><span class="sxs-lookup"><span data-stu-id="bd15a-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd15a-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd15a-176">See also</span></span>

- [<span data-ttu-id="bd15a-177">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="bd15a-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="bd15a-178">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="bd15a-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="bd15a-179">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="bd15a-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

