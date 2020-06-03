---
title: GetAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponseMessage
api_type:
- schema
ms.assetid: f0a841af-422d-4c82-b710-41e2038dbee4
description: L’élément GetAttachmentResponseMessage contient l’État et le résultat d’une seule demande d’opération GetAttachment.
ms.openlocfilehash: cfe36364431a8fe81c3f62e68356b634f00bee78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457794"
---
# <a name="getattachmentresponsemessage"></a><span data-ttu-id="1f9c9-103">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1f9c9-103">GetAttachmentResponseMessage</span></span>

<span data-ttu-id="1f9c9-104">L’élément **GetAttachmentResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1f9c9-104">The **GetAttachmentResponseMessage** element contains the status and result of a single [GetAttachment operation](getattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="1f9c9-105">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="1f9c9-105">GetAttachmentResponse</span></span>](getattachmentresponse.md) 
- [<span data-ttu-id="1f9c9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1f9c9-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="1f9c9-107">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1f9c9-107">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
  
```xml
<GetAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</GetAttachmentResponseMessage>
```

 <span data-ttu-id="1f9c9-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-108">**AttachmentInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f9c9-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1f9c9-109">Attributes and elements</span></span>

<span data-ttu-id="1f9c9-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f9c9-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="1f9c9-111">Attributes</span></span>

|<span data-ttu-id="1f9c9-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-112">**Attribute**</span></span>|<span data-ttu-id="1f9c9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f9c9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1f9c9-115">Décrit l’état d’une réponse d' [opération GetAttachment](getattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1f9c9-115">Describes the status of a [GetAttachment operation](getattachment-operation.md) response.</span></span><br/><br/> <span data-ttu-id="1f9c9-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1f9c9-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="1f9c9-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1f9c9-117">-  Success</span></span>  <br/><span data-ttu-id="1f9c9-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="1f9c9-118">-  Warning</span></span>  <br/><span data-ttu-id="1f9c9-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1f9c9-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="1f9c9-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1f9c9-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="1f9c9-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-121">**Value**</span></span>|<span data-ttu-id="1f9c9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f9c9-123">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="1f9c9-123">Success</span></span>  <br/> |<span data-ttu-id="1f9c9-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1f9c9-125">Avertissement</span><span class="sxs-lookup"><span data-stu-id="1f9c9-125">Warning</span></span>  <br/> | <span data-ttu-id="1f9c9-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="1f9c9-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1f9c9-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="1f9c9-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="1f9c9-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1f9c9-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1f9c9-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="1f9c9-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1f9c9-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="1f9c9-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="1f9c9-135">Erreur</span><span class="sxs-lookup"><span data-stu-id="1f9c9-135">Error</span></span>  <br/> | <span data-ttu-id="1f9c9-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1f9c9-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="1f9c9-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1f9c9-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="1f9c9-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1f9c9-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="1f9c9-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1f9c9-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1f9c9-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="1f9c9-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1f9c9-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1f9c9-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="1f9c9-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1f9c9-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="1f9c9-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1f9c9-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1f9c9-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1f9c9-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1f9c9-145">Child elements</span></span>

|<span data-ttu-id="1f9c9-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-146">**Element**</span></span>|<span data-ttu-id="1f9c9-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f9c9-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="1f9c9-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1f9c9-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1f9c9-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1f9c9-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1f9c9-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1f9c9-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1f9c9-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1f9c9-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1f9c9-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1f9c9-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1f9c9-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1f9c9-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1f9c9-157">Attachments</span><span class="sxs-lookup"><span data-stu-id="1f9c9-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1f9c9-158">Contient les éléments ou les fichiers qui sont ttached à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-158">Contains the items or files that are ttached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f9c9-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1f9c9-159">Parent elements</span></span>

|<span data-ttu-id="1f9c9-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-160">**Element**</span></span>|<span data-ttu-id="1f9c9-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="1f9c9-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f9c9-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1f9c9-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1f9c9-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f9c9-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="1f9c9-164">Remarks</span></span>

<span data-ttu-id="1f9c9-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1f9c9-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f9c9-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1f9c9-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f9c9-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1f9c9-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f9c9-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1f9c9-168">Schema Name</span></span>  <br/> |<span data-ttu-id="1f9c9-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1f9c9-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f9c9-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1f9c9-170">Validation File</span></span>  <br/> |<span data-ttu-id="1f9c9-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1f9c9-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f9c9-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1f9c9-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f9c9-173">False</span><span class="sxs-lookup"><span data-stu-id="1f9c9-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f9c9-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1f9c9-174">See also</span></span>

- [<span data-ttu-id="1f9c9-175">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1f9c9-175">GetAttachment</span></span>](getattachment.md) 
- [<span data-ttu-id="1f9c9-176">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1f9c9-176">GetAttachment operation</span></span>](getattachment-operation.md)

