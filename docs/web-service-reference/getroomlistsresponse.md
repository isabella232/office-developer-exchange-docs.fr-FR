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
description: L’élément GetRoomListsResponse définit la réponse à une demande d’opération GetRoomLists.
ms.openlocfilehash: 8231435f7dc348a070852f57d6152550326b5df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756739"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="7cceb-103">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="7cceb-103">GetRoomListsResponse</span></span>

<span data-ttu-id="7cceb-104">L’élément **GetRoomListsResponse** définit la réponse à une demande [d’opération GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7cceb-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="7cceb-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7cceb-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="7cceb-106">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="7cceb-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="7cceb-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7cceb-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cceb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7cceb-108">Attributes and elements</span></span>

<span data-ttu-id="7cceb-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7cceb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cceb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7cceb-110">Attributes</span></span>

|<span data-ttu-id="7cceb-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7cceb-111">**Attribute**</span></span>|<span data-ttu-id="7cceb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cceb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cceb-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7cceb-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7cceb-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7cceb-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="7cceb-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="7cceb-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="7cceb-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="7cceb-116">-  Success</span></span>  <br/><span data-ttu-id="7cceb-117">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="7cceb-117">-  Warning</span></span>  <br/><span data-ttu-id="7cceb-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="7cceb-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7cceb-119">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7cceb-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="7cceb-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7cceb-120">**Value**</span></span>|<span data-ttu-id="7cceb-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cceb-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7cceb-122">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="7cceb-122">**Success**</span></span> <br/> |<span data-ttu-id="7cceb-123">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="7cceb-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7cceb-124">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="7cceb-124">**Warning**</span></span> <br/> | <span data-ttu-id="7cceb-125">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="7cceb-125">Describes a request that was not processed.</span></span> <span data-ttu-id="7cceb-126">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="7cceb-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7cceb-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="7cceb-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7cceb-128">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="7cceb-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7cceb-129">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="7cceb-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="7cceb-130">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="7cceb-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="7cceb-131">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="7cceb-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7cceb-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="7cceb-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="7cceb-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="7cceb-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="7cceb-134">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="7cceb-134">**Error**</span></span> <br/> | <span data-ttu-id="7cceb-135">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="7cceb-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7cceb-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="7cceb-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7cceb-137">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="7cceb-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7cceb-138">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="7cceb-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7cceb-139">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="7cceb-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="7cceb-140">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="7cceb-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7cceb-141">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="7cceb-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7cceb-142">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="7cceb-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="7cceb-143">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="7cceb-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="7cceb-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7cceb-144">Child elements</span></span>

|<span data-ttu-id="7cceb-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cceb-145">**Element**</span></span>|<span data-ttu-id="7cceb-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cceb-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cceb-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="7cceb-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7cceb-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="7cceb-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7cceb-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7cceb-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7cceb-150">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="7cceb-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7cceb-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7cceb-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7cceb-152">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="7cceb-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="7cceb-153">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="7cceb-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7cceb-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7cceb-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7cceb-155">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="7cceb-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7cceb-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="7cceb-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="7cceb-157">Fournit une liste des adresses de messagerie et les noms complets qui représentent des listes de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="7cceb-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cceb-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7cceb-158">Parent elements</span></span>

|<span data-ttu-id="7cceb-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cceb-159">**Element**</span></span>|<span data-ttu-id="7cceb-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cceb-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cceb-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7cceb-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7cceb-162">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cceb-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="7cceb-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7cceb-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cceb-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7cceb-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7cceb-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7cceb-165">Schema Name</span></span>  <br/> |<span data-ttu-id="7cceb-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7cceb-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7cceb-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7cceb-167">Validation File</span></span>  <br/> |<span data-ttu-id="7cceb-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7cceb-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7cceb-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7cceb-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cceb-170">False</span><span class="sxs-lookup"><span data-stu-id="7cceb-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cceb-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7cceb-171">See also</span></span>

- [<span data-ttu-id="7cceb-172">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="7cceb-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="7cceb-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7cceb-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
