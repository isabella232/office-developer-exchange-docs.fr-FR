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
description: L’élément GetFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération GetFolder.
ms.openlocfilehash: ddf23790e804c3f0562f65ebaa3cb591433eab69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456457"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="28187-103">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="28187-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="28187-104">L’élément **GetFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="28187-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="28187-105">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="28187-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="28187-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28187-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="28187-107">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="28187-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="28187-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="28187-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28187-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28187-109">Attributes and elements</span></span>

<span data-ttu-id="28187-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28187-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28187-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="28187-111">Attributes</span></span>

|<span data-ttu-id="28187-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="28187-112">**Attribute**</span></span>|<span data-ttu-id="28187-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="28187-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28187-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="28187-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="28187-115">Décrit l’état d’une réponse d' [opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="28187-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="28187-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="28187-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="28187-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="28187-117">-  Success</span></span>  <br/><span data-ttu-id="28187-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="28187-118">-  Warning</span></span>  <br/><span data-ttu-id="28187-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="28187-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="28187-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="28187-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="28187-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="28187-121">**Value**</span></span>|<span data-ttu-id="28187-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="28187-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28187-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="28187-123">**Success**</span></span> <br/> |<span data-ttu-id="28187-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="28187-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="28187-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="28187-125">**Warning**</span></span> <br/> | <span data-ttu-id="28187-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="28187-126">Describes a request that was not processed.</span></span> <span data-ttu-id="28187-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="28187-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="28187-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="28187-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="28187-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="28187-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="28187-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="28187-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="28187-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="28187-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="28187-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="28187-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="28187-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="28187-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="28187-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="28187-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="28187-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="28187-135">**Error**</span></span> <br/> | <span data-ttu-id="28187-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="28187-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="28187-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="28187-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="28187-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="28187-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="28187-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="28187-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="28187-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="28187-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="28187-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="28187-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="28187-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="28187-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="28187-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="28187-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="28187-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="28187-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="28187-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28187-145">Child elements</span></span>

|<span data-ttu-id="28187-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28187-146">**Element**</span></span>|<span data-ttu-id="28187-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="28187-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28187-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="28187-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="28187-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="28187-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="28187-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="28187-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="28187-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="28187-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="28187-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="28187-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="28187-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="28187-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="28187-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="28187-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="28187-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="28187-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="28187-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="28187-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="28187-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="28187-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="28187-158">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="28187-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28187-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28187-159">Parent elements</span></span>

|<span data-ttu-id="28187-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28187-160">**Element**</span></span>|<span data-ttu-id="28187-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="28187-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28187-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28187-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="28187-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28187-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28187-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="28187-164">Remarks</span></span>

<span data-ttu-id="28187-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="28187-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28187-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28187-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28187-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28187-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28187-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28187-168">Schema Name</span></span>  <br/> |<span data-ttu-id="28187-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="28187-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28187-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28187-170">Validation File</span></span>  <br/> |<span data-ttu-id="28187-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28187-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28187-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28187-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="28187-173">False</span><span class="sxs-lookup"><span data-stu-id="28187-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28187-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28187-174">See also</span></span>

- [<span data-ttu-id="28187-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="28187-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="28187-176">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="28187-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="28187-177">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="28187-177">GetFolder operation</span></span>](getfolder-operation.md)

