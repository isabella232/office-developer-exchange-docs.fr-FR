---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: L’élément GetStreamingEventsResponseMessage contient l’État et le résultat d’une seule demande d’opération GetStreamingEvents.
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459145"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="1bf6d-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1bf6d-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="1bf6d-104">L’élément **GetStreamingEventsResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1bf6d-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 <span data-ttu-id="1bf6d-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bf6d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1bf6d-106">Attributes and elements</span></span>

<span data-ttu-id="1bf6d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bf6d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1bf6d-108">Attributes</span></span>

|<span data-ttu-id="1bf6d-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-109">**Attribute**</span></span>|<span data-ttu-id="1bf6d-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1bf6d-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1bf6d-112">Décrit l’état d’une réponse d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1bf6d-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="1bf6d-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1bf6d-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1bf6d-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1bf6d-114">-  Success</span></span>  <br/><span data-ttu-id="1bf6d-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="1bf6d-115">-  Warning</span></span>  <br/><span data-ttu-id="1bf6d-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1bf6d-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="1bf6d-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1bf6d-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="1bf6d-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-118">**Value**</span></span>|<span data-ttu-id="1bf6d-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1bf6d-120">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="1bf6d-120">Success</span></span>  <br/> |<span data-ttu-id="1bf6d-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1bf6d-122">Avertissement</span><span class="sxs-lookup"><span data-stu-id="1bf6d-122">Warning</span></span>  <br/> | <span data-ttu-id="1bf6d-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1bf6d-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1bf6d-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="1bf6d-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1bf6d-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1bf6d-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1bf6d-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1bf6d-129">-La base de données de boîtes aux lettres (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1bf6d-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="1bf6d-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="1bf6d-132">Erreur</span><span class="sxs-lookup"><span data-stu-id="1bf6d-132">Error</span></span>  <br/> | <span data-ttu-id="1bf6d-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1bf6d-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="1bf6d-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1bf6d-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="1bf6d-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1bf6d-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="1bf6d-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="1bf6d-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1bf6d-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="1bf6d-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1bf6d-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="1bf6d-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="1bf6d-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1bf6d-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="1bf6d-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1bf6d-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1bf6d-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1bf6d-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1bf6d-142">Child elements</span></span>

|<span data-ttu-id="1bf6d-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-143">**Element**</span></span>|<span data-ttu-id="1bf6d-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bf6d-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1bf6d-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1bf6d-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1bf6d-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1bf6d-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1bf6d-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1bf6d-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1bf6d-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1bf6d-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1bf6d-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-154">Notifications</span><span class="sxs-lookup"><span data-stu-id="1bf6d-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="1bf6d-155">Contient une liste d’informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="1bf6d-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="1bf6d-157">Contient une liste des ID d’abonnement qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="1bf6d-158">ConnectionStatus Closed</span><span class="sxs-lookup"><span data-stu-id="1bf6d-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="1bf6d-159">Fournit une description textuelle de l’état d’un abonnement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bf6d-160">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1bf6d-160">Parent elements</span></span>

|<span data-ttu-id="1bf6d-161">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-161">**Element**</span></span>|<span data-ttu-id="1bf6d-162">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bf6d-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bf6d-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1bf6d-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1bf6d-164">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1bf6d-165">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1bf6d-165">Text value</span></span>

<span data-ttu-id="1bf6d-166">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1bf6d-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1bf6d-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="1bf6d-167">Remarks</span></span>

<span data-ttu-id="1bf6d-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1bf6d-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bf6d-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1bf6d-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bf6d-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1bf6d-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1bf6d-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1bf6d-171">Schema Name</span></span>  <br/> |<span data-ttu-id="1bf6d-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1bf6d-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1bf6d-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1bf6d-173">Validation File</span></span>  <br/> |<span data-ttu-id="1bf6d-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1bf6d-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1bf6d-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1bf6d-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="1bf6d-176">False</span><span class="sxs-lookup"><span data-stu-id="1bf6d-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bf6d-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1bf6d-177">See also</span></span>

- [<span data-ttu-id="1bf6d-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="1bf6d-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="1bf6d-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="1bf6d-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="1bf6d-180">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="1bf6d-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

