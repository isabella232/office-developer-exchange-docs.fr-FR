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
description: L’élément CopyFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération CopyFolder.
ms.openlocfilehash: 796ec57116e4b4943ca370e45cf0abefe7782c08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458508"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="1324d-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1324d-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="1324d-104">L’élément **CopyFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1324d-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="1324d-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="1324d-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="1324d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1324d-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="1324d-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1324d-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="1324d-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1324d-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1324d-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1324d-109">Attributes and elements</span></span>

<span data-ttu-id="1324d-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1324d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1324d-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="1324d-111">Attributes</span></span>

|<span data-ttu-id="1324d-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1324d-112">**Attribute**</span></span>|<span data-ttu-id="1324d-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="1324d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1324d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1324d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1324d-115">Décrit l’état d’une réponse d' [opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1324d-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="1324d-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="1324d-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="1324d-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="1324d-117">- Success</span></span>  <br/><span data-ttu-id="1324d-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="1324d-118">-  Warning</span></span>  <br/><span data-ttu-id="1324d-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="1324d-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1324d-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="1324d-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="1324d-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1324d-121">**Value**</span></span>|<span data-ttu-id="1324d-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="1324d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1324d-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="1324d-123">**Success**</span></span> <br/> |<span data-ttu-id="1324d-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1324d-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1324d-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1324d-125">**Warning**</span></span> <br/> | <span data-ttu-id="1324d-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="1324d-126">Describes a request that was not processed.</span></span> <span data-ttu-id="1324d-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="1324d-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="1324d-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="1324d-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="1324d-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="1324d-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="1324d-130">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1324d-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="1324d-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="1324d-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="1324d-132">-La base de données de messages (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="1324d-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="1324d-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="1324d-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="1324d-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="1324d-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="1324d-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="1324d-135">**Error**</span></span> <br/> | <span data-ttu-id="1324d-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="1324d-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="1324d-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="1324d-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1324d-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="1324d-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1324d-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="1324d-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1324d-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="1324d-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="1324d-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="1324d-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1324d-142">-Accès non autorisé tenté par un client</span><span class="sxs-lookup"><span data-stu-id="1324d-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="1324d-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="1324d-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="1324d-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="1324d-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1324d-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1324d-145">Child elements</span></span>

|<span data-ttu-id="1324d-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1324d-146">**Element**</span></span>|<span data-ttu-id="1324d-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="1324d-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1324d-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="1324d-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1324d-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1324d-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1324d-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1324d-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1324d-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="1324d-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1324d-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1324d-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1324d-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="1324d-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="1324d-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="1324d-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1324d-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1324d-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1324d-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="1324d-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1324d-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="1324d-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1324d-158">Contient un tableau de dossiers copiés.</span><span class="sxs-lookup"><span data-stu-id="1324d-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1324d-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1324d-159">Parent elements</span></span>

|<span data-ttu-id="1324d-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1324d-160">**Element**</span></span>|<span data-ttu-id="1324d-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="1324d-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1324d-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1324d-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1324d-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1324d-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1324d-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="1324d-164">Remarks</span></span>

<span data-ttu-id="1324d-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1324d-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1324d-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1324d-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1324d-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1324d-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1324d-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1324d-168">Schema name</span></span>  <br/> |<span data-ttu-id="1324d-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1324d-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1324d-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1324d-170">Validation file</span></span>  <br/> |<span data-ttu-id="1324d-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1324d-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1324d-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1324d-172">Can be empty</span></span>  <br/> |<span data-ttu-id="1324d-173">False</span><span class="sxs-lookup"><span data-stu-id="1324d-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1324d-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1324d-174">See also</span></span>

- [<span data-ttu-id="1324d-175">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="1324d-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="1324d-176">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1324d-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="1324d-177">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1324d-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

