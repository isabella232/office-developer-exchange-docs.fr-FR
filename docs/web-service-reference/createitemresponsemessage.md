---
title: CreateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponseMessage
api_type:
- schema
ms.assetid: 595d36c2-f87a-4d50-8e8b-f58d7641564b
description: L’élément CreateItemResponseMessage contient l’État et le résultat d’une seule demande d’opération CreateItem.
ms.openlocfilehash: 6304d2c7a3c9253c03c07eb37e9a57226e794a24
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457850"
---
# <a name="createitemresponsemessage"></a><span data-ttu-id="0a665-103">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a665-103">CreateItemResponseMessage</span></span>

<span data-ttu-id="0a665-104">L’élément **CreateItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0a665-104">The **CreateItemResponseMessage** element contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0a665-105">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="0a665-105">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="0a665-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a665-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="0a665-107">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a665-107">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
  
```xml
<CreateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CreateItemResponseMessage>
```

 <span data-ttu-id="0a665-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0a665-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a665-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0a665-109">Attributes and elements</span></span>

<span data-ttu-id="0a665-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0a665-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a665-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="0a665-111">Attributes</span></span>

|<span data-ttu-id="0a665-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0a665-112">**Attribute**</span></span>|<span data-ttu-id="0a665-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a665-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a665-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0a665-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0a665-115">Décrit l’état d’une réponse à une [opération CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0a665-115">Describes the status of a [CreateItem operation](createitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="0a665-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="0a665-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="0a665-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="0a665-117">-  Success</span></span>  <br/><span data-ttu-id="0a665-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="0a665-118">-  Warning</span></span>  <br/><span data-ttu-id="0a665-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="0a665-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0a665-120">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0a665-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0a665-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0a665-121">**Value**</span></span>|<span data-ttu-id="0a665-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a665-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a665-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="0a665-123">**Success**</span></span> <br/> |<span data-ttu-id="0a665-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0a665-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0a665-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0a665-125">**Warning**</span></span> <br/> | <span data-ttu-id="0a665-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="0a665-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0a665-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="0a665-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="0a665-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="0a665-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="0a665-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="0a665-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0a665-130">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a665-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0a665-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="0a665-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0a665-132">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="0a665-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0a665-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="0a665-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0a665-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="0a665-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="0a665-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="0a665-135">**Error**</span></span> <br/> | <span data-ttu-id="0a665-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="0a665-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="0a665-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="0a665-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0a665-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="0a665-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0a665-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="0a665-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="0a665-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="0a665-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="0a665-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="0a665-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="0a665-142">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="0a665-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0a665-143">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="0a665-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="0a665-144">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0a665-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0a665-145">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0a665-145">Child elements</span></span>

|<span data-ttu-id="0a665-146">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a665-146">**Element**</span></span>|<span data-ttu-id="0a665-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a665-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a665-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0a665-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0a665-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0a665-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0a665-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0a665-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0a665-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="0a665-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0a665-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0a665-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0a665-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="0a665-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0a665-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="0a665-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0a665-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0a665-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0a665-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="0a665-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0a665-157">Items</span><span class="sxs-lookup"><span data-stu-id="0a665-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="0a665-158">Contient un tableau d’éléments créés.</span><span class="sxs-lookup"><span data-stu-id="0a665-158">Contains an array of created items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a665-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0a665-159">Parent elements</span></span>

|<span data-ttu-id="0a665-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a665-160">**Element**</span></span>|<span data-ttu-id="0a665-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a665-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a665-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a665-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0a665-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a665-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a665-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="0a665-164">Remarks</span></span>

<span data-ttu-id="0a665-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0a665-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a665-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0a665-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a665-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0a665-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a665-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0a665-168">Schema Name</span></span>  <br/> |<span data-ttu-id="0a665-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0a665-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a665-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0a665-170">Validation File</span></span>  <br/> |<span data-ttu-id="0a665-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0a665-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a665-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0a665-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a665-173">False</span><span class="sxs-lookup"><span data-stu-id="0a665-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a665-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0a665-174">See also</span></span>

- [<span data-ttu-id="0a665-175">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="0a665-175">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="0a665-176">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0a665-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="0a665-177">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0a665-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

