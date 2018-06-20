---
title: MoveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: L’élément MoveItemResponseMessage contient l’état et les résultats d’une demande d’opération MoveItem unique.
ms.openlocfilehash: af1c10391d9b5b761ab87983eea6321d61231152
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828493"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="6bd15-103">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6bd15-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="6bd15-104">L’élément **MoveItemResponseMessage** contient l’état et les résultats d’une seule demande [d’opération MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd15-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="6bd15-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6bd15-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bd15-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6bd15-106">Attributes and elements</span></span>

<span data-ttu-id="6bd15-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6bd15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bd15-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6bd15-108">Attributes</span></span>

|<span data-ttu-id="6bd15-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6bd15-109">**Attribute**</span></span>|<span data-ttu-id="6bd15-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bd15-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6bd15-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6bd15-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6bd15-112">Décrit l’état d’une réponse de [l’opération MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd15-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="6bd15-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="6bd15-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6bd15-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="6bd15-114">-  Success</span></span>  <br/><span data-ttu-id="6bd15-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="6bd15-115">-  Warning</span></span>  <br/><span data-ttu-id="6bd15-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="6bd15-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="6bd15-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6bd15-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="6bd15-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6bd15-118">**Value**</span></span>|<span data-ttu-id="6bd15-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bd15-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6bd15-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="6bd15-120">**Success**</span></span> <br/> |<span data-ttu-id="6bd15-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="6bd15-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6bd15-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="6bd15-122">**Warning**</span></span> <br/> | <span data-ttu-id="6bd15-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="6bd15-123">Describes a request that was not processed.</span></span> <span data-ttu-id="6bd15-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="6bd15-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="6bd15-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="6bd15-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="6bd15-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="6bd15-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6bd15-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6bd15-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6bd15-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="6bd15-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="6bd15-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6bd15-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6bd15-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="6bd15-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="6bd15-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="6bd15-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="6bd15-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="6bd15-132">**Error**</span></span> <br/> | <span data-ttu-id="6bd15-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="6bd15-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6bd15-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="6bd15-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="6bd15-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="6bd15-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6bd15-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="6bd15-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6bd15-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="6bd15-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="6bd15-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="6bd15-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6bd15-139">-Tout accès non autorisé a tenté par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="6bd15-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="6bd15-140">-Tout échec côté serveur en réponse à un appel côté client valid.</span><span class="sxs-lookup"><span data-stu-id="6bd15-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="6bd15-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6bd15-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6bd15-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6bd15-142">Child elements</span></span>

|<span data-ttu-id="6bd15-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6bd15-143">**Element**</span></span>|<span data-ttu-id="6bd15-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bd15-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bd15-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="6bd15-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6bd15-146">Une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="6bd15-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6bd15-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6bd15-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6bd15-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="6bd15-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6bd15-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6bd15-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6bd15-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="6bd15-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6bd15-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="6bd15-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6bd15-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6bd15-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6bd15-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="6bd15-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6bd15-154">Items</span><span class="sxs-lookup"><span data-stu-id="6bd15-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="6bd15-155">Contient un tableau d’éléments déplacés.</span><span class="sxs-lookup"><span data-stu-id="6bd15-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6bd15-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6bd15-156">Parent elements</span></span>

|<span data-ttu-id="6bd15-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6bd15-157">**Element**</span></span>|<span data-ttu-id="6bd15-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bd15-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bd15-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6bd15-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6bd15-160">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6bd15-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6bd15-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="6bd15-161">Remarks</span></span>

<span data-ttu-id="6bd15-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6bd15-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bd15-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6bd15-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bd15-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6bd15-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6bd15-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6bd15-165">Schema Name</span></span>  <br/> |<span data-ttu-id="6bd15-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6bd15-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6bd15-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6bd15-167">Validation File</span></span>  <br/> |<span data-ttu-id="6bd15-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6bd15-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6bd15-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6bd15-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bd15-170">False</span><span class="sxs-lookup"><span data-stu-id="6bd15-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bd15-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6bd15-171">See also</span></span>

- [<span data-ttu-id="6bd15-172">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="6bd15-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="6bd15-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="6bd15-173">MoveItem</span></span>](moveitem.md)

