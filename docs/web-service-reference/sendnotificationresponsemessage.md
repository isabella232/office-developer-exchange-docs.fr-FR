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
description: L’élément SendNotificationResponseMessage contient l’état et les résultats d’une demande d’opération SendNotification unique.
ms.openlocfilehash: 49677b6d61f525b469679ec3fdcb8aadcca7239d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19829348"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="d4c48-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d4c48-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="d4c48-104">L’élément **SendNotificationResponseMessage** contient l’état et les résultats d’une demande d’opération **SendNotification** unique.</span><span class="sxs-lookup"><span data-stu-id="d4c48-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="d4c48-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d4c48-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4c48-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4c48-106">Attributes and elements</span></span>

<span data-ttu-id="d4c48-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4c48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4c48-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4c48-108">Attributes</span></span>

|<span data-ttu-id="d4c48-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d4c48-109">**Attribute**</span></span>|<span data-ttu-id="d4c48-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4c48-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4c48-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d4c48-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d4c48-112">Décrit l’état d’une réponse d’opération **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="d4c48-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="d4c48-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="d4c48-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d4c48-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="d4c48-114">-  Success</span></span>  <br/><span data-ttu-id="d4c48-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="d4c48-115">-  Warning</span></span>  <br/><span data-ttu-id="d4c48-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="d4c48-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="d4c48-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d4c48-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="d4c48-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d4c48-118">**Value**</span></span>|<span data-ttu-id="d4c48-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4c48-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4c48-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="d4c48-120">**Success**</span></span> <br/> |<span data-ttu-id="d4c48-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="d4c48-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d4c48-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="d4c48-122">**Warning**</span></span> <br/> | <span data-ttu-id="d4c48-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="d4c48-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d4c48-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="d4c48-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="d4c48-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="d4c48-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d4c48-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="d4c48-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d4c48-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d4c48-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d4c48-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="d4c48-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d4c48-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d4c48-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d4c48-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="d4c48-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="d4c48-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="d4c48-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="d4c48-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="d4c48-132">**Error**</span></span> <br/> | <span data-ttu-id="d4c48-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="d4c48-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d4c48-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="d4c48-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d4c48-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="d4c48-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d4c48-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="d4c48-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d4c48-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="d4c48-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d4c48-138">-Attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="d4c48-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d4c48-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="d4c48-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d4c48-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="d4c48-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d4c48-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d4c48-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4c48-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4c48-142">Child elements</span></span>

|<span data-ttu-id="d4c48-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4c48-143">**Element**</span></span>|<span data-ttu-id="d4c48-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4c48-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4c48-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d4c48-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d4c48-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4c48-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d4c48-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4c48-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d4c48-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="d4c48-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d4c48-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d4c48-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d4c48-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="d4c48-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d4c48-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="d4c48-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d4c48-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d4c48-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d4c48-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="d4c48-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d4c48-154">Notification</span><span class="sxs-lookup"><span data-stu-id="d4c48-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d4c48-155">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="d4c48-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4c48-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4c48-156">Parent elements</span></span>

|<span data-ttu-id="d4c48-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4c48-157">**Element**</span></span>|<span data-ttu-id="d4c48-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4c48-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4c48-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d4c48-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d4c48-160">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4c48-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4c48-161">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d4c48-161">Text value</span></span>

<span data-ttu-id="d4c48-162">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4c48-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4c48-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4c48-163">Remarks</span></span>

<span data-ttu-id="d4c48-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4c48-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4c48-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4c48-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4c48-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4c48-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4c48-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4c48-167">Schema Name</span></span>  <br/> |<span data-ttu-id="d4c48-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d4c48-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4c48-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4c48-169">Validation File</span></span>  <br/> |<span data-ttu-id="d4c48-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4c48-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4c48-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4c48-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4c48-172">False</span><span class="sxs-lookup"><span data-stu-id="d4c48-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4c48-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4c48-173">See also</span></span>

- [<span data-ttu-id="d4c48-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="d4c48-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="d4c48-175">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d4c48-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="d4c48-176">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d4c48-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

