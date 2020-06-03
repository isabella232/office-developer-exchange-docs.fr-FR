---
title: CopyItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: L’élément CopyItemResponseMessage contient l’État et le résultat d’une seule demande d’opération CopyItem.
ms.openlocfilehash: 99449a4c05d0b2ea13dfca4235aa5f40d54d1214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466443"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="e16f2-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e16f2-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="e16f2-104">L’élément **CopyItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e16f2-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="e16f2-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e16f2-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e16f2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e16f2-106">Attributes and elements</span></span>

<span data-ttu-id="e16f2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e16f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e16f2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e16f2-108">Attributes</span></span>

|<span data-ttu-id="e16f2-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e16f2-109">**Attribute**</span></span>|<span data-ttu-id="e16f2-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e16f2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e16f2-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e16f2-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e16f2-112">Décrit l’état d’une réponse de l' [opération CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e16f2-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="e16f2-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="e16f2-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="e16f2-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="e16f2-114">- Success</span></span>  <br/><span data-ttu-id="e16f2-115">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="e16f2-115">-  Warning</span></span>  <br/><span data-ttu-id="e16f2-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="e16f2-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e16f2-117">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e16f2-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="e16f2-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e16f2-118">**Value**</span></span>|<span data-ttu-id="e16f2-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e16f2-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e16f2-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="e16f2-120">**Success**</span></span> <br/> |<span data-ttu-id="e16f2-121">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="e16f2-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e16f2-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e16f2-122">**Warning**</span></span> <br/> | <span data-ttu-id="e16f2-123">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="e16f2-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e16f2-124">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="e16f2-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="e16f2-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="e16f2-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="e16f2-126">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="e16f2-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="e16f2-127">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="e16f2-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="e16f2-128">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="e16f2-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="e16f2-129">-La base de données de boîtes aux lettres (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="e16f2-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="e16f2-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="e16f2-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e16f2-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="e16f2-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="e16f2-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="e16f2-132">**Error**</span></span> <br/> | <span data-ttu-id="e16f2-133">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="e16f2-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="e16f2-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="e16f2-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e16f2-135">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="e16f2-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e16f2-136">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="e16f2-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e16f2-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="e16f2-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e16f2-138">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="e16f2-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e16f2-139">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="e16f2-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e16f2-140">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="e16f2-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="e16f2-141">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="e16f2-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e16f2-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e16f2-142">Child elements</span></span>

|<span data-ttu-id="e16f2-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e16f2-143">**Element**</span></span>|<span data-ttu-id="e16f2-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="e16f2-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e16f2-145">- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="e16f2-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="e16f2-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="e16f2-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e16f2-147">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e16f2-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e16f2-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e16f2-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e16f2-149">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="e16f2-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e16f2-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e16f2-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e16f2-151">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="e16f2-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e16f2-152">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="e16f2-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e16f2-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e16f2-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e16f2-154">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="e16f2-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e16f2-155">Items</span><span class="sxs-lookup"><span data-stu-id="e16f2-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="e16f2-156">Contient un tableau d’éléments copiés</span><span class="sxs-lookup"><span data-stu-id="e16f2-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e16f2-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e16f2-157">Parent elements</span></span>

|<span data-ttu-id="e16f2-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e16f2-158">**Element**</span></span>|<span data-ttu-id="e16f2-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="e16f2-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e16f2-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e16f2-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e16f2-161">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e16f2-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e16f2-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="e16f2-162">Remarks</span></span>

<span data-ttu-id="e16f2-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e16f2-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e16f2-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e16f2-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e16f2-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e16f2-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e16f2-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e16f2-166">Schema name</span></span>  <br/> |<span data-ttu-id="e16f2-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e16f2-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e16f2-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e16f2-168">Validation file</span></span>  <br/> |<span data-ttu-id="e16f2-169">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e16f2-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e16f2-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e16f2-170">Can be empty</span></span>  <br/> |<span data-ttu-id="e16f2-171">False</span><span class="sxs-lookup"><span data-stu-id="e16f2-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e16f2-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e16f2-172">See also</span></span>

- [<span data-ttu-id="e16f2-173">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="e16f2-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="e16f2-174">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e16f2-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

