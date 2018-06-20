---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: L’élément SyncFolderItemsResponseMessage contient l’état et les résultats d’une demande d’opération SyncFolderItems unique.
ms.openlocfilehash: 9bb32232143df56ad9de93480e10a5941e68025a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838668"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="ffe67-103">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ffe67-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="ffe67-104">L’élément **SyncFolderItemsResponseMessage** contient l’état et les résultats d’une seule demande [d’opération SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ffe67-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ffe67-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="ffe67-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="ffe67-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffe67-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ffe67-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ffe67-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 <span data-ttu-id="ffe67-108">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ffe67-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffe67-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ffe67-109">Attributes and elements</span></span>

<span data-ttu-id="ffe67-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ffe67-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffe67-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ffe67-111">Attributes</span></span>

|<span data-ttu-id="ffe67-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ffe67-112">**Attribute**</span></span>|<span data-ttu-id="ffe67-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffe67-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffe67-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ffe67-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ffe67-115">Décrit l’état d’une réponse de [l’opération SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ffe67-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="ffe67-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="ffe67-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="ffe67-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="ffe67-117">-  Success</span></span>  <br/><span data-ttu-id="ffe67-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="ffe67-118">-  Warning</span></span>  <br/><span data-ttu-id="ffe67-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="ffe67-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="ffe67-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ffe67-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="ffe67-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ffe67-121">**Value**</span></span>|<span data-ttu-id="ffe67-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffe67-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ffe67-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="ffe67-123">**Success**</span></span> <br/> |<span data-ttu-id="ffe67-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="ffe67-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ffe67-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="ffe67-125">**Warning**</span></span> <br/> | <span data-ttu-id="ffe67-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="ffe67-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ffe67-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite lors du traitement d’un élément dans la demande et les éléments suivants ne peuvent pas être traitées.</span><span class="sxs-lookup"><span data-stu-id="ffe67-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="ffe67-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="ffe67-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ffe67-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="ffe67-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ffe67-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ffe67-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ffe67-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="ffe67-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ffe67-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ffe67-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ffe67-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="ffe67-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="ffe67-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="ffe67-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="ffe67-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="ffe67-135">**Error**</span></span> <br/> | <span data-ttu-id="ffe67-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="ffe67-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ffe67-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="ffe67-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ffe67-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="ffe67-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ffe67-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="ffe67-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="ffe67-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="ffe67-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="ffe67-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="ffe67-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ffe67-142">-Toute tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="ffe67-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ffe67-143">-Tout échec de côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="ffe67-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="ffe67-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ffe67-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ffe67-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ffe67-145">Child elements</span></span>

|<span data-ttu-id="ffe67-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffe67-146">**Element**</span></span>|<span data-ttu-id="ffe67-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffe67-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffe67-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ffe67-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ffe67-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ffe67-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ffe67-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ffe67-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="ffe67-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ffe67-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ffe67-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="ffe67-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ffe67-154">Il contient la valeur 0.</span><span class="sxs-lookup"><span data-stu-id="ffe67-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ffe67-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ffe67-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="ffe67-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-157">SyncState</span><span class="sxs-lookup"><span data-stu-id="ffe67-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ffe67-158">Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="ffe67-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="ffe67-159">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="ffe67-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-160">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="ffe67-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="ffe67-161">Indique si le dernier élément à synchroniser a été inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ffe67-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="ffe67-162">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="ffe67-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="ffe67-163">Contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffe67-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffe67-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ffe67-164">Parent elements</span></span>

|<span data-ttu-id="ffe67-165">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffe67-165">**Element**</span></span>|<span data-ttu-id="ffe67-166">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffe67-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffe67-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffe67-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ffe67-168">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffe67-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ffe67-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="ffe67-169">Remarks</span></span>

<span data-ttu-id="ffe67-170">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ffe67-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffe67-171">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ffe67-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffe67-172">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ffe67-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffe67-173">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ffe67-173">Schema Name</span></span>  <br/> |<span data-ttu-id="ffe67-174">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ffe67-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ffe67-175">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ffe67-175">Validation File</span></span>  <br/> |<span data-ttu-id="ffe67-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ffe67-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffe67-177">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ffe67-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffe67-178">False</span><span class="sxs-lookup"><span data-stu-id="ffe67-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffe67-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffe67-179">See also</span></span>

- [<span data-ttu-id="ffe67-180">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ffe67-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="ffe67-181">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ffe67-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

