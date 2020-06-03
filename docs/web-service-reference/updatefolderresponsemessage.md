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
description: L’élément UpdateFolderResponseMessage contient l’État et le résultat des mises à jour définies par l’élément FolderChange, d’une demande d’opération UpdateFolder.
ms.openlocfilehash: bbe01583072e6203e099d440f2a171012f51e7df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466583"
---
# <a name="updatefolderresponsemessage"></a><span data-ttu-id="a71b4-103">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a71b4-103">UpdateFolderResponseMessage</span></span>

<span data-ttu-id="a71b4-104">L’élément **UpdateFolderResponseMessage** contient l’État et le résultat des mises à jour définies par l’élément [FolderChange,](folderchange.md) d’une demande d' [opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a71b4-104">The **UpdateFolderResponseMessage** element contains the status and result of updates defined by the [FolderChange](folderchange.md) element of an [UpdateFolder operation](updatefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a71b4-105">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="a71b4-105">UpdateFolderResponse</span></span>](updatefolderresponse.md) 
- [<span data-ttu-id="a71b4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a71b4-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a71b4-107">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a71b4-107">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
  
```xml
<UpdateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</UpdateFolderResponseMessage>
```

 <span data-ttu-id="a71b4-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a71b4-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a71b4-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a71b4-109">Attributes and elements</span></span>

<span data-ttu-id="a71b4-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a71b4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a71b4-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="a71b4-111">Attributes</span></span>

|<span data-ttu-id="a71b4-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a71b4-112">**Attribute**</span></span>|<span data-ttu-id="a71b4-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a71b4-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a71b4-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a71b4-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a71b4-115">Décrit l’état d’une réponse d' [opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a71b4-115">Describes the status of an [UpdateFolder operation](updatefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a71b4-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="a71b4-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="a71b4-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="a71b4-117">-  Success</span></span>  <br/><span data-ttu-id="a71b4-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="a71b4-118">-  Warning</span></span>  <br/><span data-ttu-id="a71b4-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="a71b4-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a71b4-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a71b4-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a71b4-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a71b4-121">**Value**</span></span>|<span data-ttu-id="a71b4-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="a71b4-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a71b4-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="a71b4-123">**Success**</span></span> <br/> |<span data-ttu-id="a71b4-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="a71b4-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a71b4-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="a71b4-125">**Warning**</span></span> <br/> | <span data-ttu-id="a71b4-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="a71b4-126">Describes a request that was not processed.</span></span> <span data-ttu-id="a71b4-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="a71b4-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="a71b4-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="a71b4-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="a71b4-129">-La banque Exchange est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a71b4-129">-  The Exchange store is offline.</span></span>  <br/><span data-ttu-id="a71b4-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="a71b4-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a71b4-131">-Une boîte aux lettres est déplacée.</span><span class="sxs-lookup"><span data-stu-id="a71b4-131">-  A mailbox is moved.</span></span>  <br/><span data-ttu-id="a71b4-132">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="a71b4-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="a71b4-133">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="a71b4-133">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="a71b4-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="a71b4-134">**Error**</span></span> <br/> | <span data-ttu-id="a71b4-135">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="a71b4-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="a71b4-136">Voici des exemples de sources pour les erreurs :</span><span class="sxs-lookup"><span data-stu-id="a71b4-136">The following are examples of sources for errors:</span></span>  <br/><br/><span data-ttu-id="a71b4-137">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="a71b4-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a71b4-138">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="a71b4-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a71b4-139">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="a71b4-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="a71b4-140">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="a71b4-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a71b4-141">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="a71b4-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a71b4-142">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="a71b4-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="a71b4-143">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a71b4-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a71b4-144">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a71b4-144">Child elements</span></span>

|<span data-ttu-id="a71b4-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a71b4-145">**Element**</span></span>|<span data-ttu-id="a71b4-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="a71b4-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a71b4-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="a71b4-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a71b4-148">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="a71b4-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a71b4-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a71b4-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a71b4-150">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="a71b4-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a71b4-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a71b4-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a71b4-152">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="a71b4-152">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a71b4-153">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="a71b4-153">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a71b4-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a71b4-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a71b4-155">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="a71b4-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a71b4-156">Dossiers</span><span class="sxs-lookup"><span data-stu-id="a71b4-156">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a71b4-157">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="a71b4-157">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a71b4-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a71b4-158">Parent elements</span></span>

|<span data-ttu-id="a71b4-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a71b4-159">**Element**</span></span>|<span data-ttu-id="a71b4-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="a71b4-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a71b4-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a71b4-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a71b4-162">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a71b4-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a71b4-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="a71b4-163">Remarks</span></span>

<span data-ttu-id="a71b4-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a71b4-164">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a71b4-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a71b4-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a71b4-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a71b4-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a71b4-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a71b4-167">Schema Name</span></span>  <br/> |<span data-ttu-id="a71b4-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a71b4-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a71b4-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a71b4-169">Validation File</span></span>  <br/> |<span data-ttu-id="a71b4-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a71b4-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a71b4-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a71b4-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="a71b4-172">False</span><span class="sxs-lookup"><span data-stu-id="a71b4-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a71b4-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a71b4-173">See also</span></span>

- [<span data-ttu-id="a71b4-174">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a71b4-174">UpdateFolder operation</span></span>](updatefolder-operation.md)

