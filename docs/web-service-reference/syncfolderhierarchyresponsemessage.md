---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: L’élément SyncFolderHierarchyResponseMessage contient l’état et les résultats d’une demande d’opération SyncFolderHierarchy unique.
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838661"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="85506-103">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="85506-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="85506-104">L’élément **SyncFolderHierarchyResponseMessage** contient l’état et les résultats d’une seule demande [d’opération SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="85506-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="85506-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="85506-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="85506-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="85506-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="85506-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="85506-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 <span data-ttu-id="85506-108">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="85506-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85506-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85506-109">Attributes and elements</span></span>

<span data-ttu-id="85506-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85506-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85506-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="85506-111">Attributes</span></span>

|<span data-ttu-id="85506-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="85506-112">**Attribute**</span></span>|<span data-ttu-id="85506-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="85506-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="85506-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="85506-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="85506-115">Décrit l’état d’une réponse de [l’opération SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="85506-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="85506-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="85506-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="85506-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="85506-117">-  Success</span></span>  <br/><span data-ttu-id="85506-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="85506-118">-  Warning</span></span>  <br/><span data-ttu-id="85506-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="85506-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="85506-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="85506-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="85506-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="85506-121">**Value**</span></span>|<span data-ttu-id="85506-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="85506-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="85506-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="85506-123">**Success**</span></span> <br/> |<span data-ttu-id="85506-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="85506-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="85506-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="85506-125">**Warning**</span></span> <br/> | <span data-ttu-id="85506-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="85506-126">Describes a request that was not processed.</span></span> <span data-ttu-id="85506-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="85506-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="85506-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="85506-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="85506-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="85506-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="85506-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="85506-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="85506-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="85506-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="85506-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="85506-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="85506-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="85506-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="85506-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="85506-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="85506-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="85506-135">**Error**</span></span> <br/> | <span data-ttu-id="85506-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="85506-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="85506-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="85506-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="85506-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="85506-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="85506-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="85506-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="85506-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="85506-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="85506-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="85506-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="85506-142">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="85506-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="85506-143">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="85506-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="85506-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="85506-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="85506-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85506-145">Child elements</span></span>

|<span data-ttu-id="85506-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85506-146">**Element**</span></span>|<span data-ttu-id="85506-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="85506-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85506-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="85506-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="85506-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="85506-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="85506-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="85506-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="85506-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="85506-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="85506-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="85506-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="85506-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="85506-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="85506-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="85506-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="85506-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="85506-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="85506-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="85506-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="85506-157">SyncState</span><span class="sxs-lookup"><span data-stu-id="85506-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="85506-158">Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="85506-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="85506-159">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="85506-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="85506-160">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="85506-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="85506-161">Indique si le dernier élément à synchroniser a été inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="85506-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="85506-162">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="85506-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="85506-163">Contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="85506-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85506-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85506-164">Parent elements</span></span>

|<span data-ttu-id="85506-165">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85506-165">**Element**</span></span>|<span data-ttu-id="85506-166">**Description**</span><span class="sxs-lookup"><span data-stu-id="85506-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85506-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="85506-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="85506-168">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="85506-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85506-169">Remarques</span><span class="sxs-lookup"><span data-stu-id="85506-169">Remarks</span></span>

<span data-ttu-id="85506-170">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="85506-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85506-171">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85506-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85506-172">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85506-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="85506-173">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85506-173">Schema Name</span></span>  <br/> |<span data-ttu-id="85506-174">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="85506-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="85506-175">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85506-175">Validation File</span></span>  <br/> |<span data-ttu-id="85506-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="85506-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="85506-177">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85506-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="85506-178">False</span><span class="sxs-lookup"><span data-stu-id="85506-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85506-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85506-179">See also</span></span>

- [<span data-ttu-id="85506-180">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="85506-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="85506-181">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85506-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

