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
description: L’élément GetStreamingEventsResponseMessage contient l’état et les résultats d’une demande d’opération GetStreamingEvents unique.
ms.openlocfilehash: 5fcc7ddde41b49a5d8b304da0732f4472c61a76a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827682"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="22184-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="22184-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="22184-104">L’élément **GetStreamingEventsResponseMessage** contient l’état et les résultats d’une seule demande [d’opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="22184-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="22184-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="22184-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22184-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22184-106">Attributes and elements</span></span>

<span data-ttu-id="22184-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22184-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22184-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22184-108">Attributes</span></span>

|<span data-ttu-id="22184-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="22184-109">**Attribute**</span></span>|<span data-ttu-id="22184-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="22184-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22184-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="22184-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="22184-112">Décrit l’état d’une réponse de [l’opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="22184-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="22184-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="22184-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="22184-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="22184-114">-  Success</span></span>  <br/><span data-ttu-id="22184-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="22184-115">-  Warning</span></span>  <br/><span data-ttu-id="22184-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="22184-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="22184-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="22184-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="22184-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="22184-118">**Value**</span></span>|<span data-ttu-id="22184-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="22184-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22184-120">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="22184-120">Success</span></span>  <br/> |<span data-ttu-id="22184-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="22184-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="22184-122">Avertissement</span><span class="sxs-lookup"><span data-stu-id="22184-122">Warning</span></span>  <br/> | <span data-ttu-id="22184-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="22184-123">Describes a request that was not processed.</span></span> <span data-ttu-id="22184-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="22184-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="22184-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="22184-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="22184-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="22184-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="22184-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="22184-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="22184-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="22184-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="22184-129">-La base de données de boîtes aux lettres (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="22184-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="22184-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="22184-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="22184-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="22184-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="22184-132">Erreur</span><span class="sxs-lookup"><span data-stu-id="22184-132">Error</span></span>  <br/> | <span data-ttu-id="22184-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="22184-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="22184-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="22184-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="22184-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="22184-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="22184-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="22184-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="22184-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="22184-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="22184-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="22184-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="22184-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="22184-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="22184-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="22184-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="22184-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="22184-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22184-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22184-142">Child elements</span></span>

|<span data-ttu-id="22184-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22184-143">**Element**</span></span>|<span data-ttu-id="22184-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="22184-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22184-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="22184-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="22184-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="22184-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="22184-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="22184-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="22184-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="22184-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="22184-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="22184-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="22184-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="22184-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="22184-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="22184-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="22184-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="22184-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="22184-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="22184-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="22184-154">Notifications</span><span class="sxs-lookup"><span data-stu-id="22184-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="22184-155">Contient une liste d’informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="22184-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="22184-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="22184-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="22184-157">Contient une liste d’abonnement à un ID qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="22184-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="22184-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="22184-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="22184-159">Fournit une description textuelle de l’état d’un abonnement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="22184-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22184-160">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22184-160">Parent elements</span></span>

|<span data-ttu-id="22184-161">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22184-161">**Element**</span></span>|<span data-ttu-id="22184-162">**Description**</span><span class="sxs-lookup"><span data-stu-id="22184-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22184-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="22184-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="22184-164">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="22184-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22184-165">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="22184-165">Text value</span></span>

<span data-ttu-id="22184-166">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22184-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22184-167">Remarques</span><span class="sxs-lookup"><span data-stu-id="22184-167">Remarks</span></span>

<span data-ttu-id="22184-168">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="22184-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22184-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22184-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22184-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22184-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22184-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22184-171">Schema Name</span></span>  <br/> |<span data-ttu-id="22184-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="22184-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22184-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22184-173">Validation File</span></span>  <br/> |<span data-ttu-id="22184-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22184-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22184-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22184-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="22184-176">False</span><span class="sxs-lookup"><span data-stu-id="22184-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22184-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22184-177">See also</span></span>

- [<span data-ttu-id="22184-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="22184-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="22184-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="22184-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="22184-180">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="22184-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

