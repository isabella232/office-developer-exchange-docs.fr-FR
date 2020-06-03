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
description: L’élément SubscribeResponseMessage contient l’État et le résultat d’une demande d’opération subscribe unique.
ms.openlocfilehash: eea7356dbcf1887383d56e40a4f6dcd091535fa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465372"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="f1030-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f1030-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="f1030-104">L’élément **SubscribeResponseMessage** contient l’État et le résultat d’une demande d' [opération subscribe](subscribe-operation.md) unique.</span><span class="sxs-lookup"><span data-stu-id="f1030-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f1030-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="f1030-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="f1030-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f1030-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="f1030-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f1030-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="f1030-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f1030-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1030-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1030-109">Attributes and elements</span></span>

<span data-ttu-id="f1030-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1030-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1030-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1030-111">Attributes</span></span>

|<span data-ttu-id="f1030-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f1030-112">**Attribute**</span></span>|<span data-ttu-id="f1030-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1030-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1030-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f1030-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f1030-115">Décrit l’état d’une réponse de l' [opération subscribe](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f1030-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="f1030-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f1030-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f1030-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f1030-117">-  Success</span></span>  <br/><span data-ttu-id="f1030-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="f1030-118">-  Warning</span></span>  <br/><span data-ttu-id="f1030-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f1030-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f1030-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f1030-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f1030-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f1030-121">**Value**</span></span>|<span data-ttu-id="f1030-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1030-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1030-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f1030-123">**Success**</span></span> <br/> |<span data-ttu-id="f1030-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f1030-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f1030-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f1030-125">**Warning**</span></span> <br/> | <span data-ttu-id="f1030-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="f1030-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f1030-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="f1030-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f1030-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f1030-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f1030-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f1030-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f1030-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f1030-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f1030-131">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="f1030-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f1030-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f1030-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f1030-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f1030-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f1030-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="f1030-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f1030-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f1030-135">**Error**</span></span> <br/> | <span data-ttu-id="f1030-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f1030-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f1030-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f1030-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f1030-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="f1030-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f1030-139">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="f1030-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f1030-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f1030-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="f1030-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f1030-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f1030-142">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="f1030-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f1030-143">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="f1030-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f1030-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f1030-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f1030-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1030-145">Child elements</span></span>

|<span data-ttu-id="f1030-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1030-146">**Element**</span></span>|<span data-ttu-id="f1030-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1030-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1030-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="f1030-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f1030-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f1030-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f1030-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f1030-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f1030-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="f1030-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f1030-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f1030-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f1030-153">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f1030-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f1030-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f1030-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f1030-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f1030-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f1030-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="f1030-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f1030-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="f1030-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="f1030-158">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="f1030-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="f1030-159">Watermark</span><span class="sxs-lookup"><span data-stu-id="f1030-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="f1030-160">Représente un signet d’événement dans la file d’attente d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1030-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1030-161">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1030-161">Parent elements</span></span>

|<span data-ttu-id="f1030-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1030-162">**Element**</span></span>|<span data-ttu-id="f1030-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1030-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1030-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f1030-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f1030-165">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1030-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1030-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1030-166">Remarks</span></span>

<span data-ttu-id="f1030-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f1030-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1030-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1030-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1030-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1030-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1030-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1030-170">Schema Name</span></span>  <br/> |<span data-ttu-id="f1030-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f1030-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1030-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1030-172">Validation File</span></span>  <br/> |<span data-ttu-id="f1030-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1030-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1030-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1030-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1030-175">False</span><span class="sxs-lookup"><span data-stu-id="f1030-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1030-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1030-176">See also</span></span>

- [<span data-ttu-id="f1030-177">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="f1030-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="f1030-178">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="f1030-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="f1030-179">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="f1030-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

