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
description: L’élément UpdateItemResponseMessage contient l’État et le résultat d’une seule demande d’opération UpdateItem.
ms.openlocfilehash: ef25dcf26e06f199587cef885d8cbc9e93b52bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457941"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="1ae64-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1ae64-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="1ae64-104">L’élément **UpdateItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1ae64-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="1ae64-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="1ae64-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="1ae64-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1ae64-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="1ae64-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1ae64-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
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

 <span data-ttu-id="1ae64-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1ae64-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ae64-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1ae64-109">Attributes and elements</span></span>

<span data-ttu-id="1ae64-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1ae64-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ae64-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="1ae64-111">Attributes</span></span>

|<span data-ttu-id="1ae64-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1ae64-112">**Attribute**</span></span>|<span data-ttu-id="1ae64-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ae64-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ae64-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1ae64-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1ae64-115">Décrit l’état d’une réponse d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1ae64-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="1ae64-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1ae64-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1ae64-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1ae64-117">-  Success</span></span>  <br/><span data-ttu-id="1ae64-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="1ae64-118">-  Warning</span></span>  <br/><span data-ttu-id="1ae64-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1ae64-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1ae64-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1ae64-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="1ae64-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1ae64-121">**Value**</span></span>|<span data-ttu-id="1ae64-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ae64-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ae64-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="1ae64-123">**Success**</span></span> <br/> |<span data-ttu-id="1ae64-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1ae64-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1ae64-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1ae64-125">**Warning**</span></span> <br/> | <span data-ttu-id="1ae64-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="1ae64-126">Describes a request that was not processed.</span></span> <span data-ttu-id="1ae64-127">Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande a été traité et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="1ae64-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1ae64-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="1ae64-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1ae64-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1ae64-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1ae64-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1ae64-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1ae64-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="1ae64-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="1ae64-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1ae64-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1ae64-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1ae64-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="1ae64-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="1ae64-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="1ae64-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="1ae64-135">**Error**</span></span> <br/> | <span data-ttu-id="1ae64-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1ae64-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1ae64-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="1ae64-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1ae64-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="1ae64-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1ae64-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="1ae64-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1ae64-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1ae64-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="1ae64-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1ae64-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1ae64-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="1ae64-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1ae64-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="1ae64-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1ae64-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1ae64-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1ae64-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1ae64-145">Child elements</span></span>

|<span data-ttu-id="1ae64-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1ae64-146">**Element**</span></span>|<span data-ttu-id="1ae64-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ae64-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ae64-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="1ae64-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1ae64-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1ae64-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1ae64-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1ae64-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1ae64-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="1ae64-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1ae64-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1ae64-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1ae64-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1ae64-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1ae64-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1ae64-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1ae64-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1ae64-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1ae64-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="1ae64-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1ae64-157">Items</span><span class="sxs-lookup"><span data-stu-id="1ae64-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="1ae64-158">Contient un tableau d’éléments mis à jour.</span><span class="sxs-lookup"><span data-stu-id="1ae64-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="1ae64-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="1ae64-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="1ae64-160">Contient le nombre de conflits dans une réponse d' [opération UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1ae64-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ae64-161">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1ae64-161">Parent elements</span></span>

|<span data-ttu-id="1ae64-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1ae64-162">**Element**</span></span>|<span data-ttu-id="1ae64-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ae64-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ae64-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1ae64-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1ae64-165">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ae64-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ae64-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="1ae64-166">Remarks</span></span>

<span data-ttu-id="1ae64-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1ae64-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ae64-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1ae64-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ae64-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1ae64-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ae64-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1ae64-170">Schema Name</span></span>  <br/> |<span data-ttu-id="1ae64-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1ae64-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ae64-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1ae64-172">Validation File</span></span>  <br/> |<span data-ttu-id="1ae64-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1ae64-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ae64-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1ae64-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ae64-175">False</span><span class="sxs-lookup"><span data-stu-id="1ae64-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ae64-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1ae64-176">See also</span></span>

- [<span data-ttu-id="1ae64-177">Opération UpdateItem</span><span class="sxs-lookup"><span data-stu-id="1ae64-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="1ae64-178">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="1ae64-178">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="1ae64-179">Mise à jour des tâches</span><span class="sxs-lookup"><span data-stu-id="1ae64-179">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

