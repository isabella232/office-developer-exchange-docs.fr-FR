---
title: CreateAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: L’élément CreateAttachmentResponseMessage contient l’état et les résultats d’une demande d’opération CreateAttachment unique.
ms.openlocfilehash: a6d3adde07dedb7a2533d6e9c7fc6ff0497792bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755692"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="00010-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00010-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="00010-104">L’élément **CreateAttachmentResponseMessage** contient l’état et les résultats d’une seule demande [d’opération CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="00010-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="00010-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="00010-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="00010-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="00010-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="00010-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00010-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="00010-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="00010-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="00010-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00010-109">Attributes and elements</span></span>

<span data-ttu-id="00010-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00010-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00010-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="00010-111">Attributes</span></span>

|<span data-ttu-id="00010-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="00010-112">**Attribute**</span></span>|<span data-ttu-id="00010-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="00010-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="00010-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="00010-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="00010-115">Décrit l’état d’une réponse de [l’opération CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="00010-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="00010-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="00010-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="00010-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="00010-117">-  Success</span></span>  <br/><span data-ttu-id="00010-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="00010-118">-  Warning</span></span>  <br/><span data-ttu-id="00010-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="00010-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="00010-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="00010-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="00010-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="00010-121">**Value**</span></span>|<span data-ttu-id="00010-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="00010-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="00010-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="00010-123">**Success**</span></span> <br/> |<span data-ttu-id="00010-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="00010-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="00010-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="00010-125">**Warning**</span></span> <br/> | <span data-ttu-id="00010-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="00010-126">Describes a request that was not processed.</span></span> <span data-ttu-id="00010-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="00010-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="00010-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="00010-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="00010-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="00010-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="00010-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="00010-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="00010-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="00010-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="00010-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="00010-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="00010-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="00010-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="00010-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="00010-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="00010-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="00010-135">**Error**</span></span> <br/> | <span data-ttu-id="00010-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="00010-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="00010-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="00010-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="00010-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="00010-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="00010-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="00010-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="00010-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="00010-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="00010-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="00010-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="00010-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="00010-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="00010-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="00010-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="00010-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="00010-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="00010-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00010-145">Child elements</span></span>

|<span data-ttu-id="00010-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00010-146">**Element**</span></span>|<span data-ttu-id="00010-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="00010-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00010-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="00010-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="00010-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="00010-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="00010-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00010-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="00010-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="00010-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="00010-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="00010-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="00010-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="00010-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="00010-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="00010-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="00010-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="00010-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="00010-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="00010-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="00010-157">Attachments</span><span class="sxs-lookup"><span data-stu-id="00010-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="00010-158">Contient les éléments ou les fichiers joints à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00010-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00010-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00010-159">Parent elements</span></span>

|<span data-ttu-id="00010-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00010-160">**Element**</span></span>|<span data-ttu-id="00010-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="00010-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00010-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="00010-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="00010-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00010-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00010-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="00010-164">Remarks</span></span>

<span data-ttu-id="00010-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="00010-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="00010-166">Si plusieurs pièces jointes sont associés à un élément dans un seul aller-retour, l’attribut **RootItemChangeKey** dans le dernier message de réponse est celui qui représente la nouvelle clé de modification de l’élément qui a les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="00010-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="00010-167">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00010-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00010-168">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00010-168">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00010-169">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00010-169">Schema Name</span></span>  <br/> |<span data-ttu-id="00010-170">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="00010-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00010-171">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00010-171">Validation File</span></span>  <br/> |<span data-ttu-id="00010-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00010-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00010-173">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00010-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="00010-174">False</span><span class="sxs-lookup"><span data-stu-id="00010-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00010-175">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00010-175">See also</span></span>

- [<span data-ttu-id="00010-176">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="00010-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="00010-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="00010-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="00010-178">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="00010-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="00010-179">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00010-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
