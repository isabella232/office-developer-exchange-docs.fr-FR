---
title: FindConversationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversationResponse
api_type:
- schema
ms.assetid: a689e29d-5f3d-4deb-81ee-8b6cc60f6dea
description: L’élément FindConversationResponse définit une réponse à une demande d’opération FindConversation.
ms.openlocfilehash: 68acc42045b91ab4b574f32ba3fd622057863015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462639"
---
# <a name="findconversationresponse"></a><span data-ttu-id="65cb5-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="65cb5-103">FindConversationResponse</span></span>

<span data-ttu-id="65cb5-104">L’élément **FindConversationResponse** définit une réponse à une demande d' [opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65cb5-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="65cb5-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="65cb5-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="65cb5-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="65cb5-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65cb5-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65cb5-107">Attributes and elements</span></span>

<span data-ttu-id="65cb5-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65cb5-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65cb5-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="65cb5-109">Attributes</span></span>

|<span data-ttu-id="65cb5-110">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="65cb5-110">**Attribute**</span></span>|<span data-ttu-id="65cb5-111">**Description**</span><span class="sxs-lookup"><span data-stu-id="65cb5-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65cb5-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="65cb5-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="65cb5-113">Décrit l’état d’une réponse d' [opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65cb5-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="65cb5-114">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="65cb5-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="65cb5-115">-Réussite</span><span class="sxs-lookup"><span data-stu-id="65cb5-115">-  Success</span></span>  <br/><span data-ttu-id="65cb5-116">-AVERTISSEMENT</span><span class="sxs-lookup"><span data-stu-id="65cb5-116">-  Warning</span></span>  <br/><span data-ttu-id="65cb5-117">-Erreur</span><span class="sxs-lookup"><span data-stu-id="65cb5-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="65cb5-118">Valeurs d’attribut ResponseClass</span><span class="sxs-lookup"><span data-stu-id="65cb5-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="65cb5-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="65cb5-119">**Value**</span></span>|<span data-ttu-id="65cb5-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="65cb5-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65cb5-121">**Success**</span><span class="sxs-lookup"><span data-stu-id="65cb5-121">**Success**</span></span> <br/> |<span data-ttu-id="65cb5-122">Décrit une demande qui est satisfaite.</span><span class="sxs-lookup"><span data-stu-id="65cb5-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="65cb5-123">**Warning**</span><span class="sxs-lookup"><span data-stu-id="65cb5-123">**Warning**</span></span> <br/> | <span data-ttu-id="65cb5-124">Décrit une demande qui n’a pas été traitée.</span><span class="sxs-lookup"><span data-stu-id="65cb5-124">Describes a request that was not processed.</span></span> <span data-ttu-id="65cb5-125">Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.</span><span class="sxs-lookup"><span data-stu-id="65cb5-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="65cb5-126">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="65cb5-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="65cb5-127">-La banque Exchange est hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="65cb5-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="65cb5-128">-Les services de domaine Active Directory (AD DS) sont hors connexion.</span><span class="sxs-lookup"><span data-stu-id="65cb5-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="65cb5-129">-Les boîtes aux lettres ont été déplacées.</span><span class="sxs-lookup"><span data-stu-id="65cb5-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="65cb5-130">-La base de données de messages (MDB) est hors connexion.</span><span class="sxs-lookup"><span data-stu-id="65cb5-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="65cb5-131">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="65cb5-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="65cb5-132">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="65cb5-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="65cb5-133">**Error**</span><span class="sxs-lookup"><span data-stu-id="65cb5-133">**Error**</span></span> <br/> | <span data-ttu-id="65cb5-134">Décrit une demande qui ne peut pas être satisfaite.</span><span class="sxs-lookup"><span data-stu-id="65cb5-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="65cb5-135">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="65cb5-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="65cb5-136">-Attributs ou éléments non valides</span><span class="sxs-lookup"><span data-stu-id="65cb5-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="65cb5-137">-Les attributs ou les éléments qui sont en dehors de la plage</span><span class="sxs-lookup"><span data-stu-id="65cb5-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="65cb5-138">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="65cb5-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="65cb5-139">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="65cb5-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="65cb5-140">-Une tentative d’accès non autorisée par un client</span><span class="sxs-lookup"><span data-stu-id="65cb5-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="65cb5-141">-Un échec côté serveur en réponse à un appel côté client valide</span><span class="sxs-lookup"><span data-stu-id="65cb5-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="65cb5-142">Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="65cb5-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="65cb5-143">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65cb5-143">Child elements</span></span>

|<span data-ttu-id="65cb5-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65cb5-144">**Element**</span></span>|<span data-ttu-id="65cb5-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="65cb5-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65cb5-146">Conversations</span><span class="sxs-lookup"><span data-stu-id="65cb5-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="65cb5-147">Contient un tableau de conversations.</span><span class="sxs-lookup"><span data-stu-id="65cb5-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="65cb5-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="65cb5-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="65cb5-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="65cb5-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="65cb5-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="65cb5-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="65cb5-151">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="65cb5-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="65cb5-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="65cb5-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="65cb5-153">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="65cb5-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="65cb5-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="65cb5-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="65cb5-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="65cb5-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="65cb5-156">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="65cb5-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65cb5-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65cb5-157">Parent elements</span></span>

<span data-ttu-id="65cb5-158">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65cb5-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="65cb5-159">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="65cb5-159">Text value</span></span>

<span data-ttu-id="65cb5-160">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65cb5-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65cb5-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="65cb5-161">Remarks</span></span>

<span data-ttu-id="65cb5-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="65cb5-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65cb5-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65cb5-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65cb5-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65cb5-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65cb5-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65cb5-165">Schema name</span></span>  <br/> |<span data-ttu-id="65cb5-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="65cb5-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="65cb5-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65cb5-167">Validation file</span></span>  <br/> |<span data-ttu-id="65cb5-168">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="65cb5-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65cb5-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65cb5-169">Can be empty</span></span>  <br/> |<span data-ttu-id="65cb5-170">False</span><span class="sxs-lookup"><span data-stu-id="65cb5-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65cb5-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65cb5-171">See also</span></span>

- [<span data-ttu-id="65cb5-172">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="65cb5-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="65cb5-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65cb5-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="65cb5-174">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="65cb5-174">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

