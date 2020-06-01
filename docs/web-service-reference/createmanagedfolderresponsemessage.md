---
title: CreateManagedFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponseMessage
api_type:
- schema
ms.assetid: a72eefc3-ef0b-4b44-a74b-e6907b5b5f68
description: L’élément CreateManagedFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération CreateManagedFolder.
ms.openlocfilehash: 03ebcaeb79b2fac20882d2cea3d1e24b42dd472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467703"
---
# <a name="createmanagedfolderresponsemessage"></a><span data-ttu-id="f8ee9-103">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f8ee9-103">CreateManagedFolderResponseMessage</span></span>

<span data-ttu-id="f8ee9-104">L’élément **CreateManagedFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f8ee9-104">The **CreateManagedFolderResponseMessage** element contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f8ee9-105">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f8ee9-105">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)  
- [<span data-ttu-id="f8ee9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f8ee9-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="f8ee9-107">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f8ee9-107">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

<span data-ttu-id="f8ee9-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-108">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f8ee9-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f8ee9-109">Attributes and elements</span></span>

<span data-ttu-id="f8ee9-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8ee9-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f8ee9-111">Attributes</span></span>

|<span data-ttu-id="f8ee9-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-112">**Attribute**</span></span>|<span data-ttu-id="f8ee9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8ee9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f8ee9-115">Décrit l’état d’une réponse d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f8ee9-115">Describes the status of a [CreateManagedFolder operation](createmanagedfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="f8ee9-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f8ee9-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="f8ee9-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f8ee9-117">-  Success</span></span>  <br/><span data-ttu-id="f8ee9-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="f8ee9-118">-  Warning</span></span>  <br/><span data-ttu-id="f8ee9-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f8ee9-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f8ee9-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f8ee9-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f8ee9-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-121">**Value**</span></span>|<span data-ttu-id="f8ee9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8ee9-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-123">**Success**</span></span> <br/> |<span data-ttu-id="f8ee9-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f8ee9-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-125">**Warning**</span></span> <br/> | <span data-ttu-id="f8ee9-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f8ee9-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="f8ee9-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f8ee9-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="f8ee9-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f8ee9-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f8ee9-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f8ee9-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f8ee9-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f8ee9-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="f8ee9-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-135">**Error**</span></span> <br/> | <span data-ttu-id="f8ee9-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="f8ee9-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f8ee9-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f8ee9-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="f8ee9-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f8ee9-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="f8ee9-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f8ee9-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f8ee9-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="f8ee9-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f8ee9-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f8ee9-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="f8ee9-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f8ee9-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="f8ee9-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="f8ee9-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f8ee9-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f8ee9-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f8ee9-145">Child elements</span></span>

|<span data-ttu-id="f8ee9-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-146">**Element**</span></span>|<span data-ttu-id="f8ee9-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ee9-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="f8ee9-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f8ee9-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f8ee9-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f8ee9-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f8ee9-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f8ee9-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f8ee9-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f8ee9-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f8ee9-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f8ee9-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f8ee9-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f8ee9-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f8ee9-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="f8ee9-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f8ee9-158">Contient un tableau de dossiers gérés créés.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-158">Contains an array of created managed folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8ee9-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f8ee9-159">Parent elements</span></span>

|<span data-ttu-id="f8ee9-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-160">**Element**</span></span>|<span data-ttu-id="f8ee9-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ee9-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ee9-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f8ee9-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f8ee9-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8ee9-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="f8ee9-164">Remarks</span></span>

<span data-ttu-id="f8ee9-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f8ee9-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8ee9-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f8ee9-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8ee9-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f8ee9-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8ee9-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f8ee9-168">Schema Name</span></span>  <br/> |<span data-ttu-id="f8ee9-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f8ee9-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8ee9-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f8ee9-170">Validation File</span></span>  <br/> |<span data-ttu-id="f8ee9-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f8ee9-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8ee9-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f8ee9-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8ee9-173">False</span><span class="sxs-lookup"><span data-stu-id="f8ee9-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8ee9-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8ee9-174">See also</span></span>

- [<span data-ttu-id="f8ee9-175">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="f8ee9-175">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
- [<span data-ttu-id="f8ee9-176">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="f8ee9-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="f8ee9-177">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f8ee9-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

