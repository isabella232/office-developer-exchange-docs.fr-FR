---
title: GetRoomsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomsResponse
api_type:
- schema
ms.assetid: a8c85f65-bb63-4e7a-b0ca-7c9a04560a58
description: L’élément GetRoomsResponse définit une réponse à une demande d’opération GetRooms.
ms.openlocfilehash: 7399ab910a99b39757eb752b11a4771ba81be46a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756733"
---
# <a name="getroomsresponse"></a><span data-ttu-id="ee7a7-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="ee7a7-103">GetRoomsResponse</span></span>

<span data-ttu-id="ee7a7-104">L’élément **GetRoomsResponse** définit une réponse à une demande [d’opération GetRooms](getrooms-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ee7a7-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ee7a7-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee7a7-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="ee7a7-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="ee7a7-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="ee7a7-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee7a7-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ee7a7-108">Attributes and elements</span></span>

<span data-ttu-id="ee7a7-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee7a7-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ee7a7-110">Attributes</span></span>

|<span data-ttu-id="ee7a7-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-111">**Attribute**</span></span>|<span data-ttu-id="ee7a7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee7a7-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ee7a7-114">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="ee7a7-115">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="ee7a7-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="ee7a7-116">-Réussite</span><span class="sxs-lookup"><span data-stu-id="ee7a7-116">-  Success</span></span>  <br/><span data-ttu-id="ee7a7-117">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="ee7a7-117">-  Warning</span></span>  <br/><span data-ttu-id="ee7a7-118">-Erreur</span><span class="sxs-lookup"><span data-stu-id="ee7a7-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="ee7a7-119">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ee7a7-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="ee7a7-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-120">**Value**</span></span>|<span data-ttu-id="ee7a7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee7a7-122">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-122">**Success**</span></span> <br/> |<span data-ttu-id="ee7a7-123">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ee7a7-124">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-124">**Warning**</span></span> <br/> | <span data-ttu-id="ee7a7-125">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-125">Describes a request that was not processed.</span></span> <span data-ttu-id="ee7a7-126">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ee7a7-127">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="ee7a7-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="ee7a7-128">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ee7a7-129">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ee7a7-130">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="ee7a7-131">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ee7a7-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="ee7a7-133">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="ee7a7-134">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-134">**Error**</span></span> <br/> | <span data-ttu-id="ee7a7-135">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ee7a7-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="ee7a7-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ee7a7-137">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="ee7a7-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ee7a7-138">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="ee7a7-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ee7a7-139">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="ee7a7-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="ee7a7-140">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="ee7a7-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="ee7a7-141">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="ee7a7-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ee7a7-142">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="ee7a7-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ee7a7-143">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ee7a7-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ee7a7-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ee7a7-144">Child elements</span></span>

|<span data-ttu-id="ee7a7-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-145">**Element**</span></span>|<span data-ttu-id="ee7a7-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee7a7-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="ee7a7-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ee7a7-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ee7a7-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ee7a7-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ee7a7-150">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ee7a7-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ee7a7-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ee7a7-152">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="ee7a7-153">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ee7a7-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ee7a7-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ee7a7-155">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ee7a7-156">Salles</span><span class="sxs-lookup"><span data-stu-id="ee7a7-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="ee7a7-157">Fournit une liste des adresses de messagerie et les noms complets qui représentent des salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee7a7-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ee7a7-158">Parent elements</span></span>

|<span data-ttu-id="ee7a7-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-159">**Element**</span></span>|<span data-ttu-id="ee7a7-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="ee7a7-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee7a7-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee7a7-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ee7a7-162">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee7a7-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="ee7a7-163">Remarks</span></span>

<span data-ttu-id="ee7a7-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee7a7-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee7a7-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ee7a7-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee7a7-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ee7a7-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee7a7-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ee7a7-167">Schema Name</span></span>  <br/> |<span data-ttu-id="ee7a7-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ee7a7-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee7a7-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ee7a7-169">Validation File</span></span>  <br/> |<span data-ttu-id="ee7a7-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee7a7-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee7a7-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ee7a7-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee7a7-172">False</span><span class="sxs-lookup"><span data-stu-id="ee7a7-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee7a7-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ee7a7-173">See also</span></span>

- [<span data-ttu-id="ee7a7-174">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="ee7a7-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="ee7a7-175">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ee7a7-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

