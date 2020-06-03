---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: L’élément FindItemResponseMessage contient l’État et le résultat d’une seule demande d’opération FindItem.
ms.openlocfilehash: ca941e0c7e5b9b08f6f495ccae0d634d72b8f429
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462534"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="4b3d5-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b3d5-103">FindItemResponseMessage</span></span>

<span data-ttu-id="4b3d5-104">L’élément **FindItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3d5-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4b3d5-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="4b3d5-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="4b3d5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4b3d5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4b3d5-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b3d5-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="4b3d5-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b3d5-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b3d5-109">Attributes and elements</span></span>

<span data-ttu-id="4b3d5-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b3d5-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b3d5-111">Attributes</span></span>

|<span data-ttu-id="4b3d5-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-112">**Attribute**</span></span>|<span data-ttu-id="4b3d5-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b3d5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4b3d5-115">Décrit l’état d’une réponse d' [opération FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3d5-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="4b3d5-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="4b3d5-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="4b3d5-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="4b3d5-117">-  Success</span></span>  <br/><span data-ttu-id="4b3d5-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="4b3d5-118">-  Warning</span></span>  <br/><span data-ttu-id="4b3d5-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="4b3d5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4b3d5-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4b3d5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4b3d5-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-121">**Value**</span></span>|<span data-ttu-id="4b3d5-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4b3d5-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-123">**Success**</span></span> <br/> |<span data-ttu-id="4b3d5-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4b3d5-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-125">**Warning**</span></span> <br/> | <span data-ttu-id="4b3d5-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4b3d5-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4b3d5-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="4b3d5-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="4b3d5-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="4b3d5-130">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="4b3d5-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4b3d5-132">-La base de données de messages (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="4b3d5-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="4b3d5-134">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="4b3d5-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-135">**Error**</span></span> <br/> | <span data-ttu-id="4b3d5-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4b3d5-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="4b3d5-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4b3d5-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="4b3d5-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4b3d5-139">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="4b3d5-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="4b3d5-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="4b3d5-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="4b3d5-141">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="4b3d5-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4b3d5-142">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="4b3d5-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4b3d5-143">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="4b3d5-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4b3d5-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3d5-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4b3d5-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b3d5-145">Child elements</span></span>

|<span data-ttu-id="4b3d5-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-146">**Element**</span></span>|<span data-ttu-id="4b3d5-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b3d5-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4b3d5-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4b3d5-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4b3d5-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4b3d5-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4b3d5-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4b3d5-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4b3d5-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4b3d5-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4b3d5-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4b3d5-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4b3d5-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4b3d5-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4b3d5-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="4b3d5-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="4b3d5-158">Contient les résultats d’une recherche d’un dossier racine unique pendant une [opération FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4b3d5-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b3d5-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b3d5-159">Parent elements</span></span>

|<span data-ttu-id="4b3d5-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-160">**Element**</span></span>|<span data-ttu-id="4b3d5-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b3d5-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b3d5-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4b3d5-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4b3d5-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b3d5-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b3d5-164">Remarks</span></span>

<span data-ttu-id="4b3d5-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b3d5-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b3d5-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b3d5-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b3d5-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b3d5-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b3d5-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b3d5-168">Schema name</span></span>  <br/> |<span data-ttu-id="4b3d5-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4b3d5-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b3d5-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b3d5-170">Validation file</span></span>  <br/> |<span data-ttu-id="4b3d5-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b3d5-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b3d5-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b3d5-172">Can be empty</span></span>  <br/> |<span data-ttu-id="4b3d5-173">False</span><span class="sxs-lookup"><span data-stu-id="4b3d5-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b3d5-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b3d5-174">See also</span></span>

- [<span data-ttu-id="4b3d5-175">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="4b3d5-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="4b3d5-176">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="4b3d5-176">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

