---
title: GetSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponseMessage
api_type:
- schema
ms.assetid: b6f5fd09-09f3-4e34-84b4-2f6c1f10f28f
description: L’élément GetSharingFolderResponseMessage contient l’état et les résultats d’une demande d’opération GetSharingFolder unique.
ms.openlocfilehash: 13ce3f628ff125140fc7459df5d567a67ddf7bc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827672"
---
# <a name="getsharingfolderresponsemessage"></a><span data-ttu-id="a0ec4-103">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a0ec4-103">GetSharingFolderResponseMessage</span></span>

<span data-ttu-id="a0ec4-104">L’élément **GetSharingFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0ec4-104">The **GetSharingFolderResponseMessage** element contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<GetSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponseMessage>
```

 <span data-ttu-id="a0ec4-105">**GetSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0ec4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0ec4-106">Attributes and elements</span></span>

<span data-ttu-id="a0ec4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0ec4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0ec4-108">Attributes</span></span>

|<span data-ttu-id="a0ec4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-109">**Attribute**</span></span>|<span data-ttu-id="a0ec4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0ec4-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a0ec4-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="a0ec4-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="a0ec4-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a0ec4-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="a0ec4-114">-  Success</span></span>  <br/><span data-ttu-id="a0ec4-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="a0ec4-115">-  Warning</span></span>  <br/><span data-ttu-id="a0ec4-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="a0ec4-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a0ec4-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a0ec4-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="a0ec4-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-118">**Value**</span></span>|<span data-ttu-id="a0ec4-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0ec4-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-120">**Success**</span></span> <br/> |<span data-ttu-id="a0ec4-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a0ec4-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-122">**Warning**</span></span> <br/> | <span data-ttu-id="a0ec4-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-123">Describes a request that was not processed.</span></span> <span data-ttu-id="a0ec4-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a0ec4-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="a0ec4-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a0ec4-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a0ec4-127">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="a0ec4-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="a0ec4-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a0ec4-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="a0ec4-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="a0ec4-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-132">**Error**</span></span> <br/> | <span data-ttu-id="a0ec4-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a0ec4-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="a0ec4-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a0ec4-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="a0ec4-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a0ec4-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="a0ec4-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a0ec4-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="a0ec4-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="a0ec4-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="a0ec4-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a0ec4-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="a0ec4-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a0ec4-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="a0ec4-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="a0ec4-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a0ec4-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0ec4-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0ec4-142">Child elements</span></span>

|<span data-ttu-id="a0ec4-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-143">**Element**</span></span>|<span data-ttu-id="a0ec4-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0ec4-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="a0ec4-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a0ec4-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a0ec4-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a0ec4-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a0ec4-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a0ec4-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a0ec4-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a0ec4-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="a0ec4-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a0ec4-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a0ec4-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a0ec4-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a0ec4-154">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="a0ec4-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="a0ec4-155">Représente l’identificateur du dossier local dans une relation de partage.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0ec4-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0ec4-156">Parent elements</span></span>

|<span data-ttu-id="a0ec4-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-157">**Element**</span></span>|<span data-ttu-id="a0ec4-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0ec4-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0ec4-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a0ec4-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a0ec4-160">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0ec4-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0ec4-161">Remarks</span></span>

<span data-ttu-id="a0ec4-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="a0ec4-162">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0ec4-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0ec4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0ec4-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0ec4-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0ec4-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0ec4-165">Schema Name</span></span>  <br/> |<span data-ttu-id="a0ec4-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0ec4-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0ec4-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0ec4-167">Validation File</span></span>  <br/> |<span data-ttu-id="a0ec4-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0ec4-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0ec4-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0ec4-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0ec4-170">False</span><span class="sxs-lookup"><span data-stu-id="a0ec4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0ec4-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0ec4-171">See also</span></span>

- [<span data-ttu-id="a0ec4-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0ec4-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

