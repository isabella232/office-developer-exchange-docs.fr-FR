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
description: L’élément CreateFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération CreateFolder.
ms.openlocfilehash: 386dd2aa4e114d8382d5c83a3d6da70b1ccbbada
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457528"
---
# <a name="createfolderresponsemessage"></a><span data-ttu-id="aa779-103">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aa779-103">CreateFolderResponseMessage</span></span>

<span data-ttu-id="aa779-104">L’élément **CreateFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa779-104">The **CreateFolderResponseMessage** element contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span> 
  
```xml
<CreateFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateFolderResponseMessage>
```

<span data-ttu-id="aa779-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="aa779-105">**FolderInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="aa779-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aa779-106">Attributes and elements</span></span>

<span data-ttu-id="aa779-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aa779-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa779-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aa779-108">Attributes</span></span>

|<span data-ttu-id="aa779-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="aa779-109">**Attribute**</span></span>|<span data-ttu-id="aa779-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa779-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa779-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="aa779-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="aa779-112">Décrit l’état d’une réponse d' [opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="aa779-112">Describes the status of a [CreateFolder operation](createfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="aa779-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="aa779-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="aa779-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="aa779-114">-  Success</span></span>  <br/><span data-ttu-id="aa779-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="aa779-115">-  Warning</span></span>  <br/><span data-ttu-id="aa779-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="aa779-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="aa779-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="aa779-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="aa779-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="aa779-118">**Value**</span></span>|<span data-ttu-id="aa779-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa779-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aa779-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="aa779-120">**Success**</span></span> <br/> |<span data-ttu-id="aa779-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="aa779-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="aa779-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="aa779-122">**Warning**</span></span> <br/> | <span data-ttu-id="aa779-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="aa779-123">Describes a request that was not processed.</span></span> <span data-ttu-id="aa779-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="aa779-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="aa779-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="aa779-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="aa779-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="aa779-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="aa779-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="aa779-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="aa779-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="aa779-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="aa779-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="aa779-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="aa779-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="aa779-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="aa779-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="aa779-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="aa779-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="aa779-132">**Error**</span></span> <br/> | <span data-ttu-id="aa779-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="aa779-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="aa779-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="aa779-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="aa779-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="aa779-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="aa779-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="aa779-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="aa779-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="aa779-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="aa779-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="aa779-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="aa779-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="aa779-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="aa779-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="aa779-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="aa779-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="aa779-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aa779-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aa779-142">Child elements</span></span>

|<span data-ttu-id="aa779-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aa779-143">**Element**</span></span>|<span data-ttu-id="aa779-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa779-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa779-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="aa779-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="aa779-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="aa779-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="aa779-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="aa779-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="aa779-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="aa779-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="aa779-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="aa779-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="aa779-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="aa779-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="aa779-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="aa779-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="aa779-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="aa779-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="aa779-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="aa779-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="aa779-154">Dossiers</span><span class="sxs-lookup"><span data-stu-id="aa779-154">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aa779-155">Contient un tableau de dossiers créés.</span><span class="sxs-lookup"><span data-stu-id="aa779-155">Contains an array of created folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aa779-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aa779-156">Parent elements</span></span>

|<span data-ttu-id="aa779-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aa779-157">**Element**</span></span>|<span data-ttu-id="aa779-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="aa779-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa779-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aa779-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="aa779-160">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa779-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aa779-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="aa779-161">Remarks</span></span>

<span data-ttu-id="aa779-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="aa779-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa779-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aa779-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa779-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aa779-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa779-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aa779-165">Schema Name</span></span>  <br/> |<span data-ttu-id="aa779-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="aa779-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa779-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aa779-167">Validation File</span></span>  <br/> |<span data-ttu-id="aa779-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="aa779-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa779-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aa779-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa779-170">False</span><span class="sxs-lookup"><span data-stu-id="aa779-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa779-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aa779-171">See also</span></span>

- [<span data-ttu-id="aa779-172">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="aa779-172">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="aa779-173">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="aa779-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="aa779-174">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aa779-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

