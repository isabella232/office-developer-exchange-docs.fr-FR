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
ms.lasthandoff: 06/15/2018
ms.locfileid: "19829348"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="8acb8-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8acb8-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="8acb8-104">L’élément **SendNotificationResponseMessage** contient l’état et les résultats d’une demande d’opération **SendNotification** unique.</span><span class="sxs-lookup"><span data-stu-id="8acb8-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="8acb8-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8acb8-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8acb8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8acb8-106">Attributes and elements</span></span>

<span data-ttu-id="8acb8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8acb8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8acb8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8acb8-108">Attributes</span></span>

|<span data-ttu-id="8acb8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8acb8-109">**Attribute**</span></span>|<span data-ttu-id="8acb8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="8acb8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8acb8-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8acb8-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8acb8-112">Décrit l’état d’une réponse d’opération **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="8acb8-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="8acb8-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="8acb8-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8acb8-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="8acb8-114">-  Success</span></span>  <br/><span data-ttu-id="8acb8-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="8acb8-115">-  Warning</span></span>  <br/><span data-ttu-id="8acb8-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="8acb8-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="8acb8-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="8acb8-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="8acb8-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="8acb8-118">**Value**</span></span>|<span data-ttu-id="8acb8-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8acb8-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8acb8-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="8acb8-120">**Success**</span></span> <br/> |<span data-ttu-id="8acb8-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="8acb8-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8acb8-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="8acb8-122">**Warning**</span></span> <br/> | <span data-ttu-id="8acb8-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="8acb8-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8acb8-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="8acb8-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="8acb8-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="8acb8-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="8acb8-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="8acb8-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8acb8-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="8acb8-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8acb8-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="8acb8-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="8acb8-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="8acb8-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8acb8-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="8acb8-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="8acb8-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="8acb8-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="8acb8-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="8acb8-132">**Error**</span></span> <br/> | <span data-ttu-id="8acb8-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="8acb8-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8acb8-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="8acb8-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8acb8-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="8acb8-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8acb8-136">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="8acb8-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8acb8-137">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="8acb8-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="8acb8-138">-Attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="8acb8-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8acb8-139">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="8acb8-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8acb8-140">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="8acb8-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="8acb8-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="8acb8-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8acb8-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8acb8-142">Child elements</span></span>

|<span data-ttu-id="8acb8-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8acb8-143">**Element**</span></span>|<span data-ttu-id="8acb8-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="8acb8-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8acb8-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="8acb8-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8acb8-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="8acb8-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8acb8-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8acb8-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8acb8-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="8acb8-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8acb8-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8acb8-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8acb8-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="8acb8-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="8acb8-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="8acb8-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8acb8-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8acb8-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8acb8-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="8acb8-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8acb8-154">Notification</span><span class="sxs-lookup"><span data-stu-id="8acb8-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8acb8-155">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="8acb8-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8acb8-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8acb8-156">Parent elements</span></span>

|<span data-ttu-id="8acb8-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8acb8-157">**Element**</span></span>|<span data-ttu-id="8acb8-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="8acb8-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8acb8-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8acb8-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8acb8-160">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8acb8-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8acb8-161">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8acb8-161">Text value</span></span>

<span data-ttu-id="8acb8-162">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8acb8-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8acb8-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="8acb8-163">Remarks</span></span>

<span data-ttu-id="8acb8-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8acb8-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8acb8-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8acb8-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8acb8-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8acb8-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8acb8-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8acb8-167">Schema Name</span></span>  <br/> |<span data-ttu-id="8acb8-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8acb8-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8acb8-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8acb8-169">Validation File</span></span>  <br/> |<span data-ttu-id="8acb8-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8acb8-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8acb8-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8acb8-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="8acb8-172">False</span><span class="sxs-lookup"><span data-stu-id="8acb8-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8acb8-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8acb8-173">See also</span></span>

- [<span data-ttu-id="8acb8-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="8acb8-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="8acb8-175">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="8acb8-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="8acb8-176">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="8acb8-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

