---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: L’élément DeleteItemResponseMessage contient l’État et le résultat d’une seule demande d’opération DeleteItem.
ms.openlocfilehash: 78e3efc6a9e9e6629d7efe7f2dc294e0a731005a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526927"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="9f8f9-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f8f9-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="9f8f9-104">L’élément **DeleteItemResponseMessage** contient l’État et le résultat d’une seule demande d' [opération DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f8f9-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="9f8f9-105">Updateitemresponse</span><span class="sxs-lookup"><span data-stu-id="9f8f9-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="9f8f9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f8f9-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="9f8f9-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f8f9-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="9f8f9-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f8f9-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f8f9-109">Attributes and elements</span></span>

<span data-ttu-id="9f8f9-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f8f9-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f8f9-111">Attributes</span></span>

|<span data-ttu-id="9f8f9-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-112">**Attribute**</span></span>|<span data-ttu-id="9f8f9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f8f9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9f8f9-115">Décrit l’état d’une réponse d' [opération DeleteItem](deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f8f9-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="9f8f9-116">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="9f8f9-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="9f8f9-117">-Réussite</span><span class="sxs-lookup"><span data-stu-id="9f8f9-117">- Success</span></span>  <br/><span data-ttu-id="9f8f9-118">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="9f8f9-118">-  Warning</span></span>  <br/><span data-ttu-id="9f8f9-119">-Erreur</span><span class="sxs-lookup"><span data-stu-id="9f8f9-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="9f8f9-120">Attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9f8f9-120">ResponseClass attribute</span></span>

|<span data-ttu-id="9f8f9-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-121">**Value**</span></span>|<span data-ttu-id="9f8f9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f8f9-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-123">**Success**</span></span> <br/> |<span data-ttu-id="9f8f9-124">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9f8f9-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-125">**Warning**</span></span> <br/> | <span data-ttu-id="9f8f9-126">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="9f8f9-127">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="9f8f9-128">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="9f8f9-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="9f8f9-129">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="9f8f9-130">-Les services de domaine Active Directory (AD DS) sont en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="9f8f9-131">-Les boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="9f8f9-132">-La base de données de messages (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="9f8f9-133">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="9f8f9-134">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="9f8f9-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-135">**Error**</span></span> <br/> | <span data-ttu-id="9f8f9-136">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="9f8f9-137">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="9f8f9-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="9f8f9-138">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="9f8f9-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9f8f9-139">-Les attributs ou les éléments sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="9f8f9-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="9f8f9-140">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="9f8f9-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="9f8f9-141">-Attribut ou élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="9f8f9-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="9f8f9-142">-Une tentative client de définition du niveau de journalisation des erreurs au-dessus du niveau maximal autorisé par l’administrateur</span><span class="sxs-lookup"><span data-stu-id="9f8f9-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="9f8f9-143">-Une tentative client de définir le niveau d’échec de gravité sous le niveau par défaut spécifié par l’administrateur ;</span><span class="sxs-lookup"><span data-stu-id="9f8f9-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="9f8f9-144">-Tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="9f8f9-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9f8f9-145">-Échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="9f8f9-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="9f8f9-146">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9f8f9-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f8f9-147">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f8f9-147">Child elements</span></span>

|<span data-ttu-id="9f8f9-148">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-148">**Element**</span></span>|<span data-ttu-id="9f8f9-149">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f8f9-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="9f8f9-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9f8f9-151">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9f8f9-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9f8f9-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9f8f9-153">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9f8f9-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9f8f9-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9f8f9-155">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9f8f9-156">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9f8f9-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9f8f9-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9f8f9-158">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f8f9-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f8f9-159">Parent elements</span></span>

|<span data-ttu-id="9f8f9-160">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-160">**Element**</span></span>|<span data-ttu-id="9f8f9-161">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f8f9-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f8f9-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f8f9-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f8f9-163">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f8f9-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f8f9-164">Remarks</span></span>

<span data-ttu-id="9f8f9-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="9f8f9-166">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="9f8f9-166">Version differences</span></span>

<span data-ttu-id="9f8f9-167">Dans les versions d’Exchange commençant par Build 15.00.0986.00, l’élément **DeleteItemResponseMessage** est de type **DeleteItemResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="9f8f9-168">Dans les versions antérieures, l’élément est de type **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="9f8f9-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f8f9-169">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f8f9-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f8f9-170">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f8f9-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f8f9-171">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f8f9-171">Schema Name</span></span>  <br/> |<span data-ttu-id="9f8f9-172">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9f8f9-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f8f9-173">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f8f9-173">Validation File</span></span>  <br/> |<span data-ttu-id="9f8f9-174">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9f8f9-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f8f9-175">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f8f9-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f8f9-176">False</span><span class="sxs-lookup"><span data-stu-id="9f8f9-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f8f9-177">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f8f9-177">See also</span></span>

- [<span data-ttu-id="9f8f9-178">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="9f8f9-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="9f8f9-179">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="9f8f9-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="9f8f9-180">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f8f9-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9f8f9-181">Suppression d’éléments (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="9f8f9-181">Deleting Items (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

