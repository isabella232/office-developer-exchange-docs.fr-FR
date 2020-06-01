---
title: GetRoomListsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomListsResponse
api_type:
- schema
ms.assetid: 8c736f68-1026-496a-b12f-c169c078abd0
description: L’élément GetRoomListsResponse définit la réponse à partir d’une demande d’opération GetRoomLists.
ms.openlocfilehash: b6d7c2baa2861309d72bcbf880eaed2ad0989175
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462942"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="d4b13-103">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="d4b13-103">GetRoomListsResponse</span></span>

<span data-ttu-id="d4b13-104">L’élément **GetRoomListsResponse** définit la réponse à partir d’une demande d' [opération GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b13-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d4b13-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d4b13-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d4b13-106">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="d4b13-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="d4b13-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d4b13-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4b13-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4b13-108">Attributes and elements</span></span>

<span data-ttu-id="d4b13-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4b13-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4b13-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4b13-110">Attributes</span></span>

|<span data-ttu-id="d4b13-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d4b13-111">**Attribute**</span></span>|<span data-ttu-id="d4b13-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b13-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4b13-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d4b13-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d4b13-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4b13-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d4b13-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="d4b13-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d4b13-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="d4b13-116">-  Success</span></span>  <br/><span data-ttu-id="d4b13-117">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="d4b13-117">-  Warning</span></span>  <br/><span data-ttu-id="d4b13-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="d4b13-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d4b13-119">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d4b13-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="d4b13-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d4b13-120">**Value**</span></span>|<span data-ttu-id="d4b13-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b13-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4b13-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="d4b13-122">**Success**</span></span> <br/> |<span data-ttu-id="d4b13-123">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="d4b13-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d4b13-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d4b13-124">**Warning**</span></span> <br/> | <span data-ttu-id="d4b13-125">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="d4b13-125">Describes a request that was not processed.</span></span> <span data-ttu-id="d4b13-126">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="d4b13-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d4b13-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="d4b13-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d4b13-128">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="d4b13-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d4b13-129">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d4b13-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="d4b13-130">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="d4b13-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d4b13-131">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d4b13-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d4b13-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="d4b13-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="d4b13-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="d4b13-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d4b13-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="d4b13-134">**Error**</span></span> <br/> | <span data-ttu-id="d4b13-135">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="d4b13-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d4b13-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="d4b13-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d4b13-137">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="d4b13-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d4b13-138">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="d4b13-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d4b13-139">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="d4b13-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="d4b13-140">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="d4b13-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d4b13-141">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="d4b13-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d4b13-142">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="d4b13-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d4b13-143">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b13-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="d4b13-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4b13-144">Child elements</span></span>

|<span data-ttu-id="d4b13-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4b13-145">**Element**</span></span>|<span data-ttu-id="d4b13-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b13-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4b13-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="d4b13-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d4b13-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4b13-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d4b13-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4b13-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d4b13-150">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="d4b13-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d4b13-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d4b13-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d4b13-152">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="d4b13-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d4b13-153">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="d4b13-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d4b13-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d4b13-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d4b13-155">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="d4b13-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d4b13-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="d4b13-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="d4b13-157">Fournit la liste des adresses de messagerie et des noms d’affichage qui représentent les listes des salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="d4b13-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4b13-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4b13-158">Parent elements</span></span>

|<span data-ttu-id="d4b13-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4b13-159">**Element**</span></span>|<span data-ttu-id="d4b13-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b13-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4b13-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d4b13-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d4b13-162">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4b13-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d4b13-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4b13-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4b13-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4b13-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4b13-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4b13-165">Schema Name</span></span>  <br/> |<span data-ttu-id="d4b13-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d4b13-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4b13-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4b13-167">Validation File</span></span>  <br/> |<span data-ttu-id="d4b13-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d4b13-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4b13-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4b13-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4b13-170">False</span><span class="sxs-lookup"><span data-stu-id="d4b13-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4b13-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4b13-171">See also</span></span>

- [<span data-ttu-id="d4b13-172">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="d4b13-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="d4b13-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4b13-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

