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
description: L’élément UploadItemsResponseMessage contient l’état et les résultats d’une demande pour télécharger un élément de boîte aux lettres unique.
ms.openlocfilehash: 9a1a33011aa1e240ab7e15794e2e89401238ffda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838934"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="bef29-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bef29-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="bef29-104">L’élément **UploadItemsResponseMessage** contient l’état et les résultats d’une demande pour télécharger un élément de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="bef29-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="bef29-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="bef29-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="bef29-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bef29-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="bef29-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bef29-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="bef29-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bef29-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bef29-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bef29-109">Attributes and elements</span></span>

<span data-ttu-id="bef29-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bef29-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bef29-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="bef29-111">Attributes</span></span>

|<span data-ttu-id="bef29-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bef29-112">**Attribute**</span></span>|<span data-ttu-id="bef29-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef29-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bef29-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bef29-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bef29-115">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="bef29-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="bef29-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="bef29-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="bef29-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="bef29-117">-  Success</span></span>  <br/><span data-ttu-id="bef29-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="bef29-118">-  Warning</span></span>  <br/><span data-ttu-id="bef29-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="bef29-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bef29-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="bef29-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bef29-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bef29-121">**Value**</span></span>|<span data-ttu-id="bef29-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef29-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bef29-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="bef29-123">**Success**</span></span> <br/> |<span data-ttu-id="bef29-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="bef29-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bef29-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="bef29-125">**Warning**</span></span> <br/> | <span data-ttu-id="bef29-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="bef29-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bef29-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="bef29-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="bef29-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="bef29-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="bef29-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="bef29-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bef29-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bef29-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bef29-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="bef29-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bef29-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="bef29-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bef29-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="bef29-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bef29-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="bef29-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bef29-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="bef29-135">**Error**</span></span> <br/> | <span data-ttu-id="bef29-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="bef29-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bef29-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="bef29-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bef29-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="bef29-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bef29-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="bef29-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="bef29-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="bef29-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="bef29-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="bef29-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="bef29-142">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="bef29-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bef29-143">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="bef29-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="bef29-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="bef29-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bef29-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bef29-145">Child elements</span></span>

|<span data-ttu-id="bef29-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bef29-146">**Element**</span></span>|<span data-ttu-id="bef29-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef29-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bef29-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="bef29-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bef29-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="bef29-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bef29-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bef29-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bef29-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="bef29-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bef29-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bef29-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bef29-153">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="bef29-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bef29-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="bef29-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bef29-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bef29-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bef29-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="bef29-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bef29-157">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="bef29-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bef29-158">Contient l’identificateur d’élément d’un élément téléchargé.</span><span class="sxs-lookup"><span data-stu-id="bef29-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bef29-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bef29-159">Parent elements</span></span>

|<span data-ttu-id="bef29-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bef29-160">**Element**</span></span>|<span data-ttu-id="bef29-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef29-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bef29-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bef29-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bef29-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bef29-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bef29-164">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bef29-164">Text value</span></span>

<span data-ttu-id="bef29-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bef29-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bef29-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="bef29-166">Remarks</span></span>

<span data-ttu-id="bef29-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bef29-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bef29-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bef29-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bef29-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bef29-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bef29-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bef29-170">Schema Name</span></span>  <br/> |<span data-ttu-id="bef29-171">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="bef29-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="bef29-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bef29-172">Validation File</span></span>  <br/> |<span data-ttu-id="bef29-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bef29-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bef29-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bef29-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="bef29-175">False</span><span class="sxs-lookup"><span data-stu-id="bef29-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bef29-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bef29-176">See also</span></span>

- [<span data-ttu-id="bef29-177">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="bef29-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="bef29-178">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="bef29-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="bef29-179">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bef29-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

