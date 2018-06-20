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
description: L’élément CopyItemResponseMessage contient l’état et les résultats d’une demande d’opération CopyItem unique.
ms.openlocfilehash: 6c1acaff422fd731ca81a3ab244d76a73f3b5c15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755671"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="b30bc-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b30bc-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="b30bc-104">L’élément **CopyItemResponseMessage** contient l’état et les résultats d’une seule demande [d’opération CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b30bc-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="b30bc-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b30bc-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b30bc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b30bc-106">Attributes and elements</span></span>

<span data-ttu-id="b30bc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b30bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b30bc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b30bc-108">Attributes</span></span>

|<span data-ttu-id="b30bc-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b30bc-109">**Attribute**</span></span>|<span data-ttu-id="b30bc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b30bc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b30bc-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b30bc-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b30bc-112">Décrit l’état d’une réponse de [l’opération CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b30bc-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="b30bc-113">Les valeurs suivantes sont valides pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="b30bc-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="b30bc-114">-Réussite</span><span class="sxs-lookup"><span data-stu-id="b30bc-114">- Success</span></span>  <br/><span data-ttu-id="b30bc-115">-Avertissement</span><span class="sxs-lookup"><span data-stu-id="b30bc-115">-  Warning</span></span>  <br/><span data-ttu-id="b30bc-116">-Erreur</span><span class="sxs-lookup"><span data-stu-id="b30bc-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b30bc-117">Valeurs des attributs ResponseClass</span><span class="sxs-lookup"><span data-stu-id="b30bc-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b30bc-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b30bc-118">**Value**</span></span>|<span data-ttu-id="b30bc-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="b30bc-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b30bc-120">**Opération réussie**</span><span class="sxs-lookup"><span data-stu-id="b30bc-120">**Success**</span></span> <br/> |<span data-ttu-id="b30bc-121">Décrit une demande est remplie.</span><span class="sxs-lookup"><span data-stu-id="b30bc-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b30bc-122">**Avertissement**</span><span class="sxs-lookup"><span data-stu-id="b30bc-122">**Warning**</span></span> <br/> | <span data-ttu-id="b30bc-123">Décrit une demande qui n’a pas aboutie.</span><span class="sxs-lookup"><span data-stu-id="b30bc-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b30bc-124">Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.</span><span class="sxs-lookup"><span data-stu-id="b30bc-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="b30bc-125">Voici des exemples de sources d’avertissements :</span><span class="sxs-lookup"><span data-stu-id="b30bc-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="b30bc-126">-La banque d’informations Exchange est déconnecté pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="b30bc-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="b30bc-127">-Services de domaine actives Directory (AD DS) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b30bc-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="b30bc-128">-Boîtes aux lettres sont déplacées.</span><span class="sxs-lookup"><span data-stu-id="b30bc-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b30bc-129">-La base de données de boîtes aux lettres (MDB) passe en mode hors connexion.</span><span class="sxs-lookup"><span data-stu-id="b30bc-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="b30bc-130">-Un mot de passe a expiré.</span><span class="sxs-lookup"><span data-stu-id="b30bc-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b30bc-131">-Un quota est dépassé.</span><span class="sxs-lookup"><span data-stu-id="b30bc-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="b30bc-132">**Erreur**</span><span class="sxs-lookup"><span data-stu-id="b30bc-132">**Error**</span></span> <br/> | <span data-ttu-id="b30bc-133">Décrit une demande ne peut pas être traitée.</span><span class="sxs-lookup"><span data-stu-id="b30bc-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="b30bc-134">Voici des exemples de sources d’erreurs :</span><span class="sxs-lookup"><span data-stu-id="b30bc-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b30bc-135">-Non valide attributs ou éléments</span><span class="sxs-lookup"><span data-stu-id="b30bc-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b30bc-136">-Attributs ou éléments hors limites</span><span class="sxs-lookup"><span data-stu-id="b30bc-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="b30bc-137">-Balise inconnue</span><span class="sxs-lookup"><span data-stu-id="b30bc-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="b30bc-138">-Attribut ou un élément non valide dans le contexte</span><span class="sxs-lookup"><span data-stu-id="b30bc-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="b30bc-139">-Tentative d’accès non autorisé par n’importe quel client</span><span class="sxs-lookup"><span data-stu-id="b30bc-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b30bc-140">Échec du côté serveur en réponse à un appel côté client valid</span><span class="sxs-lookup"><span data-stu-id="b30bc-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="b30bc-141">Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="b30bc-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b30bc-142">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b30bc-142">Child elements</span></span>

|<span data-ttu-id="b30bc-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b30bc-143">**Element**</span></span>|<span data-ttu-id="b30bc-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="b30bc-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b30bc-145">- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="b30bc-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="b30bc-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="b30bc-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b30bc-147">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b30bc-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b30bc-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b30bc-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b30bc-149">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="b30bc-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b30bc-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b30bc-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b30bc-151">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="b30bc-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b30bc-152">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b30bc-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b30bc-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b30bc-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b30bc-154">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b30bc-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b30bc-155">Items</span><span class="sxs-lookup"><span data-stu-id="b30bc-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="b30bc-156">Contient un tableau d’éléments copiés</span><span class="sxs-lookup"><span data-stu-id="b30bc-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b30bc-157">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b30bc-157">Parent elements</span></span>

|<span data-ttu-id="b30bc-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b30bc-158">**Element**</span></span>|<span data-ttu-id="b30bc-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="b30bc-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b30bc-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b30bc-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b30bc-161">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b30bc-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b30bc-162">Remarques</span><span class="sxs-lookup"><span data-stu-id="b30bc-162">Remarks</span></span>

<span data-ttu-id="b30bc-163">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b30bc-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b30bc-164">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b30bc-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b30bc-165">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b30bc-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b30bc-166">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b30bc-166">Schema name</span></span>  <br/> |<span data-ttu-id="b30bc-167">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b30bc-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b30bc-168">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b30bc-168">Validation file</span></span>  <br/> |<span data-ttu-id="b30bc-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b30bc-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b30bc-170">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b30bc-170">Can be empty</span></span>  <br/> |<span data-ttu-id="b30bc-171">False</span><span class="sxs-lookup"><span data-stu-id="b30bc-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b30bc-172">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b30bc-172">See also</span></span>

- [<span data-ttu-id="b30bc-173">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="b30bc-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="b30bc-174">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b30bc-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

