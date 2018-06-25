---
title: CreateFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolderResponseMessage
api_type:
- schema
ms.assetid: 1301dd15-b008-4fd9-8c89-b15a20b186e2
description: L’élément CreateFolderResponseMessage contient l’état et les résultats d’une demande d’opération CreateFolder unique.
ms.openlocfilehash: c587cca1f935b295a0ed30ab2210de40af28d06d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755710"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="9366e-103">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9366e-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="9366e-104">L’élément **CreateFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9366e-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="9366e-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9366e-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9366e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9366e-106">Attributes and elements</span></span>

<span data-ttu-id="9366e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9366e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9366e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9366e-108">Attributes</span></span>

|<span data-ttu-id="9366e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9366e-109">**Attribute**</span></span>|<span data-ttu-id="9366e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9366e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9366e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9366e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9366e-112">Décrit l’état d’une réponse de [l’opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9366e-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="9366e-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="9366e-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="9366e-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="9366e-114">-  Success</span></span>  <br/><span data-ttu-id="9366e-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="9366e-115">-  Warning</span></span>  <br/><span data-ttu-id="9366e-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="9366e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9366e-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9366e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9366e-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9366e-118">**Value**</span></span>|<span data-ttu-id="9366e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="9366e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9366e-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="9366e-120">**Success**</span></span> <br/> |<span data-ttu-id="9366e-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="9366e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9366e-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="9366e-122">**Warning**</span></span> <br/> | <span data-ttu-id="9366e-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="9366e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9366e-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="9366e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="9366e-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="9366e-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="9366e-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="9366e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9366e-127">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="9366e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9366e-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="9366e-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="9366e-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="9366e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9366e-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="9366e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9366e-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="9366e-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="9366e-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="9366e-132">**Error**</span></span> <br/> | <span data-ttu-id="9366e-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="9366e-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="9366e-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="9366e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9366e-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="9366e-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9366e-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="9366e-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="9366e-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="9366e-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="9366e-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="9366e-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="9366e-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="9366e-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9366e-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="9366e-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="9366e-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9366e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9366e-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9366e-142">Child elements</span></span>

|<span data-ttu-id="9366e-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9366e-143">**Element**</span></span>|<span data-ttu-id="9366e-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="9366e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9366e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9366e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9366e-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="9366e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9366e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9366e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9366e-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="9366e-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9366e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9366e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9366e-150">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="9366e-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9366e-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="9366e-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9366e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9366e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9366e-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="9366e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9366e-154">Dossiers</span><span class="sxs-lookup"><span data-stu-id="9366e-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9366e-155">Contient un tableau des dossiers créés.</span><span class="sxs-lookup"><span data-stu-id="9366e-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9366e-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9366e-156">Parent elements</span></span>

|<span data-ttu-id="9366e-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9366e-157">**Element**</span></span>|<span data-ttu-id="9366e-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="9366e-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9366e-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9366e-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9366e-160">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9366e-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9366e-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="9366e-161">Remarks</span></span>

<span data-ttu-id="9366e-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="9366e-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9366e-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9366e-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9366e-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9366e-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9366e-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9366e-165">Schema Name</span></span>  <br/> |<span data-ttu-id="9366e-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9366e-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9366e-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9366e-167">Validation File</span></span>  <br/> |<span data-ttu-id="9366e-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9366e-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9366e-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9366e-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="9366e-170">False</span><span class="sxs-lookup"><span data-stu-id="9366e-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9366e-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9366e-171">See also</span></span>

- [<span data-ttu-id="9366e-172">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9366e-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="9366e-173">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="9366e-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="9366e-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9366e-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

