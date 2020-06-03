---
title: UploadItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: L’élément UploadItemsResponseMessage contient l’État et les résultats d’une demande de téléchargement d’un seul élément de boîte aux lettres.
ms.openlocfilehash: 4049772c560f3d54a31351fe1fbed77fe5780bf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468494"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="0a082-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a082-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="0a082-104">L’élément **UploadItemsResponseMessage** contient l’État et les résultats d’une demande de téléchargement d’un seul élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0a082-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="0a082-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0a082-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="0a082-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a082-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0a082-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a082-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="0a082-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0a082-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a082-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0a082-109">Attributes and elements</span></span>

<span data-ttu-id="0a082-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0a082-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a082-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="0a082-111">Attributes</span></span>

|<span data-ttu-id="0a082-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0a082-112">**Attribute**</span></span>|<span data-ttu-id="0a082-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a082-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a082-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0a082-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0a082-115">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0a082-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0a082-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="0a082-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0a082-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="0a082-117">-  Success</span></span>  <br/><span data-ttu-id="0a082-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="0a082-118">-  Warning</span></span>  <br/><span data-ttu-id="0a082-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="0a082-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0a082-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0a082-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0a082-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0a082-121">**Value**</span></span>|<span data-ttu-id="0a082-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a082-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a082-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="0a082-123">**Success**</span></span> <br/> |<span data-ttu-id="0a082-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0a082-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0a082-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0a082-125">**Warning**</span></span> <br/> | <span data-ttu-id="0a082-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="0a082-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0a082-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="0a082-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0a082-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="0a082-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0a082-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="0a082-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0a082-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a082-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0a082-131">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="0a082-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0a082-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a082-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0a082-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="0a082-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0a082-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="0a082-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0a082-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="0a082-135">**Error**</span></span> <br/> | <span data-ttu-id="0a082-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0a082-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0a082-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="0a082-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0a082-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="0a082-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0a082-139">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="0a082-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0a082-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="0a082-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="0a082-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="0a082-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="0a082-142">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="0a082-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0a082-143">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="0a082-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="0a082-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0a082-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0a082-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0a082-145">Child elements</span></span>

|<span data-ttu-id="0a082-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a082-146">**Element**</span></span>|<span data-ttu-id="0a082-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a082-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a082-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0a082-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0a082-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0a082-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0a082-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0a082-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0a082-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="0a082-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0a082-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0a082-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0a082-153">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0a082-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="0a082-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="0a082-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0a082-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0a082-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0a082-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="0a082-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0a082-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="0a082-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0a082-158">Contient l’identificateur d’élément d’un élément téléchargé.</span><span class="sxs-lookup"><span data-stu-id="0a082-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a082-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0a082-159">Parent elements</span></span>

|<span data-ttu-id="0a082-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a082-160">**Element**</span></span>|<span data-ttu-id="0a082-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a082-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a082-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a082-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0a082-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a082-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a082-164">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0a082-164">Text value</span></span>

<span data-ttu-id="0a082-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0a082-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a082-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="0a082-166">Remarks</span></span>

<span data-ttu-id="0a082-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0a082-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a082-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0a082-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a082-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0a082-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a082-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0a082-170">Schema Name</span></span>  <br/> |<span data-ttu-id="0a082-171">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="0a082-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="0a082-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0a082-172">Validation File</span></span>  <br/> |<span data-ttu-id="0a082-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0a082-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a082-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0a082-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a082-175">False</span><span class="sxs-lookup"><span data-stu-id="0a082-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a082-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0a082-176">See also</span></span>

- [<span data-ttu-id="0a082-177">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="0a082-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="0a082-178">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="0a082-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="0a082-179">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0a082-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

