---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: L’élément GetItemResponseMessage contient l’État et le résultat d’une seule demande d’opération GetItem.
ms.openlocfilehash: bd25a82641259e1546bad6eef5c2f6f8f03e98cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458669"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="216eb-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="216eb-103">GetItemResponseMessage</span></span>

<span data-ttu-id="216eb-104">L’élément **GetItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="216eb-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="216eb-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="216eb-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="216eb-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="216eb-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="216eb-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="216eb-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="216eb-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="216eb-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="216eb-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="216eb-109">Attributes and elements</span></span>

<span data-ttu-id="216eb-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="216eb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="216eb-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="216eb-111">Attributes</span></span>

|<span data-ttu-id="216eb-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="216eb-112">**Attribute**</span></span>|<span data-ttu-id="216eb-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="216eb-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="216eb-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="216eb-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="216eb-115">Décrit l’état d’une réponse de l' [opération GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="216eb-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="216eb-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="216eb-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="216eb-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="216eb-117">- Success</span></span><br/><span data-ttu-id="216eb-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="216eb-118">- Warning</span></span><br/><span data-ttu-id="216eb-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="216eb-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="216eb-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="216eb-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="216eb-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="216eb-121">**Value**</span></span>|<span data-ttu-id="216eb-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="216eb-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="216eb-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="216eb-123">**Success**</span></span> <br/> |<span data-ttu-id="216eb-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="216eb-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="216eb-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="216eb-125">**Warning**</span></span> <br/> | <span data-ttu-id="216eb-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="216eb-126">Describes a request that was not processed.</span></span> <span data-ttu-id="216eb-127">Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande a été traité et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="216eb-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="216eb-128">Voici des exemples de sources pour les avertissements :</span><span class="sxs-lookup"><span data-stu-id="216eb-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="216eb-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="216eb-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="216eb-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="216eb-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="216eb-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="216eb-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="216eb-132">-MDB est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="216eb-132">- MDB is offline.</span></span><br/><span data-ttu-id="216eb-133">-Le mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="216eb-133">- Password is expired.</span></span>  <br/><span data-ttu-id="216eb-134">-Quota dépassé.</span><span class="sxs-lookup"><span data-stu-id="216eb-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="216eb-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="216eb-135">**Error**</span></span> <br/> | <span data-ttu-id="216eb-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="216eb-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="216eb-137">Voici des exemples de sources pour les erreurs :</span><span class="sxs-lookup"><span data-stu-id="216eb-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="216eb-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="216eb-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="216eb-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="216eb-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="216eb-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="216eb-140">- Unknown tag</span></span><br/><span data-ttu-id="216eb-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="216eb-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="216eb-142">-Accès non autorisé tenté par un client</span><span class="sxs-lookup"><span data-stu-id="216eb-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="216eb-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="216eb-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="216eb-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="216eb-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="216eb-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="216eb-145">Child elements</span></span>

|<span data-ttu-id="216eb-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="216eb-146">**Element**</span></span>|<span data-ttu-id="216eb-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="216eb-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="216eb-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="216eb-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="216eb-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="216eb-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="216eb-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="216eb-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="216eb-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="216eb-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="216eb-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="216eb-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="216eb-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="216eb-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="216eb-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="216eb-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="216eb-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="216eb-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="216eb-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="216eb-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="216eb-157">Items</span><span class="sxs-lookup"><span data-stu-id="216eb-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="216eb-158">Contient un tableau des éléments retournés.</span><span class="sxs-lookup"><span data-stu-id="216eb-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="216eb-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="216eb-159">Parent elements</span></span>

|<span data-ttu-id="216eb-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="216eb-160">**Element**</span></span>|<span data-ttu-id="216eb-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="216eb-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="216eb-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="216eb-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="216eb-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="216eb-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="216eb-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="216eb-164">Remarks</span></span>

<span data-ttu-id="216eb-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="216eb-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="216eb-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="216eb-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="216eb-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="216eb-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="216eb-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="216eb-168">Schema Name</span></span>  <br/> |<span data-ttu-id="216eb-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="216eb-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="216eb-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="216eb-170">Validation File</span></span>  <br/> |<span data-ttu-id="216eb-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="216eb-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="216eb-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="216eb-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="216eb-173">False</span><span class="sxs-lookup"><span data-stu-id="216eb-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="216eb-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="216eb-174">See also</span></span>

- [<span data-ttu-id="216eb-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="216eb-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="216eb-176">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="216eb-176">GetItem operation</span></span>](getitem-operation.md)

