---
title: GetSharingMetadataResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponse
api_type:
- schema
ms.assetid: 1acc2d8f-7104-4b36-9c04-dd4fc4f571bb
description: L’élément GetSharingMetadataResponse définit une réponse à une demande d’opération GetSharingMetadata.
ms.openlocfilehash: 820b5bf7aa5528b61aa6649e5b1886885b5f022e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827676"
---
# <a name="getsharingmetadataresponse"></a><span data-ttu-id="f1559-103">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="f1559-103">GetSharingMetadataResponse</span></span>

<span data-ttu-id="f1559-104">L’élément **GetSharingMetadataResponse** définit une réponse à une demande [d’opération GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f1559-104">The **GetSharingMetadataResponse** element defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponse>
```

 <span data-ttu-id="f1559-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f1559-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1559-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1559-106">Attributes and elements</span></span>

<span data-ttu-id="f1559-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1559-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1559-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1559-108">Attributes</span></span>

|<span data-ttu-id="f1559-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f1559-109">**Attribute**</span></span>|<span data-ttu-id="f1559-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1559-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1559-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f1559-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f1559-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f1559-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f1559-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f1559-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f1559-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f1559-114">-  Success</span></span>  <br/><span data-ttu-id="f1559-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="f1559-115">-  Warning</span></span>  <br/><span data-ttu-id="f1559-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f1559-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f1559-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f1559-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f1559-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f1559-118">**Value**</span></span>|<span data-ttu-id="f1559-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1559-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1559-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="f1559-120">**Success**</span></span> <br/> |<span data-ttu-id="f1559-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="f1559-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f1559-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="f1559-122">**Warning**</span></span> <br/> | <span data-ttu-id="f1559-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="f1559-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f1559-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="f1559-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f1559-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f1559-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f1559-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f1559-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f1559-127">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f1559-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="f1559-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="f1559-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f1559-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f1559-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f1559-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f1559-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f1559-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="f1559-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f1559-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="f1559-132">**Error**</span></span> <br/> | <span data-ttu-id="f1559-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="f1559-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f1559-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f1559-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f1559-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="f1559-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f1559-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="f1559-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f1559-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f1559-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="f1559-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f1559-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f1559-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="f1559-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f1559-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="f1559-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="f1559-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f1559-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f1559-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1559-142">Child elements</span></span>

|<span data-ttu-id="f1559-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1559-143">**Element**</span></span>|<span data-ttu-id="f1559-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1559-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1559-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f1559-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f1559-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f1559-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f1559-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f1559-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f1559-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="f1559-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f1559-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f1559-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f1559-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="f1559-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f1559-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f1559-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f1559-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f1559-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f1559-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="f1559-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f1559-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="f1559-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="f1559-155">Contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="f1559-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="f1559-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="f1559-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="f1559-157">Représente les destinataires du dossier de demande de partage qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="f1559-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1559-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1559-158">Parent elements</span></span>

<span data-ttu-id="f1559-159">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1559-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1559-160">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1559-160">Remarks</span></span>

<span data-ttu-id="f1559-161">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="f1559-161">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1559-162">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1559-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1559-163">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1559-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1559-164">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1559-164">Schema Name</span></span>  <br/> |<span data-ttu-id="f1559-165">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f1559-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1559-166">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1559-166">Validation File</span></span>  <br/> |<span data-ttu-id="f1559-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f1559-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1559-168">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1559-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1559-169">False</span><span class="sxs-lookup"><span data-stu-id="f1559-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1559-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1559-170">See also</span></span>

- [<span data-ttu-id="f1559-171">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f1559-171">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="f1559-172">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1559-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

