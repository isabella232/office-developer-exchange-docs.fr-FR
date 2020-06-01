---
title: GetEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEventsResponseMessage
api_type:
- schema
ms.assetid: d433977f-b86a-499e-b9c3-f405ac229358
description: L’élément GetEventsResponseMessage contient l’État et le résultat d’une seule demande d’opération GetEvents.
ms.openlocfilehash: d307aa1f5234ab5a7a2527c55f5e48814ea2687b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462856"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="b0c3f-103">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b0c3f-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="b0c3f-104">L’élément **GetEventsResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetEvents](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c3f-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="b0c3f-105">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0c3f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b0c3f-106">Attributes and elements</span></span>

<span data-ttu-id="b0c3f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0c3f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b0c3f-108">Attributes</span></span>

|<span data-ttu-id="b0c3f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-109">**Attribute**</span></span>|<span data-ttu-id="b0c3f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0c3f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b0c3f-112">Décrit l’état d’une réponse d' [opération GetEvents](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c3f-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b0c3f-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b0c3f-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="b0c3f-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b0c3f-114">-  Success</span></span>  <br/><span data-ttu-id="b0c3f-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="b0c3f-115">-  Warning</span></span>  <br/><span data-ttu-id="b0c3f-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b0c3f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="b0c3f-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b0c3f-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="b0c3f-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-118">**Value**</span></span>|<span data-ttu-id="b0c3f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0c3f-120">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="b0c3f-120">Success</span></span>  <br/> |<span data-ttu-id="b0c3f-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b0c3f-122">Avertissement</span><span class="sxs-lookup"><span data-stu-id="b0c3f-122">Warning</span></span>  <br/> | <span data-ttu-id="b0c3f-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b0c3f-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b0c3f-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b0c3f-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="b0c3f-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b0c3f-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b0c3f-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b0c3f-129">-La base de données de boîtes aux lettres (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b0c3f-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="b0c3f-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="b0c3f-132">Erreur</span><span class="sxs-lookup"><span data-stu-id="b0c3f-132">Error</span></span>  <br/> | <span data-ttu-id="b0c3f-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b0c3f-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b0c3f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b0c3f-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="b0c3f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b0c3f-136">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="b0c3f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b0c3f-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b0c3f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b0c3f-138">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b0c3f-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b0c3f-139">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="b0c3f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b0c3f-140">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="b0c3f-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b0c3f-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c3f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b0c3f-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b0c3f-142">Child elements</span></span>

|<span data-ttu-id="b0c3f-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-143">**Element**</span></span>|<span data-ttu-id="b0c3f-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0c3f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b0c3f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b0c3f-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b0c3f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b0c3f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b0c3f-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b0c3f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b0c3f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b0c3f-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b0c3f-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b0c3f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b0c3f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b0c3f-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b0c3f-154">Notification</span><span class="sxs-lookup"><span data-stu-id="b0c3f-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0c3f-155">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0c3f-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b0c3f-156">Parent elements</span></span>

|<span data-ttu-id="b0c3f-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-157">**Element**</span></span>|<span data-ttu-id="b0c3f-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c3f-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0c3f-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b0c3f-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b0c3f-160">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0c3f-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0c3f-161">Remarks</span></span>

<span data-ttu-id="b0c3f-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b0c3f-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0c3f-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b0c3f-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0c3f-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b0c3f-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0c3f-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b0c3f-165">Schema Name</span></span>  <br/> |<span data-ttu-id="b0c3f-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b0c3f-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0c3f-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b0c3f-167">Validation File</span></span>  <br/> |<span data-ttu-id="b0c3f-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b0c3f-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0c3f-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b0c3f-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0c3f-170">False</span><span class="sxs-lookup"><span data-stu-id="b0c3f-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0c3f-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0c3f-171">See also</span></span>

- [<span data-ttu-id="b0c3f-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="b0c3f-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="b0c3f-173">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="b0c3f-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="b0c3f-174">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="b0c3f-174">GetEvents operation</span></span>](getevents-operation.md)

