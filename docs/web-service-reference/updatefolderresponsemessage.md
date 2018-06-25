---
title: UpdateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolderResponseMessage
api_type:
- schema
ms.assetid: 914bb683-49ee-44a2-b59d-ef560244dfb8
description: L’élément UpdateFolderResponseMessage contient l’état et les résultats des mises à jour définie par l’élément FolderChange d’une demande d’opération UpdateFolder.
ms.openlocfilehash: 4cd00232bcc233f6534d844418f523c248ce54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838876"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="fc948-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fc948-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="fc948-104">L’élément **UpdateFolderResponseMessage** contient l’état et les résultats des mises à jour définie par l’élément [FolderChange](folderchange.md) d’une demande [d’opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fc948-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="fc948-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="fc948-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="fc948-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fc948-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="fc948-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fc948-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="fc948-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fc948-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc948-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fc948-109">Attributes and elements</span></span>

<span data-ttu-id="fc948-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fc948-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc948-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="fc948-111">Attributes</span></span>

|<span data-ttu-id="fc948-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fc948-112">**Attribute**</span></span>|<span data-ttu-id="fc948-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc948-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fc948-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="fc948-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="fc948-115">Décrit l’état d’une réponse de [l’opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fc948-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="fc948-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="fc948-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="fc948-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="fc948-117">-  Success</span></span>  <br/><span data-ttu-id="fc948-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="fc948-118">-  Warning</span></span>  <br/><span data-ttu-id="fc948-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="fc948-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="fc948-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fc948-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="fc948-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fc948-121">**Value**</span></span>|<span data-ttu-id="fc948-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc948-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fc948-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="fc948-123">**Success**</span></span> <br/> |<span data-ttu-id="fc948-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="fc948-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="fc948-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="fc948-125">**Warning**</span></span> <br/> | <span data-ttu-id="fc948-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="fc948-126">Describes a request that was not processed.</span></span> <span data-ttu-id="fc948-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="fc948-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="fc948-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="fc948-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="fc948-129">-La banque d’informations Exchange est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="fc948-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="fc948-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="fc948-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="fc948-131">-Une boîte aux lettres est déplacée.</span><span class="sxs-lookup"><span data-stu-id="fc948-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="fc948-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="fc948-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="fc948-133">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="fc948-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="fc948-134">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="fc948-134">**Error**</span></span> <br/> | <span data-ttu-id="fc948-135">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="fc948-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="fc948-136">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="fc948-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="fc948-137">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="fc948-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="fc948-138">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="fc948-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="fc948-139">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="fc948-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="fc948-140">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="fc948-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="fc948-141">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="fc948-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="fc948-142">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="fc948-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="fc948-143">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="fc948-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fc948-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fc948-144">Child elements</span></span>

|<span data-ttu-id="fc948-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc948-145">**Element**</span></span>|<span data-ttu-id="fc948-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc948-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc948-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="fc948-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fc948-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="fc948-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fc948-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fc948-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fc948-150">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="fc948-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="fc948-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fc948-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fc948-152">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="fc948-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="fc948-153">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="fc948-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="fc948-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fc948-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fc948-155">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="fc948-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fc948-156">Dossiers</span><span class="sxs-lookup"><span data-stu-id="fc948-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="fc948-157">Contient un tableau des dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="fc948-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc948-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fc948-158">Parent elements</span></span>

|<span data-ttu-id="fc948-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc948-159">**Element**</span></span>|<span data-ttu-id="fc948-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc948-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc948-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fc948-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fc948-162">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc948-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc948-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="fc948-163">Remarks</span></span>

<span data-ttu-id="fc948-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="fc948-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc948-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fc948-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc948-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fc948-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc948-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fc948-167">Schema Name</span></span>  <br/> |<span data-ttu-id="fc948-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fc948-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc948-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fc948-169">Validation File</span></span>  <br/> |<span data-ttu-id="fc948-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc948-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc948-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fc948-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc948-172">False</span><span class="sxs-lookup"><span data-stu-id="fc948-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc948-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc948-173">See also</span></span>

- [<span data-ttu-id="fc948-174">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fc948-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

