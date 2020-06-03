---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: L’élément SendNotificationResponseMessage contient l’État et le résultat d’une seule demande d’opération SendNotification.
ms.openlocfilehash: cf44a09624d1b8a7341f9dd98db48472fea7393b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462107"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="ba302-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ba302-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="ba302-104">L’élément **SendNotificationResponseMessage** contient l’État et le résultat d’une seule demande d’opération **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="ba302-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="ba302-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ba302-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba302-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba302-106">Attributes and elements</span></span>

<span data-ttu-id="ba302-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba302-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba302-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba302-108">Attributes</span></span>

|<span data-ttu-id="ba302-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ba302-109">**Attribute**</span></span>|<span data-ttu-id="ba302-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba302-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba302-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ba302-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ba302-112">Décrit l’état d’une réponse d’opération **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="ba302-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="ba302-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="ba302-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="ba302-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="ba302-114">-  Success</span></span>  <br/><span data-ttu-id="ba302-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="ba302-115">-  Warning</span></span>  <br/><span data-ttu-id="ba302-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="ba302-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="ba302-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ba302-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="ba302-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ba302-118">**Value**</span></span>|<span data-ttu-id="ba302-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba302-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba302-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="ba302-120">**Success**</span></span> <br/> |<span data-ttu-id="ba302-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="ba302-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ba302-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ba302-122">**Warning**</span></span> <br/> | <span data-ttu-id="ba302-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="ba302-123">Describes a request that was not processed.</span></span> <span data-ttu-id="ba302-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="ba302-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="ba302-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="ba302-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ba302-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="ba302-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ba302-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ba302-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ba302-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="ba302-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="ba302-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ba302-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ba302-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="ba302-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="ba302-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="ba302-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="ba302-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="ba302-132">**Error**</span></span> <br/> | <span data-ttu-id="ba302-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="ba302-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ba302-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="ba302-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ba302-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="ba302-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ba302-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="ba302-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="ba302-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="ba302-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="ba302-138">-Attribut ou élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="ba302-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ba302-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="ba302-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ba302-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="ba302-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ba302-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ba302-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ba302-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba302-142">Child elements</span></span>

|<span data-ttu-id="ba302-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba302-143">**Element**</span></span>|<span data-ttu-id="ba302-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba302-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba302-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="ba302-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ba302-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ba302-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ba302-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ba302-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ba302-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="ba302-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ba302-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ba302-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ba302-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="ba302-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ba302-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="ba302-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ba302-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ba302-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ba302-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="ba302-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ba302-154">Notification</span><span class="sxs-lookup"><span data-stu-id="ba302-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ba302-155">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="ba302-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba302-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba302-156">Parent elements</span></span>

|<span data-ttu-id="ba302-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba302-157">**Element**</span></span>|<span data-ttu-id="ba302-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba302-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba302-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ba302-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ba302-160">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba302-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba302-161">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ba302-161">Text value</span></span>

<span data-ttu-id="ba302-162">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba302-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba302-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba302-163">Remarks</span></span>

<span data-ttu-id="ba302-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba302-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba302-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba302-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba302-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba302-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ba302-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba302-167">Schema Name</span></span>  <br/> |<span data-ttu-id="ba302-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ba302-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ba302-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba302-169">Validation File</span></span>  <br/> |<span data-ttu-id="ba302-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ba302-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ba302-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba302-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba302-172">False</span><span class="sxs-lookup"><span data-stu-id="ba302-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba302-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba302-173">See also</span></span>

- [<span data-ttu-id="ba302-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="ba302-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="ba302-175">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ba302-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="ba302-176">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ba302-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

