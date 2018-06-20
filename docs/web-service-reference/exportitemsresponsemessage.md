---
title: ExportItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponseMessage
api_type:
- schema
ms.assetid: 830fb008-3c45-4988-9041-91a3da3fe689
description: L’élément ExportItemsResponseMessage contient l’état et les résultats d’une demande pour exporter un élément de boîte aux lettres unique.
ms.openlocfilehash: 99c2ca3f95efff6562ff95350b30fc79c5fb51e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756269"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="d3b02-103">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3b02-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="d3b02-104">L’élément **ExportItemsResponseMessage** contient l’état et les résultats d’une demande pour exporter un élément de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="d3b02-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="d3b02-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="d3b02-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="d3b02-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3b02-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="d3b02-107">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3b02-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
```XML
<ExportItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
   <Data/>
</ExportItemsResponseMessage>
```

<span data-ttu-id="d3b02-108">**ExportItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d3b02-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d3b02-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3b02-109">Attributes and elements</span></span>

<span data-ttu-id="d3b02-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3b02-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3b02-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3b02-111">Attributes</span></span>

|<span data-ttu-id="d3b02-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d3b02-112">**Attribute**</span></span>|<span data-ttu-id="d3b02-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3b02-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3b02-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d3b02-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d3b02-115">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d3b02-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="d3b02-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="d3b02-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="d3b02-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="d3b02-117">-  Success</span></span>  <br/><span data-ttu-id="d3b02-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="d3b02-118">-  Warning</span></span>  <br/><span data-ttu-id="d3b02-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="d3b02-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d3b02-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="d3b02-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="d3b02-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d3b02-121">**Value**</span></span>|<span data-ttu-id="d3b02-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3b02-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3b02-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="d3b02-123">**Success**</span></span> <br/> |<span data-ttu-id="d3b02-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="d3b02-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d3b02-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="d3b02-125">**Warning**</span></span> <br/> | <span data-ttu-id="d3b02-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="d3b02-126">Describes a request that was not processed.</span></span> <span data-ttu-id="d3b02-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="d3b02-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="d3b02-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="d3b02-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d3b02-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="d3b02-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d3b02-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d3b02-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d3b02-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="d3b02-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d3b02-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="d3b02-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d3b02-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="d3b02-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="d3b02-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="d3b02-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d3b02-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="d3b02-135">**Error**</span></span> <br/> | <span data-ttu-id="d3b02-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="d3b02-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d3b02-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="d3b02-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d3b02-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="d3b02-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d3b02-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="d3b02-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d3b02-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="d3b02-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="d3b02-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="d3b02-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d3b02-142">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="d3b02-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d3b02-143">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="d3b02-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d3b02-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="d3b02-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d3b02-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3b02-145">Child elements</span></span>

|<span data-ttu-id="d3b02-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3b02-146">**Element**</span></span>|<span data-ttu-id="d3b02-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3b02-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3b02-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="d3b02-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d3b02-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="d3b02-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d3b02-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3b02-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d3b02-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="d3b02-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d3b02-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d3b02-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d3b02-153">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="d3b02-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d3b02-154">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="d3b02-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d3b02-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d3b02-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d3b02-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="d3b02-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d3b02-157">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="d3b02-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d3b02-158">Contient l’identificateur d’élément d’un élément exporté.</span><span class="sxs-lookup"><span data-stu-id="d3b02-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="d3b02-159">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="d3b02-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="d3b02-160">Contient le contenu d’un élément exporté.</span><span class="sxs-lookup"><span data-stu-id="d3b02-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3b02-161">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3b02-161">Parent elements</span></span>

|<span data-ttu-id="d3b02-162">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3b02-162">**Element**</span></span>|<span data-ttu-id="d3b02-163">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3b02-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3b02-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3b02-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d3b02-165">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3b02-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3b02-166">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d3b02-166">Text value</span></span>

<span data-ttu-id="d3b02-167">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3b02-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3b02-168">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3b02-168">Remarks</span></span>

<span data-ttu-id="d3b02-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d3b02-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3b02-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3b02-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3b02-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3b02-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3b02-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3b02-172">Schema Name</span></span>  <br/> |<span data-ttu-id="d3b02-173">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="d3b02-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="d3b02-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3b02-174">Validation File</span></span>  <br/> |<span data-ttu-id="d3b02-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3b02-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3b02-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3b02-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3b02-177">False</span><span class="sxs-lookup"><span data-stu-id="d3b02-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3b02-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3b02-178">See also</span></span>

- [<span data-ttu-id="d3b02-179">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="d3b02-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="d3b02-180">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="d3b02-180">UploadItems operation</span></span>](uploaditems-operation.md)

