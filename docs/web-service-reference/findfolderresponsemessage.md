---
title: FindFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponseMessage
api_type:
- schema
ms.assetid: 538d64fe-51ae-41d2-bfab-91698678aa1b
description: L’élément FindFolderResponseMessage contient l’état et les résultats d’une demande d’opération FindFolder unique.
ms.openlocfilehash: 5623e5e538e617e5bd4bbc4444328ac83d7b8065
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756393"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="ec519-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec519-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="ec519-104">L’élément **FindFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ec519-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="ec519-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ec519-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="ec519-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec519-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="ec519-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec519-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="ec519-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ec519-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec519-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec519-109">Attributes and elements</span></span>

<span data-ttu-id="ec519-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec519-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec519-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec519-111">Attributes</span></span>

|<span data-ttu-id="ec519-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="ec519-112">**Attribute**</span></span>|<span data-ttu-id="ec519-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec519-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec519-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ec519-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ec519-115">Décrit l’état d’une réponse de [l’opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="ec519-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="ec519-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="ec519-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="ec519-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="ec519-117">-  Success</span></span>  <br/><span data-ttu-id="ec519-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="ec519-118">-  Warning</span></span>  <br/><span data-ttu-id="ec519-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="ec519-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="ec519-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ec519-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="ec519-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="ec519-121">**Value**</span></span>|<span data-ttu-id="ec519-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec519-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ec519-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="ec519-123">**Success**</span></span> <br/> |<span data-ttu-id="ec519-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="ec519-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ec519-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="ec519-125">**Warning**</span></span> <br/> | <span data-ttu-id="ec519-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="ec519-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ec519-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="ec519-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ec519-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="ec519-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="ec519-129">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="ec519-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="ec519-130">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ec519-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="ec519-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="ec519-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="ec519-132">-La base de données de message (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="ec519-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="ec519-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="ec519-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="ec519-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="ec519-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="ec519-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="ec519-135">**Error**</span></span> <br/> | <span data-ttu-id="ec519-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="ec519-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ec519-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="ec519-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="ec519-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="ec519-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ec519-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="ec519-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ec519-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="ec519-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="ec519-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="ec519-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="ec519-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="ec519-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ec519-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="ec519-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ec519-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="ec519-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ec519-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec519-145">Child elements</span></span>

|<span data-ttu-id="ec519-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec519-146">**Element**</span></span>|<span data-ttu-id="ec519-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec519-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec519-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ec519-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ec519-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ec519-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ec519-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ec519-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ec519-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="ec519-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ec519-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ec519-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ec519-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="ec519-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ec519-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="ec519-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ec519-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ec519-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ec519-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="ec519-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ec519-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ec519-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="ec519-158">Contient les résultats de la recherche d’un dossier racine unique lors d’une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ec519-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec519-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec519-159">Parent elements</span></span>

|<span data-ttu-id="ec519-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec519-160">**Element**</span></span>|<span data-ttu-id="ec519-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec519-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec519-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec519-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ec519-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec519-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ec519-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec519-164">Remarks</span></span>

<span data-ttu-id="ec519-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec519-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec519-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec519-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec519-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec519-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec519-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec519-168">Schema name</span></span>  <br/> |<span data-ttu-id="ec519-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ec519-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec519-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec519-170">Validation file</span></span>  <br/> |<span data-ttu-id="ec519-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec519-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec519-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec519-172">Can be empty</span></span>  <br/> |<span data-ttu-id="ec519-173">False</span><span class="sxs-lookup"><span data-stu-id="ec519-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec519-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec519-174">See also</span></span>

- [<span data-ttu-id="ec519-175">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="ec519-175">FindFolder operation</span></span>](findfolder-operation.md)
- [<span data-ttu-id="ec519-176">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="ec519-176">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

