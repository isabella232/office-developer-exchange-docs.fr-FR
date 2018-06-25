---
title: GetSharingMetadataResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponseMessage
api_type:
- schema
ms.assetid: d81b8708-ebb2-45c2-861f-b9a814eee6ba
description: L’élément GetSharingMetadataResponseMessage contient l’état et les résultats d’une demande d’opération GetSharingMetadata unique.
ms.openlocfilehash: 24da0a78870b2c92e0751eba0631d58076b96eae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827674"
---
# <a name="getsharingmetadataresponsemessage"></a><span data-ttu-id="0a623-103">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a623-103">GetSharingMetadataResponseMessage</span></span>

<span data-ttu-id="0a623-104">L’élément **GetSharingMetadataResponseMessage** contient l’état et les résultats d’une seule demande [d’opération GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0a623-104">The **GetSharingMetadataResponseMessage** element contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponseMessage>
```

 <span data-ttu-id="0a623-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0a623-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a623-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0a623-106">Attributes and elements</span></span>

<span data-ttu-id="0a623-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0a623-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a623-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0a623-108">Attributes</span></span>

|<span data-ttu-id="0a623-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0a623-109">**Attribute**</span></span>|<span data-ttu-id="0a623-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a623-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a623-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0a623-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0a623-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0a623-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0a623-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="0a623-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0a623-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="0a623-114">-  Success</span></span>  <br/><span data-ttu-id="0a623-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="0a623-115">-  Warning</span></span>  <br/><span data-ttu-id="0a623-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="0a623-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0a623-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0a623-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="0a623-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0a623-118">**Value**</span></span>|<span data-ttu-id="0a623-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a623-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a623-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="0a623-120">**Success**</span></span> <br/> |<span data-ttu-id="0a623-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="0a623-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0a623-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="0a623-122">**Warning**</span></span> <br/> | <span data-ttu-id="0a623-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="0a623-123">Describes a request that was not processed.</span></span> <span data-ttu-id="0a623-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="0a623-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0a623-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="0a623-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0a623-126">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="0a623-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0a623-127">-Le service d’annuaire Active Directory est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a623-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="0a623-128">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="0a623-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0a623-129">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a623-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0a623-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="0a623-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="0a623-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="0a623-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0a623-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="0a623-132">**Error**</span></span> <br/> | <span data-ttu-id="0a623-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="0a623-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0a623-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="0a623-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0a623-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="0a623-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0a623-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="0a623-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="0a623-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="0a623-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="0a623-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="0a623-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="0a623-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="0a623-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0a623-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="0a623-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="0a623-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0a623-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0a623-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0a623-142">Child elements</span></span>

|<span data-ttu-id="0a623-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a623-143">**Element**</span></span>|<span data-ttu-id="0a623-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a623-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a623-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="0a623-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0a623-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0a623-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0a623-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0a623-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0a623-148">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="0a623-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0a623-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0a623-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0a623-150">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="0a623-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="0a623-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="0a623-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0a623-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0a623-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0a623-153">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="0a623-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0a623-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="0a623-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="0a623-155">Contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="0a623-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="0a623-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="0a623-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="0a623-157">Représente les destinataires du dossier de demande de partage qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="0a623-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a623-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0a623-158">Parent elements</span></span>

|<span data-ttu-id="0a623-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a623-159">**Element**</span></span>|<span data-ttu-id="0a623-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a623-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a623-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a623-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0a623-162">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a623-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a623-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="0a623-163">Remarks</span></span>

<span data-ttu-id="0a623-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="0a623-164">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a623-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0a623-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a623-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0a623-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a623-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0a623-167">Schema Name</span></span>  <br/> |<span data-ttu-id="0a623-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0a623-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a623-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0a623-169">Validation File</span></span>  <br/> |<span data-ttu-id="0a623-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0a623-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a623-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0a623-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a623-172">False</span><span class="sxs-lookup"><span data-stu-id="0a623-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a623-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0a623-173">See also</span></span>

- [<span data-ttu-id="0a623-174">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="0a623-174">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="0a623-175">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0a623-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

