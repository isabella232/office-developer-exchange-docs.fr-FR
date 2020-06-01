---
title: DeleteAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponseMessage
api_type:
- schema
ms.assetid: 1edb085f-1674-48e5-8ec3-42351adeac7d
description: L’élément DeleteAttachmentResponseMessage contient l’État et le résultat d’une seule demande d’opération DeleteAttachment.
ms.openlocfilehash: 3ff253a5c2b6cbd69b7b976f7f41ca8b83814a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464258"
---
# <a name="deleteattachmentresponsemessage"></a><span data-ttu-id="6967e-103">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6967e-103">DeleteAttachmentResponseMessage</span></span>

<span data-ttu-id="6967e-104">L’élément **DeleteAttachmentResponseMessage** contient l’État et le résultat d’une seule demande d' [opération DeleteAttachment](deleteattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6967e-104">The **DeleteAttachmentResponseMessage** element contains the status and result of a single [DeleteAttachment operation](deleteattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="6967e-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="6967e-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)  
- [<span data-ttu-id="6967e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6967e-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="6967e-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6967e-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
```xml
<DeleteAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootItemId/>
</DeleteAttachmentResponseMessage>
```

<span data-ttu-id="6967e-108">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6967e-108">**DeleteAttachmentResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6967e-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6967e-109">Attributes and elements</span></span>

<span data-ttu-id="6967e-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6967e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6967e-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="6967e-111">Attributes</span></span>

|<span data-ttu-id="6967e-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6967e-112">**Attribute**</span></span>|<span data-ttu-id="6967e-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6967e-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6967e-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6967e-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6967e-115">Décrit l’état d’une réponse d' [opération DeleteAttachment](deleteattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6967e-115">Describes the status of a [DeleteAttachment operation](deleteattachment-operation.md) response.</span></span><br/><br/><span data-ttu-id="6967e-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="6967e-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="6967e-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="6967e-117">-  Success</span></span>  <br/><span data-ttu-id="6967e-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="6967e-118">-  Warning</span></span>  <br/><span data-ttu-id="6967e-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="6967e-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="6967e-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6967e-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="6967e-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6967e-121">**Value**</span></span>|<span data-ttu-id="6967e-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="6967e-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6967e-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="6967e-123">**Success**</span></span> <br/> |<span data-ttu-id="6967e-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="6967e-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6967e-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="6967e-125">**Warning**</span></span> <br/> | <span data-ttu-id="6967e-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="6967e-126">Describes a request that was not processed.</span></span> <span data-ttu-id="6967e-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="6967e-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="6967e-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="6967e-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="6967e-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="6967e-129">- The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6967e-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6967e-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6967e-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="6967e-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="6967e-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6967e-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6967e-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="6967e-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="6967e-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="6967e-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="6967e-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="6967e-135">**Error**</span></span> <br/> | <span data-ttu-id="6967e-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="6967e-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="6967e-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="6967e-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="6967e-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="6967e-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6967e-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="6967e-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6967e-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="6967e-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="6967e-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="6967e-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6967e-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="6967e-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6967e-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="6967e-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="6967e-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6967e-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6967e-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6967e-145">Child elements</span></span>

|<span data-ttu-id="6967e-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6967e-146">**Element**</span></span>|<span data-ttu-id="6967e-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="6967e-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6967e-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="6967e-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6967e-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="6967e-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6967e-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6967e-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6967e-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="6967e-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6967e-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6967e-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6967e-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="6967e-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6967e-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="6967e-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6967e-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6967e-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6967e-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="6967e-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6967e-157">RootItemId</span><span class="sxs-lookup"><span data-stu-id="6967e-157">RootItemId</span></span>](rootitemid.md) <br/> |<span data-ttu-id="6967e-158">Identifie l’élément parent d’une pièce jointe supprimée.</span><span class="sxs-lookup"><span data-stu-id="6967e-158">Identifies the parent item of a deleted attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6967e-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6967e-159">Parent elements</span></span>

|<span data-ttu-id="6967e-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6967e-160">**Element**</span></span>|<span data-ttu-id="6967e-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="6967e-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6967e-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6967e-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6967e-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6967e-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6967e-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="6967e-164">Remarks</span></span>

<span data-ttu-id="6967e-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6967e-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6967e-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6967e-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6967e-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6967e-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6967e-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6967e-168">Schema Name</span></span>  <br/> |<span data-ttu-id="6967e-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6967e-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6967e-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6967e-170">Validation File</span></span>  <br/> |<span data-ttu-id="6967e-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6967e-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6967e-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6967e-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="6967e-173">False</span><span class="sxs-lookup"><span data-stu-id="6967e-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6967e-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6967e-174">See also</span></span>

- [<span data-ttu-id="6967e-175">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="6967e-175">DeleteAttachment</span></span>](deleteattachment.md) 
- [<span data-ttu-id="6967e-176">Opération DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="6967e-176">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="6967e-177">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="6967e-177">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="6967e-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6967e-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

