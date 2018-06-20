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
ms.openlocfilehash: 5754ea7540fa6daac8cd725386ca213d5bf05c8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756383"
---
# <a name="findconversationresponse"></a><span data-ttu-id="c51c4-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="c51c4-103">FindConversationResponse</span></span>

<span data-ttu-id="c51c4-104">L’élément **FindConversationResponse** définit une réponse à une demande [d’opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c51c4-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="c51c4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="c51c4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="c51c4-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c51c4-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c51c4-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c51c4-107">Attributes and elements</span></span>

<span data-ttu-id="c51c4-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c51c4-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c51c4-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="c51c4-109">Attributes</span></span>

|<span data-ttu-id="c51c4-110">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c51c4-110">**Attribute**</span></span>|<span data-ttu-id="c51c4-111">**Description**</span><span class="sxs-lookup"><span data-stu-id="c51c4-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c51c4-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c51c4-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c51c4-113">Décrit l’état d’une réponse de [l’opération FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c51c4-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="c51c4-114">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="c51c4-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="c51c4-115">-Réussite</span><span class="sxs-lookup"><span data-stu-id="c51c4-115">-  Success</span></span>  <br/><span data-ttu-id="c51c4-116">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="c51c4-116">-  Warning</span></span>  <br/><span data-ttu-id="c51c4-117">-Erreur</span><span class="sxs-lookup"><span data-stu-id="c51c4-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c51c4-118">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c51c4-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="c51c4-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c51c4-119">**Value**</span></span>|<span data-ttu-id="c51c4-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="c51c4-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c51c4-121">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="c51c4-121">**Success**</span></span> <br/> |<span data-ttu-id="c51c4-122">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="c51c4-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c51c4-123">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="c51c4-123">**Warning**</span></span> <br/> | <span data-ttu-id="c51c4-124">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="c51c4-124">Describes a request that was not processed.</span></span> <span data-ttu-id="c51c4-125">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="c51c4-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="c51c4-126">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="c51c4-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="c51c4-127">-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="c51c4-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c51c4-128">-Services de domaine actives Directory (AD DS) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="c51c4-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="c51c4-129">-Boîtes aux lettres ont été déplacés.</span><span class="sxs-lookup"><span data-stu-id="c51c4-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="c51c4-130">-La base de données de message (MDB) est en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="c51c4-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c51c4-131">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="c51c4-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="c51c4-132">-Un quota a été dépassé.</span><span class="sxs-lookup"><span data-stu-id="c51c4-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="c51c4-133">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="c51c4-133">**Error**</span></span> <br/> | <span data-ttu-id="c51c4-134">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="c51c4-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c51c4-135">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="c51c4-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c51c4-136">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="c51c4-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c51c4-137">-Attributs ou éléments qui se trouvent en dehors des limites</span><span class="sxs-lookup"><span data-stu-id="c51c4-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="c51c4-138">-Une balise inconnue</span><span class="sxs-lookup"><span data-stu-id="c51c4-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="c51c4-139">-Un attribut ou un élément qui n’est pas valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="c51c4-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="c51c4-140">-Une tentative d’accès non autorisés par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="c51c4-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c51c4-141">-Une panne côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="c51c4-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c51c4-142">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="c51c4-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c51c4-143">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c51c4-143">Child elements</span></span>

|<span data-ttu-id="c51c4-144">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c51c4-144">**Element**</span></span>|<span data-ttu-id="c51c4-145">**Description**</span><span class="sxs-lookup"><span data-stu-id="c51c4-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c51c4-146">Conversations</span><span class="sxs-lookup"><span data-stu-id="c51c4-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c51c4-147">Contient un tableau des conversations.</span><span class="sxs-lookup"><span data-stu-id="c51c4-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="c51c4-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c51c4-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c51c4-149">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="c51c4-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c51c4-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c51c4-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c51c4-151">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="c51c4-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c51c4-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c51c4-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c51c4-153">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="c51c4-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c51c4-154">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="c51c4-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c51c4-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c51c4-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c51c4-156">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="c51c4-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c51c4-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c51c4-157">Parent elements</span></span>

<span data-ttu-id="c51c4-158">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c51c4-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c51c4-159">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c51c4-159">Text value</span></span>

<span data-ttu-id="c51c4-160">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c51c4-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c51c4-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="c51c4-161">Remarks</span></span>

<span data-ttu-id="c51c4-162">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c51c4-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c51c4-163">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c51c4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c51c4-164">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c51c4-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c51c4-165">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c51c4-165">Schema name</span></span>  <br/> |<span data-ttu-id="c51c4-166">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c51c4-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c51c4-167">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c51c4-167">Validation file</span></span>  <br/> |<span data-ttu-id="c51c4-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c51c4-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c51c4-169">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c51c4-169">Can be empty</span></span>  <br/> |<span data-ttu-id="c51c4-170">False</span><span class="sxs-lookup"><span data-stu-id="c51c4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c51c4-171">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c51c4-171">See also</span></span>

- [<span data-ttu-id="c51c4-172">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="c51c4-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="c51c4-173">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c51c4-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c51c4-174">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="c51c4-174">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

