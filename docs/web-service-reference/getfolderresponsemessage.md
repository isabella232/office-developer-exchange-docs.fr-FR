---
title: GetFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponseMessage
api_type:
- schema
ms.assetid: 51359863-d110-4c12-b89f-aba5e3e40c1d
description: L’élément GetFolderResponseMessage contient l’état et les résultats d’une demande d’opération GetFolder unique.
ms.openlocfilehash: a6b67907dba311a3ce482ff8f524378fb4be9694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756624"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="0ad81-103">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ad81-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="0ad81-104">L’élément **GetFolderResponseMessage** contient l’état et les résultats d’une seule demande [d’opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ad81-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0ad81-105">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0ad81-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="0ad81-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ad81-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0ad81-107">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ad81-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="0ad81-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0ad81-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ad81-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ad81-109">Attributes and elements</span></span>

<span data-ttu-id="0ad81-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ad81-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ad81-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ad81-111">Attributes</span></span>

|<span data-ttu-id="0ad81-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0ad81-112">**Attribute**</span></span>|<span data-ttu-id="0ad81-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ad81-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ad81-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0ad81-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0ad81-115">Décrit l’état d’une réponse de [l’opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0ad81-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0ad81-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="0ad81-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="0ad81-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="0ad81-117">-  Success</span></span>  <br/><span data-ttu-id="0ad81-118">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="0ad81-118">-  Warning</span></span>  <br/><span data-ttu-id="0ad81-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="0ad81-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="0ad81-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0ad81-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="0ad81-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0ad81-121">**Value**</span></span>|<span data-ttu-id="0ad81-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ad81-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ad81-123">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="0ad81-123">**Success**</span></span> <br/> |<span data-ttu-id="0ad81-124">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="0ad81-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0ad81-125">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="0ad81-125">**Warning**</span></span> <br/> | <span data-ttu-id="0ad81-126">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="0ad81-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0ad81-127">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="0ad81-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0ad81-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="0ad81-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0ad81-129">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="0ad81-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0ad81-130">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0ad81-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0ad81-131">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="0ad81-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0ad81-132">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0ad81-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0ad81-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="0ad81-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0ad81-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="0ad81-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="0ad81-135">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="0ad81-135">**Error**</span></span> <br/> | <span data-ttu-id="0ad81-136">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="0ad81-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0ad81-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="0ad81-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0ad81-138">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="0ad81-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0ad81-139">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="0ad81-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="0ad81-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="0ad81-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="0ad81-141">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="0ad81-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="0ad81-142">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="0ad81-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0ad81-143">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="0ad81-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="0ad81-144">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0ad81-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0ad81-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ad81-145">Child elements</span></span>

|<span data-ttu-id="0ad81-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ad81-146">**Element**</span></span>|<span data-ttu-id="0ad81-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ad81-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ad81-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ad81-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0ad81-149">Fournit le texte de description de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0ad81-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0ad81-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ad81-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0ad81-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="0ad81-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0ad81-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ad81-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0ad81-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="0ad81-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0ad81-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="0ad81-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0ad81-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0ad81-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0ad81-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="0ad81-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0ad81-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="0ad81-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0ad81-158">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="0ad81-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ad81-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ad81-159">Parent elements</span></span>

|<span data-ttu-id="0ad81-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ad81-160">**Element**</span></span>|<span data-ttu-id="0ad81-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ad81-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ad81-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ad81-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0ad81-163">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ad81-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ad81-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ad81-164">Remarks</span></span>

<span data-ttu-id="0ad81-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="0ad81-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ad81-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ad81-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ad81-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ad81-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ad81-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ad81-168">Schema Name</span></span>  <br/> |<span data-ttu-id="0ad81-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0ad81-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ad81-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ad81-170">Validation File</span></span>  <br/> |<span data-ttu-id="0ad81-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ad81-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ad81-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ad81-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ad81-173">False</span><span class="sxs-lookup"><span data-stu-id="0ad81-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ad81-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ad81-174">See also</span></span>

- [<span data-ttu-id="0ad81-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="0ad81-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="0ad81-176">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0ad81-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="0ad81-177">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="0ad81-177">GetFolder operation</span></span>](getfolder-operation.md)

