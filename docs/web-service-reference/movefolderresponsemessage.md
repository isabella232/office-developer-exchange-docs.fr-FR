---
title: MoveFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: L’élément MoveFolderResponseMessage contient l’état et les résultats d’une demande d’opération MoveFolder unique.
ms.openlocfilehash: 777520bf6a093882da95a7bfd466b66acdab957c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828496"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="6adec-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6adec-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="6adec-104">L’élément **MoveFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6adec-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="6adec-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="6adec-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="6adec-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6adec-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="6adec-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6adec-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="6adec-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6adec-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6adec-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6adec-109">Attributes and elements</span></span>

<span data-ttu-id="6adec-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6adec-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6adec-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="6adec-111">Attributes</span></span>

|<span data-ttu-id="6adec-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6adec-112">**Attribute**</span></span>|<span data-ttu-id="6adec-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adec-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6adec-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6adec-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6adec-115">Décrit l’état d’une réponse de [l’opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6adec-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="6adec-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="6adec-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6adec-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="6adec-117">-  Success</span></span>  <br/><span data-ttu-id="6adec-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="6adec-118">-  Warning</span></span>  <br/><span data-ttu-id="6adec-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="6adec-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="6adec-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6adec-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="6adec-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6adec-121">**Value**</span></span>|<span data-ttu-id="6adec-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adec-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6adec-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="6adec-123">**Success**</span></span> <br/> |<span data-ttu-id="6adec-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="6adec-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6adec-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="6adec-125">**Warning**</span></span> <br/> | <span data-ttu-id="6adec-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="6adec-126">Describes a request that was not processed.</span></span> <span data-ttu-id="6adec-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="6adec-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="6adec-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="6adec-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="6adec-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="6adec-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6adec-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6adec-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6adec-131">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="6adec-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="6adec-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="6adec-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6adec-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="6adec-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="6adec-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="6adec-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="6adec-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="6adec-135">**Error**</span></span> <br/> | <span data-ttu-id="6adec-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="6adec-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6adec-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="6adec-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="6adec-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="6adec-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6adec-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="6adec-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6adec-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="6adec-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="6adec-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="6adec-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6adec-142">-Toute tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="6adec-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6adec-143">-Tout échec de côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="6adec-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="6adec-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6adec-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6adec-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6adec-145">Child elements</span></span>

|<span data-ttu-id="6adec-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6adec-146">**Element**</span></span>|<span data-ttu-id="6adec-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adec-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6adec-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="6adec-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6adec-149">Une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="6adec-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6adec-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6adec-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6adec-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="6adec-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6adec-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6adec-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6adec-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="6adec-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6adec-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="6adec-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6adec-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6adec-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6adec-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="6adec-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6adec-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="6adec-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6adec-158">Contient un tableau des dossiers déplacés.</span><span class="sxs-lookup"><span data-stu-id="6adec-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6adec-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6adec-159">Parent elements</span></span>

|<span data-ttu-id="6adec-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6adec-160">**Element**</span></span>|<span data-ttu-id="6adec-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adec-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6adec-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6adec-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6adec-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6adec-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6adec-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="6adec-164">Remarks</span></span>

<span data-ttu-id="6adec-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6adec-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6adec-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6adec-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6adec-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6adec-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6adec-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6adec-168">Schema Name</span></span>  <br/> |<span data-ttu-id="6adec-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6adec-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6adec-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6adec-170">Validation File</span></span>  <br/> |<span data-ttu-id="6adec-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6adec-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6adec-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6adec-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="6adec-173">False</span><span class="sxs-lookup"><span data-stu-id="6adec-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6adec-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6adec-174">See also</span></span>

- [<span data-ttu-id="6adec-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="6adec-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="6adec-176">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="6adec-176">MoveFolder operation</span></span>](movefolder-operation.md)

