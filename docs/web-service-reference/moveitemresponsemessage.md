---
title: MoveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: L’élément MoveItemResponseMessage contient l’État et le résultat d’une seule demande d’opération MoveItem.
ms.openlocfilehash: fd96c34840acd5b6137a2a5d50980dc86202629f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530393"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="898de-103">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="898de-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="898de-104">L’élément **MoveItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="898de-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="898de-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="898de-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="898de-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="898de-106">Attributes and elements</span></span>

<span data-ttu-id="898de-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="898de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="898de-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="898de-108">Attributes</span></span>

|<span data-ttu-id="898de-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="898de-109">**Attribute**</span></span>|<span data-ttu-id="898de-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="898de-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="898de-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="898de-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="898de-112">Décrit l’état d’une réponse d' [opération MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="898de-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="898de-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="898de-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="898de-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="898de-114">-  Success</span></span>  <br/><span data-ttu-id="898de-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="898de-115">-  Warning</span></span>  <br/><span data-ttu-id="898de-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="898de-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="898de-117">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="898de-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="898de-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="898de-118">**Value**</span></span>|<span data-ttu-id="898de-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="898de-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="898de-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="898de-120">**Success**</span></span> <br/> |<span data-ttu-id="898de-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="898de-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="898de-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="898de-122">**Warning**</span></span> <br/> | <span data-ttu-id="898de-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="898de-123">Describes a request that was not processed.</span></span> <span data-ttu-id="898de-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="898de-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="898de-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="898de-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="898de-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="898de-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="898de-127">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="898de-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="898de-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="898de-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="898de-129">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="898de-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="898de-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="898de-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="898de-131">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="898de-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="898de-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="898de-132">**Error**</span></span> <br/> | <span data-ttu-id="898de-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="898de-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="898de-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="898de-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="898de-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="898de-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="898de-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="898de-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="898de-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="898de-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="898de-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="898de-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="898de-139">-Tout accès non autorisé tenté par un client</span><span class="sxs-lookup"><span data-stu-id="898de-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="898de-140">-Tout échec côté serveur en réponse à un appel côté client valide.</span><span class="sxs-lookup"><span data-stu-id="898de-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="898de-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="898de-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="898de-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="898de-142">Child elements</span></span>

|<span data-ttu-id="898de-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="898de-143">**Element**</span></span>|<span data-ttu-id="898de-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="898de-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="898de-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="898de-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="898de-146">Texte décrivant l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="898de-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="898de-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="898de-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="898de-148">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="898de-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="898de-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="898de-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="898de-150">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="898de-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="898de-151">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="898de-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="898de-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="898de-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="898de-153">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="898de-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="898de-154">Items</span><span class="sxs-lookup"><span data-stu-id="898de-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="898de-155">Contient un tableau d’éléments déplacés.</span><span class="sxs-lookup"><span data-stu-id="898de-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="898de-156">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="898de-156">Parent elements</span></span>

|<span data-ttu-id="898de-157">**Élément**</span><span class="sxs-lookup"><span data-stu-id="898de-157">**Element**</span></span>|<span data-ttu-id="898de-158">**Description**</span><span class="sxs-lookup"><span data-stu-id="898de-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="898de-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="898de-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="898de-160">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="898de-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="898de-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="898de-161">Remarks</span></span>

<span data-ttu-id="898de-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="898de-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="898de-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="898de-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="898de-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="898de-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="898de-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="898de-165">Schema Name</span></span>  <br/> |<span data-ttu-id="898de-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="898de-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="898de-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="898de-167">Validation File</span></span>  <br/> |<span data-ttu-id="898de-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="898de-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="898de-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="898de-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="898de-170">False</span><span class="sxs-lookup"><span data-stu-id="898de-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="898de-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="898de-171">See also</span></span>

- [<span data-ttu-id="898de-172">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="898de-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="898de-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="898de-173">MoveItem</span></span>](moveitem.md)

