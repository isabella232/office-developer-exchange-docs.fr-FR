---
title: RefreshSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponseMessage
api_type:
- schema
ms.assetid: 53ee65bd-cf75-4e04-9b27-eff1b040ae82
description: L’élément RefreshSharingFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération RefreshSharingFolder.
ms.openlocfilehash: f2cc357298d523b418d2c45598639627c5a63252
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468669"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="e1a92-103">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1a92-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="e1a92-104">L’élément **RefreshSharingFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération RefreshSharingFolder](refreshsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e1a92-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="e1a92-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e1a92-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1a92-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e1a92-106">Attributes and elements</span></span>

<span data-ttu-id="e1a92-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e1a92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1a92-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e1a92-108">Attributes</span></span>

|<span data-ttu-id="e1a92-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e1a92-109">**Attribute**</span></span>|<span data-ttu-id="e1a92-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1a92-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1a92-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e1a92-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e1a92-112">Décrit l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e1a92-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="e1a92-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="e1a92-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e1a92-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="e1a92-114">-  Success</span></span>  <br/><span data-ttu-id="e1a92-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="e1a92-115">-  Warning</span></span>  <br/><span data-ttu-id="e1a92-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="e1a92-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e1a92-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e1a92-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="e1a92-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e1a92-118">**Value**</span></span>|<span data-ttu-id="e1a92-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1a92-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1a92-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="e1a92-120">**Success**</span></span> <br/> |<span data-ttu-id="e1a92-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="e1a92-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e1a92-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e1a92-122">**Warning**</span></span> <br/> | <span data-ttu-id="e1a92-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="e1a92-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e1a92-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="e1a92-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e1a92-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="e1a92-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="e1a92-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="e1a92-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e1a92-127">-Le service d’annuaire Active Directory est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="e1a92-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="e1a92-128">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="e1a92-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e1a92-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="e1a92-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e1a92-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="e1a92-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e1a92-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="e1a92-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="e1a92-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="e1a92-132">**Error**</span></span> <br/> | <span data-ttu-id="e1a92-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="e1a92-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e1a92-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="e1a92-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e1a92-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="e1a92-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e1a92-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="e1a92-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e1a92-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="e1a92-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e1a92-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="e1a92-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e1a92-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="e1a92-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e1a92-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="e1a92-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="e1a92-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e1a92-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e1a92-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e1a92-142">Child elements</span></span>

|<span data-ttu-id="e1a92-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1a92-143">**Element**</span></span>|<span data-ttu-id="e1a92-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1a92-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1a92-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="e1a92-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e1a92-146">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e1a92-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e1a92-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1a92-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e1a92-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="e1a92-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e1a92-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e1a92-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e1a92-150">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="e1a92-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="e1a92-151">Cet élément contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="e1a92-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e1a92-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e1a92-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e1a92-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="e1a92-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1a92-154">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e1a92-154">Parent elements</span></span>

|<span data-ttu-id="e1a92-155">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1a92-155">**Element**</span></span>|<span data-ttu-id="e1a92-156">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1a92-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1a92-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e1a92-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e1a92-158">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1a92-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1a92-159">Remarques</span><span class="sxs-lookup"><span data-stu-id="e1a92-159">Remarks</span></span>

<span data-ttu-id="e1a92-160">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e1a92-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1a92-161">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e1a92-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1a92-162">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e1a92-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1a92-163">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e1a92-163">Schema Name</span></span>  <br/> |<span data-ttu-id="e1a92-164">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e1a92-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e1a92-165">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e1a92-165">Validation File</span></span>  <br/> |<span data-ttu-id="e1a92-166">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e1a92-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1a92-167">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e1a92-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1a92-168">False</span><span class="sxs-lookup"><span data-stu-id="e1a92-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1a92-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1a92-169">See also</span></span>

- [<span data-ttu-id="e1a92-170">Opération RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1a92-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="e1a92-171">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1a92-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

