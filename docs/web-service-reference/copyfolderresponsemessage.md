---
title: CopyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: L’élément CopyFolderResponseMessage contient l’état et les résultats d’une demande d’opération CopyFolder unique.
ms.openlocfilehash: 2bb2b407e0ae6b854d214c4b9d68ac8ed65b2c7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755665"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="b5133-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b5133-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="b5133-104">L’élément **CopyFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b5133-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b5133-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b5133-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="b5133-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b5133-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="b5133-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b5133-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="b5133-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b5133-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5133-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b5133-109">Attributes and elements</span></span>

<span data-ttu-id="b5133-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b5133-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5133-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="b5133-111">Attributes</span></span>

|<span data-ttu-id="b5133-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b5133-112">**Attribute**</span></span>|<span data-ttu-id="b5133-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5133-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5133-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b5133-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b5133-115">Décrit l’état d’une réponse de [l’opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b5133-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="b5133-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b5133-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="b5133-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b5133-117">- Success</span></span>  <br/><span data-ttu-id="b5133-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="b5133-118">-  Warning</span></span>  <br/><span data-ttu-id="b5133-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b5133-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b5133-120">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b5133-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="b5133-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b5133-121">**Value**</span></span>|<span data-ttu-id="b5133-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5133-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5133-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="b5133-123">**Success**</span></span> <br/> |<span data-ttu-id="b5133-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="b5133-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b5133-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="b5133-125">**Warning**</span></span> <br/> | <span data-ttu-id="b5133-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="b5133-126">Describes a request that was not processed.</span></span> <span data-ttu-id="b5133-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="b5133-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="b5133-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b5133-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="b5133-129">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b5133-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="b5133-130">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b5133-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="b5133-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="b5133-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b5133-132">-La base de données de message (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b5133-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="b5133-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b5133-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="b5133-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="b5133-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b5133-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="b5133-135">**Error**</span></span> <br/> | <span data-ttu-id="b5133-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="b5133-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="b5133-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b5133-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b5133-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="b5133-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b5133-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="b5133-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b5133-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b5133-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="b5133-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b5133-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b5133-142">-Accès non autorisé a tenté par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="b5133-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="b5133-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="b5133-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="b5133-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b5133-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b5133-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b5133-145">Child elements</span></span>

|<span data-ttu-id="b5133-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b5133-146">**Element**</span></span>|<span data-ttu-id="b5133-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5133-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5133-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="b5133-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b5133-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b5133-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b5133-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b5133-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b5133-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="b5133-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b5133-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b5133-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b5133-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="b5133-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b5133-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b5133-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b5133-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b5133-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b5133-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b5133-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b5133-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="b5133-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b5133-158">Contient un tableau des dossiers copiés.</span><span class="sxs-lookup"><span data-stu-id="b5133-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b5133-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b5133-159">Parent elements</span></span>

|<span data-ttu-id="b5133-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b5133-160">**Element**</span></span>|<span data-ttu-id="b5133-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5133-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5133-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b5133-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b5133-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5133-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b5133-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="b5133-164">Remarks</span></span>

<span data-ttu-id="b5133-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b5133-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5133-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b5133-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5133-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b5133-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b5133-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b5133-168">Schema name</span></span>  <br/> |<span data-ttu-id="b5133-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b5133-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b5133-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b5133-170">Validation file</span></span>  <br/> |<span data-ttu-id="b5133-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b5133-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b5133-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b5133-172">Can be empty</span></span>  <br/> |<span data-ttu-id="b5133-173">False</span><span class="sxs-lookup"><span data-stu-id="b5133-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5133-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b5133-174">See also</span></span>

- [<span data-ttu-id="b5133-175">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="b5133-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="b5133-176">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b5133-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="b5133-177">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b5133-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

