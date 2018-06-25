---
title: UpdateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponseMessage
api_type:
- schema
ms.assetid: dc585b05-5afc-4c74-8763-5a54f9a650ec
description: L’élément UpdateItemResponseMessage contient l’état et les résultats d’une demande d’opération UpdateItem unique.
ms.openlocfilehash: c971657813784e68a01539899e8fabea67847325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838898"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="d122c-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d122c-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="d122c-104">L’élément **UpdateItemResponseMessage** contient l’état et les résultats d’une seule demande [d’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d122c-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="d122c-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="d122c-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="d122c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d122c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d122c-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d122c-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
```xml
<UpdateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <ConflictResults/>
</UpdateItemResponseMessage>
```

 <span data-ttu-id="d122c-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d122c-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d122c-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d122c-109">Attributes and elements</span></span>

<span data-ttu-id="d122c-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d122c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d122c-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="d122c-111">Attributes</span></span>

|<span data-ttu-id="d122c-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d122c-112">**Attribute**</span></span>|<span data-ttu-id="d122c-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="d122c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d122c-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d122c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d122c-115">Décrit l’état d’une réponse de [l’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d122c-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="d122c-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="d122c-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d122c-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="d122c-117">-  Success</span></span>  <br/><span data-ttu-id="d122c-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="d122c-118">-  Warning</span></span>  <br/><span data-ttu-id="d122c-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="d122c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d122c-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d122c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d122c-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d122c-121">**Value**</span></span>|<span data-ttu-id="d122c-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d122c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d122c-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="d122c-123">**Success**</span></span> <br/> |<span data-ttu-id="d122c-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="d122c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d122c-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="d122c-125">**Warning**</span></span> <br/> | <span data-ttu-id="d122c-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="d122c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d122c-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant un élément dans la demande a été traité et les éléments suivants n’ont pas peuvent être traitées.</span><span class="sxs-lookup"><span data-stu-id="d122c-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d122c-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="d122c-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d122c-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="d122c-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d122c-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d122c-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d122c-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="d122c-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d122c-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d122c-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d122c-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="d122c-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="d122c-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="d122c-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d122c-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="d122c-135">**Error**</span></span> <br/> | <span data-ttu-id="d122c-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="d122c-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d122c-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="d122c-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d122c-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="d122c-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d122c-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="d122c-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d122c-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="d122c-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="d122c-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="d122c-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d122c-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="d122c-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d122c-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="d122c-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d122c-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d122c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d122c-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d122c-145">Child elements</span></span>

|<span data-ttu-id="d122c-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d122c-146">**Element**</span></span>|<span data-ttu-id="d122c-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="d122c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d122c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d122c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d122c-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d122c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d122c-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d122c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d122c-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="d122c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d122c-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d122c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d122c-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="d122c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d122c-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="d122c-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d122c-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d122c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d122c-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="d122c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d122c-157">Items</span><span class="sxs-lookup"><span data-stu-id="d122c-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="d122c-158">Contient un tableau d’éléments mis à jour.</span><span class="sxs-lookup"><span data-stu-id="d122c-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="d122c-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="d122c-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="d122c-160">Contient le nombre de conflits dans une réponse [d’opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d122c-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d122c-161">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d122c-161">Parent elements</span></span>

|<span data-ttu-id="d122c-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d122c-162">**Element**</span></span>|<span data-ttu-id="d122c-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="d122c-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d122c-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d122c-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d122c-165">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d122c-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d122c-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="d122c-166">Remarks</span></span>

<span data-ttu-id="d122c-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d122c-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d122c-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d122c-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d122c-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d122c-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d122c-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d122c-170">Schema Name</span></span>  <br/> |<span data-ttu-id="d122c-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d122c-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d122c-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d122c-172">Validation File</span></span>  <br/> |<span data-ttu-id="d122c-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d122c-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d122c-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d122c-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="d122c-175">False</span><span class="sxs-lookup"><span data-stu-id="d122c-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d122c-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d122c-176">See also</span></span>

- [<span data-ttu-id="d122c-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d122c-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="d122c-178">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="d122c-178">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="d122c-179">Mise à jour de tâches</span><span class="sxs-lookup"><span data-stu-id="d122c-179">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

