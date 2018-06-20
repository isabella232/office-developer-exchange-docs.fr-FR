---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: L’élément FindItemResponseMessage contient l’état et les résultats d’une demande d’opération FindItem unique.
ms.openlocfilehash: 0a4bfb3ba8d85b0bff0d03f043be865ce7276229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756404"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="f54e9-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f54e9-103">FindItemResponseMessage</span></span>

<span data-ttu-id="f54e9-104">L’élément **FindItemResponseMessage** contient l’état et les résultats d’une seule demande [d’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f54e9-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f54e9-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="f54e9-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="f54e9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f54e9-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="f54e9-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f54e9-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="f54e9-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f54e9-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f54e9-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f54e9-109">Attributes and elements</span></span>

<span data-ttu-id="f54e9-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f54e9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f54e9-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f54e9-111">Attributes</span></span>

|<span data-ttu-id="f54e9-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f54e9-112">**Attribute**</span></span>|<span data-ttu-id="f54e9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="f54e9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f54e9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f54e9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f54e9-115">Décrit l’état d’une réponse de [l’opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f54e9-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="f54e9-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f54e9-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="f54e9-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f54e9-117">-  Success</span></span>  <br/><span data-ttu-id="f54e9-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="f54e9-118">-  Warning</span></span>  <br/><span data-ttu-id="f54e9-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f54e9-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f54e9-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f54e9-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f54e9-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f54e9-121">**Value**</span></span>|<span data-ttu-id="f54e9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="f54e9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f54e9-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="f54e9-123">**Success**</span></span> <br/> |<span data-ttu-id="f54e9-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="f54e9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f54e9-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="f54e9-125">**Warning**</span></span> <br/> | <span data-ttu-id="f54e9-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="f54e9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f54e9-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite lors du traitement de traitement d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traitées.</span><span class="sxs-lookup"><span data-stu-id="f54e9-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f54e9-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f54e9-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="f54e9-129">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f54e9-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="f54e9-130">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f54e9-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="f54e9-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="f54e9-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f54e9-132">-La base de données de message (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f54e9-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="f54e9-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f54e9-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f54e9-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="f54e9-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="f54e9-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="f54e9-135">**Error**</span></span> <br/> | <span data-ttu-id="f54e9-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="f54e9-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f54e9-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f54e9-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f54e9-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="f54e9-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f54e9-139">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="f54e9-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f54e9-140">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f54e9-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="f54e9-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f54e9-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f54e9-142">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="f54e9-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f54e9-143">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="f54e9-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f54e9-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f54e9-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f54e9-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f54e9-145">Child elements</span></span>

|<span data-ttu-id="f54e9-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f54e9-146">**Element**</span></span>|<span data-ttu-id="f54e9-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="f54e9-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f54e9-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="f54e9-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f54e9-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f54e9-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f54e9-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f54e9-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f54e9-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="f54e9-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f54e9-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f54e9-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f54e9-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="f54e9-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f54e9-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f54e9-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f54e9-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f54e9-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f54e9-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="f54e9-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f54e9-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="f54e9-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="f54e9-158">Contient les résultats de la recherche d’un dossier racine unique lors d’une [opération FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f54e9-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f54e9-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f54e9-159">Parent elements</span></span>

|<span data-ttu-id="f54e9-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f54e9-160">**Element**</span></span>|<span data-ttu-id="f54e9-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="f54e9-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f54e9-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f54e9-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f54e9-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f54e9-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f54e9-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="f54e9-164">Remarks</span></span>

<span data-ttu-id="f54e9-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="f54e9-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f54e9-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f54e9-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f54e9-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f54e9-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f54e9-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f54e9-168">Schema name</span></span>  <br/> |<span data-ttu-id="f54e9-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f54e9-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f54e9-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f54e9-170">Validation file</span></span>  <br/> |<span data-ttu-id="f54e9-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f54e9-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f54e9-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f54e9-172">Can be empty</span></span>  <br/> |<span data-ttu-id="f54e9-173">False</span><span class="sxs-lookup"><span data-stu-id="f54e9-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f54e9-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f54e9-174">See also</span></span>

- [<span data-ttu-id="f54e9-175">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="f54e9-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="f54e9-176">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="f54e9-176">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

