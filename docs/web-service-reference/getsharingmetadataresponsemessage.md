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
description: L’élément GetSharingMetadataResponseMessage contient l’État et le résultat d’une seule demande d’opération GetSharingMetadata.
ms.openlocfilehash: cca06cb12ce48ba182c4ebfe475b2acfcc861d63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457339"
---
# <a name="getsharingmetadataresponsemessage"></a><span data-ttu-id="f0f7f-103">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f0f7f-103">GetSharingMetadataResponseMessage</span></span>

<span data-ttu-id="f0f7f-104">L’élément **GetSharingMetadataResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0f7f-104">The **GetSharingMetadataResponseMessage** element contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponseMessage>
```

 <span data-ttu-id="f0f7f-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0f7f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f0f7f-106">Attributes and elements</span></span>

<span data-ttu-id="f0f7f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0f7f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f0f7f-108">Attributes</span></span>

|<span data-ttu-id="f0f7f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-109">**Attribute**</span></span>|<span data-ttu-id="f0f7f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0f7f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f0f7f-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f0f7f-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="f0f7f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f0f7f-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="f0f7f-114">-  Success</span></span>  <br/><span data-ttu-id="f0f7f-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="f0f7f-115">-  Warning</span></span>  <br/><span data-ttu-id="f0f7f-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="f0f7f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f0f7f-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f0f7f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f0f7f-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-118">**Value**</span></span>|<span data-ttu-id="f0f7f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0f7f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-120">**Success**</span></span> <br/> |<span data-ttu-id="f0f7f-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f0f7f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-122">**Warning**</span></span> <br/> | <span data-ttu-id="f0f7f-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f0f7f-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f0f7f-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="f0f7f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f0f7f-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f0f7f-127">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="f0f7f-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f0f7f-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f0f7f-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f0f7f-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f0f7f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-132">**Error**</span></span> <br/> | <span data-ttu-id="f0f7f-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f0f7f-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="f0f7f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f0f7f-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="f0f7f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f0f7f-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="f0f7f-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f0f7f-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="f0f7f-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="f0f7f-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="f0f7f-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f0f7f-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="f0f7f-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f0f7f-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="f0f7f-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f0f7f-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f0f7f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0f7f-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f0f7f-142">Child elements</span></span>

|<span data-ttu-id="f0f7f-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-143">**Element**</span></span>|<span data-ttu-id="f0f7f-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f7f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f0f7f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f0f7f-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f0f7f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f0f7f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f0f7f-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f0f7f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f0f7f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f0f7f-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f0f7f-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f0f7f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f0f7f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f0f7f-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f0f7f-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="f0f7f-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="f0f7f-155">Contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="f0f7f-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="f0f7f-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="f0f7f-157">Représente les destinataires de la demande de partage de dossier qui ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0f7f-158">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f0f7f-158">Parent elements</span></span>

|<span data-ttu-id="f0f7f-159">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-159">**Element**</span></span>|<span data-ttu-id="f0f7f-160">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0f7f-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0f7f-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f0f7f-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f0f7f-162">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0f7f-163">Remarques</span><span class="sxs-lookup"><span data-stu-id="f0f7f-163">Remarks</span></span>

<span data-ttu-id="f0f7f-164">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f0f7f-164">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0f7f-165">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f0f7f-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0f7f-166">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f0f7f-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0f7f-167">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f0f7f-167">Schema Name</span></span>  <br/> |<span data-ttu-id="f0f7f-168">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f0f7f-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0f7f-169">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f0f7f-169">Validation File</span></span>  <br/> |<span data-ttu-id="f0f7f-170">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f0f7f-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0f7f-171">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f0f7f-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0f7f-172">False</span><span class="sxs-lookup"><span data-stu-id="f0f7f-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0f7f-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f0f7f-173">See also</span></span>

- [<span data-ttu-id="f0f7f-174">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f0f7f-174">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="f0f7f-175">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f0f7f-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

